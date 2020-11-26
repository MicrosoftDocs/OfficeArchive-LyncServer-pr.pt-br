---
title: 'Lync Server 2013: Definindo seus requisitos para chamadas de emergência'
description: 'Lync Server 2013: definindo seus requisitos de chamadas de emergência.'
ms.reviewer: ''
ms.author: v-lanac
author: lanachin
f1.keywords:
- NOCSH
TOCTitle: Defining your requirements for emergency calls
ms:assetid: 5c12b517-9be6-41d0-83e2-11c78793620c
ms:mtpsurl: https://technet.microsoft.com/en-us/library/Gg398404(v=OCS.15)
ms:contentKeyID: 48184276
ms.date: 07/23/2014
manager: serdars
mtps_version: v=OCS.15
ms.openlocfilehash: 8d3c9908dcb4008a1442af86971e42eb4096a98b
ms.sourcegitcommit: 36fee89bb887bea4f18b19f17a8c69daf5bc423d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2020
ms.locfileid: "49430830"
---
# <a name="defining-your-requirements-for-emergency-calls-in-lync-server-2013"></a><span data-ttu-id="5d489-103">Definindo seus requisitos para chamadas de emergência no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-103">Defining your requirements for emergency calls in Lync Server 2013</span></span>

<div data-xmlns="http://www.w3.org/1999/xhtml">

<div class="topic" data-xmlns="http://www.w3.org/1999/xhtml" data-msxsl="urn:schemas-microsoft-com:xslt" data-cs="https://msdn.microsoft.com/">

<div data-asp="https://msdn2.microsoft.com/asp">



</div>

<div id="mainSection">

<div id="mainBody"><span data-ttu-id="5d489-104">

<span> </span></span><span class="sxs-lookup"><span data-stu-id="5d489-104">

<span> </span></span></span>

<span data-ttu-id="5d489-105">_**Tópico da última modificação:** 2012-06-06_</span><span class="sxs-lookup"><span data-stu-id="5d489-105">_**Topic Last Modified:** 2012-06-06_</span></span>

<span data-ttu-id="5d489-106">Antes de começar uma implantação do Microsoft Lync Server 2013 E9-1-1, você deve primeiro poder responder às perguntas detalhadas nas seções a seguir.</span><span class="sxs-lookup"><span data-stu-id="5d489-106">Before you begin a Microsoft Lync Server 2013 E9-1-1 deployment, you should first be able to answer the questions detailed in the following sections.</span></span> <span data-ttu-id="5d489-107">O planejamento necessário dependerá do tipo de solução E9-1-1 que você optar por implantar: um provedor de serviços E9-1-1 de tronco SIP ou um gateway ELIN (número de identificação de local de emergência).</span><span class="sxs-lookup"><span data-stu-id="5d489-107">The planning you need to do depends on the type of E9-1-1 solution that you choose to deploy—a SIP trunk E9-1-1 service provider or an Emergency Location Identification Number (ELIN) gateway.</span></span> <span data-ttu-id="5d489-108">A tabela a seguir identifica as seções desta apostila de planejamento que você precisará consultar para cada uma dessas soluções.</span><span class="sxs-lookup"><span data-stu-id="5d489-108">The following table identifies the sections in this planning workbook that you’ll need to review for each of those solutions.</span></span>

