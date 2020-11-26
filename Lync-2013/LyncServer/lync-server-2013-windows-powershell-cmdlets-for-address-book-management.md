---
title: 'Lync Server 2013: cmdlets do Windows PowerShell para gerenciamento de catálogo de endereços'
description: 'Lync Server 2013: cmdlets do Windows PowerShell para gerenciamento de catálogo de endereços.'
ms.reviewer: ''
ms.author: v-lanac
author: lanachin
f1.keywords:
- NOCSH
TOCTitle: Windows PowerShell cmdlets for Address Book management
ms:assetid: 73bfa949-5628-4156-ad20-fe07a0dc6216
ms:mtpsurl: https://technet.microsoft.com/en-us/library/Gg429708(v=OCS.15)
ms:contentKeyID: 48184512
ms.date: 07/23/2014
manager: serdars
mtps_version: v=OCS.15
ms.openlocfilehash: b598d91a4d1a29a67d8f8ceb2477f2d9b96f1319
ms.sourcegitcommit: 36fee89bb887bea4f18b19f17a8c69daf5bc423d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/26/2020
ms.locfileid: "49446174"
---
# <a name="windows-powershell-cmdlets-for-address-book-services-in-lync-server-2013"></a><span data-ttu-id="67fe3-103">Cmdlets do Windows PowerShell para serviços de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-103">Windows PowerShell cmdlets for Address Book Services in Lync Server 2013</span></span>

<div data-xmlns="http://www.w3.org/1999/xhtml">

<div class="topic" data-xmlns="http://www.w3.org/1999/xhtml" data-msxsl="urn:schemas-microsoft-com:xslt" data-cs="https://msdn.microsoft.com/">

<div data-asp="https://msdn2.microsoft.com/asp">



</div>

<div id="mainSection">

<div id="mainBody"><span data-ttu-id="67fe3-104">

<span> </span></span><span class="sxs-lookup"><span data-stu-id="67fe3-104">

<span> </span></span></span>

<span data-ttu-id="67fe3-105">_**Tópico da última modificação:** 2012-11-01_</span><span class="sxs-lookup"><span data-stu-id="67fe3-105">_**Topic Last Modified:** 2012-11-01_</span></span>

<span data-ttu-id="67fe3-106">O Lync Server fornece vários cmdlets de interface de linha de comando do Windows PowerShell para gerenciar e configurar o serviço de catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="67fe3-106">Lync Server provides a number of Windows PowerShell command-line interface cmdlets to manage and configure the Address Book service.</span></span> <span data-ttu-id="67fe3-107">Alguns desses cmdlets são substituições para os comandos ABServer.exe usados nas versões anteriores do Office Communications Server.</span><span class="sxs-lookup"><span data-stu-id="67fe3-107">Some of these cmdlets are replacements for the ABServer.exe commands used in previous versions of Office Communications Server.</span></span> <span data-ttu-id="67fe3-108">Nos tópicos a seguir estão os cmdlets que são usados para definir, criar e recuperar informações sobre o serviço de catálogo de endereços, suas configurações e informações sobre os serviços Web que o serviço catálogo de endereços usa quando os clientes recuperam arquivos e configurações do serviço de catálogo de endereços.</span><span class="sxs-lookup"><span data-stu-id="67fe3-108">In the following topics are the cmdlets that are used to set, create, and retrieve information about the Address Book service, its configuration and information about the Web services that the Address Book service uses when clients retrieve Address Book service files and settings.</span></span>

<span data-ttu-id="67fe3-109">Todos esses cmdlets são emitidos por meio do Shell de gerenciamento do Lync Server localizado nas ferramentas do Lync Server em um servidor ou estação de trabalho onde as ferramentas de administração foram instaladas.</span><span class="sxs-lookup"><span data-stu-id="67fe3-109">All of these cmdlets are issued through the Lync Server Management Shell found in the Lync Server tools on a server or workstation where the administration tools have been installed.</span></span>

<div>

## <a name="in-this-section"></a><span data-ttu-id="67fe3-110">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="67fe3-110">In This Section</span></span>

  - [<span data-ttu-id="67fe3-111">New-CsAddressBookConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-111">New-CsAddressBookConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-New-CsAddressBookConfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-112">Set-CsAddressBookConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-112">Set-CsAddressBookConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-set-csaddressbookconfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-113">Get-CsAddressBookConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-113">Get-CsAddressBookConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-get-csaddressbookconfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-114">Remove-CsAddressBookConfiguration para gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-114">Remove-CsAddressBookConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-remove-csaddressbookconfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-115">Test-CsAddressBookService para gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-115">Test-CsAddressBookService for Address Book management in Lync Server 2013</span></span>](lync-server-2013-test-csaddressbookservice-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-116">Test-CsAddressBookWebQuery para gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-116">Test-CsAddressBookWebQuery for Address Book management in Lync Server 2013</span></span>](lync-server-2013-test-csaddressbookwebquery-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-117">Update-CsAddressBook para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-117">Update-CsAddressBook for Address Book management in Lync Server 2013</span></span>](lync-server-2013-update-csaddressbook-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-118">New-CsClientPolicy para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-118">New-CsClientPolicy for Address Book management in Lync Server 2013</span></span>](lync-server-2013-new-csclientpolicy-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-119">Set-CsClientPolicy para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-119">Set-CsClientPolicy for Address Book management in Lync Server 2013</span></span>](lync-server-2013-set-csclientpolicy-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-120">Get-CsService para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-120">Get-CsService for Address Book management in Lync Server 2013</span></span>](lync-server-2013-get-csservice-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-121">New-CsWebServiceConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-121">New-CsWebServiceConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-New-CsWebServiceConfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-122">Get-CsWebServiceConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-122">Get-CsWebServiceConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-get-cswebserviceconfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-123">Set-CsWebServiceConfiguration para o gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-123">Set-CsWebServiceConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-set-cswebserviceconfiguration-for-address-book-management.md)

  - [<span data-ttu-id="67fe3-124">Remove-CsWebServiceConfiguration para gerenciamento de catálogo de endereços no Lync Server 2013</span><span class="sxs-lookup"><span data-stu-id="67fe3-124">Remove-CsWebServiceConfiguration for Address Book management in Lync Server 2013</span></span>](lync-server-2013-remove-cswebserviceconfiguration-for-address-book-management.md)

</div>

<div>

## <a name="related-sections"></a><span data-ttu-id="67fe3-125">Seções Relacionadas</span><span class="sxs-lookup"><span data-stu-id="67fe3-125">Related Sections</span></span>

</div>

<div>

## <a name="see-also"></a><span data-ttu-id="67fe3-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="67fe3-126">See Also</span></span>


[https://go.microsoft.com/fwlink/p/?linkId=205826](https://go.microsoft.com/fwlink/p/?linkid=205826)  
  

<span data-ttu-id="67fe3-127"></div>

</div>

<span> </span>

</div>

</div>

</span><span class="sxs-lookup"><span data-stu-id="67fe3-127"></div>

</div>

<span> </span>

</div>

</div>

</span></span></div>

