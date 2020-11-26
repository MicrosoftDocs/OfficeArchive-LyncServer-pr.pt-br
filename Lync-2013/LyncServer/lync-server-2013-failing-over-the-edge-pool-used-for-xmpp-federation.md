---
title: 'Lync Server 2013: Failover do pool de Borda usado para federação de XMPP'
description: 'Lync Server 2013: falha sobre o pool de bordas usado para Federação do XMPP.'
ms.reviewer: ''
ms.author: v-lanac
author: lanachin
f1.keywords:
- NOCSH
TOCTitle: Failing over the Edge pool used for XMPP federation
ms:assetid: 587e7829-a26b-46f8-8aad-b78a7b325b55
ms:mtpsurl: https://technet.microsoft.com/en-us/library/JJ688065(v=OCS.15)
ms:contentKeyID: 49733659
ms.date: 07/23/2014
manager: serdars
mtps_version: v=OCS.15
ms.openlocfilehash: ccdfe119258b4d09ddedefb22d0272d72003bf04
ms.sourcegitcommit: 36fee89bb887bea4f18b19f17a8c69daf5bc423d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2020
ms.locfileid: "49428248"
---
# <a name="failing-over-the-edge-pool-used-for-xmpp-federation-in-lync-server-2013"></a><span data-ttu-id="eca04-103">Failover do pool de Borda usado para federação de XMPP no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="eca04-103">Failing over the Edge pool used for XMPP federation in Lync Server 2013</span></span>

<div data-xmlns="http://www.w3.org/1999/xhtml">

<div class="topic" data-xmlns="http://www.w3.org/1999/xhtml" data-msxsl="urn:schemas-microsoft-com:xslt" data-cs="https://msdn.microsoft.com/">

<div data-asp="https://msdn2.microsoft.com/asp">



</div>

<div id="mainSection">

<div id="mainBody"><span data-ttu-id="eca04-104">

<span> </span></span><span class="sxs-lookup"><span data-stu-id="eca04-104">

<span> </span></span></span>

<span data-ttu-id="eca04-105">_**Tópico da última modificação:** 2012-10-19_</span><span class="sxs-lookup"><span data-stu-id="eca04-105">_**Topic Last Modified:** 2012-10-19_</span></span>

<span data-ttu-id="eca04-106">Em sua organização, há um pool de bordas designado como o pool a ser usado para a Federação do XMPP.</span><span class="sxs-lookup"><span data-stu-id="eca04-106">In your organization, there is one Edge pool designated as the pool to use for XMPP federation.</span></span> <span data-ttu-id="eca04-107">Se esse pool ficar inativo, você deve fazer failover da Federação do XMPP para usar um pool de bordas diferente antes que o XMPP federado possa funcionar novamente.</span><span class="sxs-lookup"><span data-stu-id="eca04-107">If this pool goes down, you must fail over XMPP federation to use a different Edge pool before XMPP federation can work again.</span></span>

<span data-ttu-id="eca04-108">Ao instalar primeiro os pools de borda e habilitar a Federação do XMPP, você pode simplificar o processo de recuperação de desastres Configurando os registros SRV DNS externos para todos os seus pools de bordas para a Federação do XMPP, em vez de apenas um.</span><span class="sxs-lookup"><span data-stu-id="eca04-108">When you first install Edge pools and enable XMPP Federation, you can simplify the disaster recovery process by setting up external DNS SRV records for all of your Edge pools for XMPP federation, instead of just one.</span></span> <span data-ttu-id="eca04-109">Cada um desses registros SRV deve ter um conjunto de prioridades diferente.</span><span class="sxs-lookup"><span data-stu-id="eca04-109">Each of these SRV records must have a different priority set.</span></span> <span data-ttu-id="eca04-110">Todo o tráfego de Federação do XMPP passa pelo pool com o registro SRV com a prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="eca04-110">All XMPP federation traffic goes through the pool with the SRV record with the highest priority.</span></span> <span data-ttu-id="eca04-111">Para obter mais informações sobre como habilitar e configurar a Federação do XMPP, consulte [Configurando a Federação do XMPP no Lync Server 2013](lync-server-2013-setting-up-xmpp-federation.md).</span><span class="sxs-lookup"><span data-stu-id="eca04-111">For more information on enabling and setting up XMPP federation, see [Setting up XMPP federation in Lync Server 2013](lync-server-2013-setting-up-xmpp-federation.md).</span></span>