### <a name="planning-steps-by-type-of-e9-1-1-solution"></a><span data-ttu-id="5d489-109">Planejando as etapas por tipo de solução E9-1-1</span><span class="sxs-lookup"><span data-stu-id="5d489-109">Planning Steps by Type of E9-1-1 Solution</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="5d489-110">Provedor de serviços de tronco SIP</span><span class="sxs-lookup"><span data-stu-id="5d489-110">SIP trunk service provider</span></span></th>
<th><span data-ttu-id="5d489-111">Gateway ELIN</span><span class="sxs-lookup"><span data-stu-id="5d489-111">ELIN gateway</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="5d489-112"><a href="lync-server-2013-defining-the-scope-of-the-e9-1-1-deployment.md">Definindo o escopo da implantação do E9-1-1 no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-112"><a href="lync-server-2013-defining-the-scope-of-the-e9-1-1-deployment.md">Defining the scope of the E9-1-1 deployment in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-113"><a href="lync-server-2013-defining-the-scope-of-the-e9-1-1-deployment.md">Definindo o escopo da implantação do E9-1-1 no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-113"><a href="lync-server-2013-defining-the-scope-of-the-e9-1-1-deployment.md">Defining the scope of the E9-1-1 deployment in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d489-114"><a href="lync-server-2013-defining-the-network-elements-used-to-determine-location.md">Definindo os elementos de rede usados para determinar o local no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-114"><a href="lync-server-2013-defining-the-network-elements-used-to-determine-location.md">Defining the network elements used to determine location in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-115"><a href="lync-server-2013-defining-the-network-elements-used-to-determine-location.md">Definindo os elementos de rede usados para determinar o local no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-115"><a href="lync-server-2013-defining-the-network-elements-used-to-determine-location.md">Defining the network elements used to determine location in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5d489-116"><a href="lync-server-2013-enabling-users-for-e9-1-1.md">Permitindo que os usuários do E9-1-1 no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-116"><a href="lync-server-2013-enabling-users-for-e9-1-1.md">Enabling users for E9-1-1 in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-117"><a href="lync-server-2013-enabling-users-for-e9-1-1.md">Permitindo que os usuários do E9-1-1 no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-117"><a href="lync-server-2013-enabling-users-for-e9-1-1.md">Enabling users for E9-1-1 in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d489-118"><a href="lync-server-2013-managing-locations-for-sip-trunk-service-providers.md">Gerenciando locais para provedores de serviço de tronco SIP no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-118"><a href="lync-server-2013-managing-locations-for-sip-trunk-service-providers.md">Managing locations for SIP trunk service providers in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-119"><a href="lync-server-2013-managing-locations-for-elin-gateways.md">Gerenciando locais para gateways do ELIN no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-119"><a href="lync-server-2013-managing-locations-for-elin-gateways.md">Managing locations for ELIN gateways in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5d489-120"><a href="lync-server-2013-defining-the-user-experience-for-manually-acquiring-a-location.md">Definindo a experiência do usuário para adquirir manualmente um local no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-120"><a href="lync-server-2013-defining-the-user-experience-for-manually-acquiring-a-location.md">Defining the user experience for manually acquiring a location in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-121"><a href="lync-server-2013-defining-the-user-experience-for-manually-acquiring-a-location.md">Definindo a experiência do usuário para adquirir manualmente um local no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-121"><a href="lync-server-2013-defining-the-user-experience-for-manually-acquiring-a-location.md">Defining the user experience for manually acquiring a location in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d489-122"><a href="lync-server-2013-designing-the-sip-trunk-for-e9-1-1.md">Criando o tronco SIP para E9-1-1 no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-122"><a href="lync-server-2013-designing-the-sip-trunk-for-e9-1-1.md">Designing the SIP trunk for E9-1-1 in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-123"><a href="lync-server-2013-including-the-security-desk.md">Incluindo a central de segurança no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-123"><a href="lync-server-2013-including-the-security-desk.md">Including the security desk in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5d489-124"><a href="lync-server-2013-including-the-security-desk.md">Incluindo a central de segurança no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-124"><a href="lync-server-2013-including-the-security-desk.md">Including the security desk in Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-125"><a href="lync-server-2013-defining-the-location-policy.md">Definindo a política de localização do Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-125"><a href="lync-server-2013-defining-the-location-policy.md">Defining the location policy for Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d489-126"><a href="lync-server-2013-choosing-an-e9-1-1-service-provider.md">Escolher um provedor de serviços E9-1-1 para o Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-126"><a href="lync-server-2013-choosing-an-e9-1-1-service-provider.md">Choosing an E9-1-1 service provider for Lync Server 2013</a></span></span></p></td>
<td><p><span data-ttu-id="5d489-127"><a href="lync-server-2013-assigning-location-policy-scope.md">Atribuindo o escopo da política de localização no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-127"><a href="lync-server-2013-assigning-location-policy-scope.md">Assigning location policy scope in Lync Server 2013</a></span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5d489-128"><a href="lync-server-2013-defining-the-location-policy.md">Definindo a política de localização do Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-128"><a href="lync-server-2013-defining-the-location-policy.md">Defining the location policy for Lync Server 2013</a></span></span></p></td>
<td></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5d489-129"><a href="lync-server-2013-assigning-location-policy-scope.md">Atribuindo o escopo da política de localização no Lync Server 2013</a></span><span class="sxs-lookup"><span data-stu-id="5d489-129"><a href="lync-server-2013-assigning-location-policy-scope.md">Assigning location policy scope in Lync Server 2013</a></span></span></p></td>
<td></td>
</tr>
</tbody>
</table>


