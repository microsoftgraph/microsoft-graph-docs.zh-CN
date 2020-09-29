---
title: Intune 设备和应用 API 概述
description: 'Microsoft Intune 可帮助企业管理组织内的设备和应用。 你可以使用 Microsoft Graph 中的 Intune API 来管理设备和应用，甚至可以在使用首选工具时配置 Intune。 '
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: a3fa7e8dcd60a5070e7f52a307d355e0e0df4d04
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288347"
---
# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="9be2a-104">Intune 设备和应用 API 概述</span><span class="sxs-lookup"><span data-stu-id="9be2a-104">Intune devices and apps API overview</span></span>

<span data-ttu-id="9be2a-105">Microsoft Intune 可帮助企业管理组织内的设备和应用。</span><span class="sxs-lookup"><span data-stu-id="9be2a-105">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="9be2a-106">你可以使用 Microsoft Graph 中的 Intune API 来管理设备和应用，甚至可以在使用首选工具时配置 Intune。</span><span class="sxs-lookup"><span data-stu-id="9be2a-106">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="9be2a-107">如果你是 ISV，则还可以使用 Intune API 来管理客户端租户。</span><span class="sxs-lookup"><span data-stu-id="9be2a-107">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a><span data-ttu-id="9be2a-108">为什么与 Intune 集成？</span><span class="sxs-lookup"><span data-stu-id="9be2a-108">Why integrate with Intune?</span></span>

<span data-ttu-id="9be2a-109">你可以使用 Microsoft Graph 中的 Intune API 访问 Intune 设备和应用程序信息，管理设备、管理应用和自动执行 Intune。</span><span class="sxs-lookup"><span data-stu-id="9be2a-109">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="9be2a-110">管理设备</span><span class="sxs-lookup"><span data-stu-id="9be2a-110">Manage devices</span></span>

<span data-ttu-id="9be2a-111">可以使用 Intune API 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="9be2a-111">You can use the Intune API to:</span></span>

- <span data-ttu-id="9be2a-112">定义并强制实施[设备合规性](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)策略，例如密码复杂性和持续时间、加密、威胁保护级别等。</span><span class="sxs-lookup"><span data-stu-id="9be2a-112">Define and enforce [device compliance](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="9be2a-113">（支持的策略会根据操作系统和版本的不同而异）。</span><span class="sxs-lookup"><span data-stu-id="9be2a-113">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="9be2a-114">[保护公司数据](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)，无论设备平台是 Windows、Android、Mac 还是 iOS。</span><span class="sxs-lookup"><span data-stu-id="9be2a-114">[Protect company data](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="9be2a-115">创建和部署[设备配置](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)策略，包括操作系统平台/版本控制、域成员身份和配置设置管理。</span><span class="sxs-lookup"><span data-stu-id="9be2a-115">Create and deploy [device configuration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="9be2a-116">创建和部署设备[访问控制](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)策略，包括受限的下载、网络附件访问和文件传输。</span><span class="sxs-lookup"><span data-stu-id="9be2a-116">Create and deploy device [access control](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="9be2a-117">执行[远程操作](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)，如定位设备、更改密码和擦除设备。</span><span class="sxs-lookup"><span data-stu-id="9be2a-117">Perform [remote actions](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="9be2a-118">管理应用</span><span class="sxs-lookup"><span data-stu-id="9be2a-118">Manage apps</span></span> 

<span data-ttu-id="9be2a-119">Intune API 可用于执行下列应用管理任务：</span><span class="sxs-lookup"><span data-stu-id="9be2a-119">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="9be2a-120">[将应用部署到设备](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)或阻止部署应用。</span><span class="sxs-lookup"><span data-stu-id="9be2a-120">Deploy [apps to devices](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="9be2a-121">管理对[电子书](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)及相关服务的访问。</span><span class="sxs-lookup"><span data-stu-id="9be2a-121">Manage access to [ebooks](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0) and related services.</span></span>
- <span data-ttu-id="9be2a-122">定义和部署应用配置设置、应用保护设置和应用使用策略。</span><span class="sxs-lookup"><span data-stu-id="9be2a-122">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="9be2a-123">自动执行 Intune</span><span class="sxs-lookup"><span data-stu-id="9be2a-123">Automate Intune</span></span>

<span data-ttu-id="9be2a-124">使用 Intune API 自动执行 Intune 可进行以下操作：</span><span class="sxs-lookup"><span data-stu-id="9be2a-124">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="9be2a-125">定义和分配[基于角色的](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0)访问控件。</span><span class="sxs-lookup"><span data-stu-id="9be2a-125">Define and assign [role based](/graph/api/resources/intune-rbac-conceptual?view=graph-rest-1.0) access controls.</span></span>
- <span data-ttu-id="9be2a-126">审核和报告合规性、使用情况和访问权限。</span><span class="sxs-lookup"><span data-stu-id="9be2a-126">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="9be2a-127">管理[电信费用](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="9be2a-127">Manage [telecom expenses](/graph/api/resources/intune-tem-conceptual?view=graph-rest-1.0).</span></span>

## <a name="api-reference"></a><span data-ttu-id="9be2a-128">API 参考</span><span class="sxs-lookup"><span data-stu-id="9be2a-128">API reference</span></span>
<span data-ttu-id="9be2a-129">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="9be2a-129">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="9be2a-130">Microsoft Graph v1.0 中的 Intune API</span><span class="sxs-lookup"><span data-stu-id="9be2a-130">Intune API in Microsoft Graph v1.0</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)
- [<span data-ttu-id="9be2a-131">Microsoft Graph beta 中的 Intune API</span><span class="sxs-lookup"><span data-stu-id="9be2a-131">Intune API in Microsoft Graph beta</span></span>](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="9be2a-132">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9be2a-132">Next steps</span></span>

- <span data-ttu-id="9be2a-133">[使用 Azure AD 访问 Intune API](/intune/intune-graph-apis)。</span><span class="sxs-lookup"><span data-stu-id="9be2a-133">[Use Azure AD to access the Intune API](/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="9be2a-134">了解如何使用 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)执行常见任务。</span><span class="sxs-lookup"><span data-stu-id="9be2a-134">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="9be2a-135">了解如何[使用 Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="9be2a-135">Find out how to [use the Intune REST API](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="9be2a-136">有关 Intune API 中新增功能的信息，请参阅[更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="9be2a-136">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="9be2a-137">浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="9be2a-137">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>