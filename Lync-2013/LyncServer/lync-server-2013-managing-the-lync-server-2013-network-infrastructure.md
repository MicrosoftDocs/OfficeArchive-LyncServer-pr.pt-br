---
title: 'Lync Server 2013: Gerenciando a infraestrutura de rede do Lync Server 2013'
description: 'Lync Server 2013: gerenciamento da infraestrutura de rede do Lync Server 2013.'
ms.reviewer: ''
ms.author: v-lanac
author: lanachin
f1.keywords:
- NOCSH
TOCTitle: Managing the Lync Server 2013 network infrastructure
ms:assetid: cb13456a-8f66-4595-be21-8887f30ad4eb
ms:mtpsurl: https://technet.microsoft.com/en-us/library/Gg182585(v=OCS.15)
ms:contentKeyID: 48185638
ms.date: 07/23/2014
manager: serdars
mtps_version: v=OCS.15
ms.openlocfilehash: ab1b5c6fe52374b012063ac26640e9bb25496ad7
ms.sourcegitcommit: 36fee89bb887bea4f18b19f17a8c69daf5bc423d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2020
ms.locfileid: "49425854"
---
# <a name="managing-the-lync-server-2013-network-infrastructure"></a><span data-ttu-id="aeee7-103">Gerenciando a infraestrutura de rede do Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-103">Managing the Lync Server 2013 network infrastructure</span></span>

<div data-xmlns="http://www.w3.org/1999/xhtml">

<div class="topic" data-xmlns="http://www.w3.org/1999/xhtml" data-msxsl="urn:schemas-microsoft-com:xslt" data-cs="https://msdn.microsoft.com/">

<div data-asp="https://msdn2.microsoft.com/asp">



</div>

<div id="mainSection">

<div id="mainBody"><span data-ttu-id="aeee7-104">

<span> </span></span><span class="sxs-lookup"><span data-stu-id="aeee7-104">

<span> </span></span></span>

<span data-ttu-id="aeee7-105">_**Tópico da última modificação:** 2014-02-11_</span><span class="sxs-lookup"><span data-stu-id="aeee7-105">_**Topic Last Modified:** 2014-02-11_</span></span>

<span data-ttu-id="aeee7-106">O Microsoft Lync Server 2013 inclui suporte para o controle de admissão de chamadas (CAC) e bypass de mídia.</span><span class="sxs-lookup"><span data-stu-id="aeee7-106">Microsoft Lync Server 2013 includes support for call admission control (CAC) and media bypass.</span></span> <span data-ttu-id="aeee7-107">Para implementar esses recursos, você deve configurar uma rede de regiões, sites, sub-redes e assim por diante que permitirá que você gerencie a largura de banda em situações nas quais as transmissões de áudio e vídeo precisam ser restritas.</span><span class="sxs-lookup"><span data-stu-id="aeee7-107">To implement these features you must configure a network of regions, sites, subnets, and so on that will allow you to manage bandwidth in situations where audio and video transmissions need to be restricted.</span></span> <span data-ttu-id="aeee7-108">Você também pode usar a tecnologia de rede de qualidade de serviço (QoS) para ajudar a oferecer uma experiência ideal para os usuários finais de comunicações de áudio e vídeo.</span><span class="sxs-lookup"><span data-stu-id="aeee7-108">You can also use the Quality of Service (QoS) networking technology to help provide an optimal end-user experience for audio and video communications.</span></span>

<span data-ttu-id="aeee7-109">Você pode usar o painel de controle do Lync Server para configurar e gerenciar o CAC, o bypass de mídia e a QoS.</span><span class="sxs-lookup"><span data-stu-id="aeee7-109">You can use the Lync Server Control Panel to set up and manage CAC, media bypass, and QoS.</span></span> <span data-ttu-id="aeee7-110">Os tópicos a seguir fornecem etapas para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="aeee7-110">The following topics provide steps for how to do this.</span></span>

<div>

## <a name="in-this-section"></a><span data-ttu-id="aeee7-111">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="aeee7-111">In This Section</span></span>

  - [<span data-ttu-id="aeee7-112">Gerenciando a qualidade do serviço (QoS) no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-112">Managing Quality of Service (QoS) in Lync Server 2013</span></span>](lync-server-2013-managing-quality-of-service-qos.md)

  - [<span data-ttu-id="aeee7-113">Gerenciando o controle de admissão de chamadas no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-113">Managing call admission control in Lync Server 2013</span></span>](lync-server-2013-managing-call-admission-control.md)

  - [<span data-ttu-id="aeee7-114">Interfaces de rede do Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-114">Lync Server 2013 network interfaces</span></span>](lync-server-2013-lync-server-network-interfaces.md)

  - [<span data-ttu-id="aeee7-115">Impedir novas conexões com o Lync Server 2013 para manutenção do servidor</span><span class="sxs-lookup"><span data-stu-id="aeee7-115">Prevent new connections to Lync Server 2013 for server maintenance</span></span>](lync-server-2013-prevent-new-connections-to-lync-server-for-server-maintenance.md)

  - [<span data-ttu-id="aeee7-116">Metodologia de qualidade de chamada do Lync no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-116">Lync Call Quality Methodology in Lync Server 2013</span></span>](lync-server-2013-poster-lync-call-quality-methodology.md)

  - [<span data-ttu-id="aeee7-117">Principais indicadores de integridade no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="aeee7-117">Key Health Indicators in Lync Server 2013</span></span>](lync-server-2013-poster-key-health-indicators.md)

<span data-ttu-id="aeee7-118"></div>

</div>

<span> </span>

</div>

</div>

</span><span class="sxs-lookup"><span data-stu-id="aeee7-118"></div>

</div>

<span> </span>

</div>

</div>

</span></span></div>