<div>

## <a name="in-this-section"></a><span data-ttu-id="5d489-130">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="5d489-130">In This Section</span></span>

  - [<span data-ttu-id="5d489-131">Definindo o escopo da implantação do E9-1-1 no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-131">Defining the scope of the E9-1-1 deployment in Lync Server 2013</span></span>](lync-server-2013-defining-the-scope-of-the-e9-1-1-deployment.md)

  - [<span data-ttu-id="5d489-132">Definindo os elementos de rede usados para determinar o local no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-132">Defining the network elements used to determine location in Lync Server 2013</span></span>](lync-server-2013-defining-the-network-elements-used-to-determine-location.md)

  - [<span data-ttu-id="5d489-133">Permitindo que os usuários do E9-1-1 no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-133">Enabling users for E9-1-1 in Lync Server 2013</span></span>](lync-server-2013-enabling-users-for-e9-1-1.md)

  - [<span data-ttu-id="5d489-134">Gerenciando locais para provedores de serviço de tronco SIP no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-134">Managing locations for SIP trunk service providers in Lync Server 2013</span></span>](lync-server-2013-managing-locations-for-sip-trunk-service-providers.md)

  - [<span data-ttu-id="5d489-135">Gerenciando locais para gateways do ELIN no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-135">Managing locations for ELIN gateways in Lync Server 2013</span></span>](lync-server-2013-managing-locations-for-elin-gateways.md)

  - [<span data-ttu-id="5d489-136">Definindo a experiência do usuário para adquirir manualmente um local no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-136">Defining the user experience for manually acquiring a location in Lync Server 2013</span></span>](lync-server-2013-defining-the-user-experience-for-manually-acquiring-a-location.md)

  - [<span data-ttu-id="5d489-137">Criando o tronco SIP para E9-1-1 no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-137">Designing the SIP trunk for E9-1-1 in Lync Server 2013</span></span>](lync-server-2013-designing-the-sip-trunk-for-e9-1-1.md)

  - [<span data-ttu-id="5d489-138">Incluindo a central de segurança no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-138">Including the security desk in Lync Server 2013</span></span>](lync-server-2013-including-the-security-desk.md)

  - [<span data-ttu-id="5d489-139">Escolher um provedor de serviços E9-1-1 para o Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-139">Choosing an E9-1-1 service provider for Lync Server 2013</span></span>](lync-server-2013-choosing-an-e9-1-1-service-provider.md)

  - [<span data-ttu-id="5d489-140">Definindo a política de localização do Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-140">Defining the location policy for Lync Server 2013</span></span>](lync-server-2013-defining-the-location-policy.md)

  - [<span data-ttu-id="5d489-141">Atribuindo o escopo da política de localização no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="5d489-141">Assigning location policy scope in Lync Server 2013</span></span>](lync-server-2013-assigning-location-policy-scope.md)

<span data-ttu-id="5d489-142"></div>

</div>

<span> </span>

</div>

</div>

</span><span class="sxs-lookup"><span data-stu-id="5d489-142"></div>

</div>

<span> </span>

</div>

</div>

</span></span></div>