<span data-ttu-id="eca04-112">No procedimento a seguir, EdgePool1 é o pool que hospeda originalmente a Federação do XMPP, e EdgePool2 é o pool que agora hospeda XMPP Federação.</span><span class="sxs-lookup"><span data-stu-id="eca04-112">In the following procedure, EdgePool1 is the pool which originally hosted XMPP federation, and EdgePool2 is the pool which will now host XMPP federation.</span></span>

<div>

## <a name="failing-over-the-edge-pool-used-for-xmpp-federation"></a><span data-ttu-id="eca04-113">Falha sobre o pool de bordas usado para a Federação do XMPP</span><span class="sxs-lookup"><span data-stu-id="eca04-113">Failing Over the Edge Pool Used for XMPP Federation</span></span>

1.  <span data-ttu-id="eca04-114">Se você ainda não tiver outro pool de bordas implantado (além do que está indisponível no momento), implante esse pool.</span><span class="sxs-lookup"><span data-stu-id="eca04-114">If you don’t already have another Edge pool deployed (besides the one which is currently down), deploy that pool.</span></span> <span data-ttu-id="eca04-115">Para obter detalhes, consulte [implantando o acesso de usuários externos no Lync Server 2013](lync-server-2013-deploying-external-user-access.md).</span><span class="sxs-lookup"><span data-stu-id="eca04-115">For details, see [Deploying external user access in Lync Server 2013](lync-server-2013-deploying-external-user-access.md).</span></span>

2.  <span data-ttu-id="eca04-116">Em cada servidor de borda no novo pool de bordas que agora hospeda a Federação do XMPP (EdgePool2), execute o seguinte cmdlet:</span><span class="sxs-lookup"><span data-stu-id="eca04-116">On each Edge Server in the new Edge pool which will now host XMPP federation (EdgePool2), run the following cmdlet:</span></span>
    
        Stop-CsWindowsService

3.  <span data-ttu-id="eca04-117">Execute o cmdlet a seguir para redirecionar a rota de Federação do XMPP para EdgePool2:</span><span class="sxs-lookup"><span data-stu-id="eca04-117">Run the following cmdlet to repoint the XMPP federation route to EdgePool2:</span></span>
    
        Set-CsSite Site2 -XmppExternalFederationRoute EdgeServer2.contoso.com
    
    <span data-ttu-id="eca04-118">Neste exemplo, site2 é o site que contém o pool de borda que agora hospeda a rota de Federação do XMPP, e EdgeServer2.contoso.com é o FQDN de um servidor de borda nesse pool.</span><span class="sxs-lookup"><span data-stu-id="eca04-118">In this example, Site2 is the site containing the Edge pool which will now host the XMPP federation route, and EdgeServer2.contoso.com is the FQDN of an Edge Server in that pool.</span></span>

4.  <span data-ttu-id="eca04-119">No servidor DNS externo, altere o registro DNS a para a Federação XMPP para apontar para EdgeServer2.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="eca04-119">On the external DNS server, change the DNS A record for XMPP federation to point to EdgeServer2.contoso.com.</span></span>

5.  <span data-ttu-id="eca04-120">Se você ainda não tiver um registro SRV DNS para a Federação do XMPP, que é resolvido para o pool de borda que agora hospedará a Federação do XMPP, você deve adicioná-lo, como no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="eca04-120">If you do not already have a DNS SRV record for XMPP federation which resolves to the Edge pool which will now host XMPP federation, you must add it, as in the following example.</span></span> <span data-ttu-id="eca04-121">Esse registro SRV deve ter um valor de porta 5269.</span><span class="sxs-lookup"><span data-stu-id="eca04-121">This SRV record must have a port value of 5269.</span></span>
    
        _xmpp-server._tcp.contoso.com

6.  <span data-ttu-id="eca04-122">Verifique se o pool de bordas que agora hospeda a Federação do XMPP tem a porta 5269 aberta externamente.</span><span class="sxs-lookup"><span data-stu-id="eca04-122">Verify that the Edge pool which will now host XMPP federation has port 5269 open externally.</span></span>

7.  <span data-ttu-id="eca04-123">Inicie os serviços em todos os servidores de borda do pool de borda que agora hospedarão a Federação do XMPP:</span><span class="sxs-lookup"><span data-stu-id="eca04-123">Start the services on all Edge Servers in the Edge pool which will now host XMPP federation:</span></span>
    
        Start-CsWindowsService

<span data-ttu-id="eca04-124"></div>

</div>

<span> </span>

</div>

</div>

</span><span class="sxs-lookup"><span data-stu-id="eca04-124"></div>

</div>

<span> </span>

</div>

</div>

</span></span></div>

