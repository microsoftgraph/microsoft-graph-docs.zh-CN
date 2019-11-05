---
title: Microsoft 信息保护标记概述
description: Microsoft 信息保护标签可帮助组织基于 Office 365 安全性和合规性中心敏感度标签对数据进行分类、标记和保护。
author: tommoser
localization_priority: Normal
ms.prod: microsoft.informationprotection
ms.openlocfilehash: cdbe4b3bdb7bdada33fa8c46c074280abcf6c174
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969827"
---
# <a name="information-protection-overview"></a><span data-ttu-id="785ee-103">信息保护概述</span><span class="sxs-lookup"><span data-stu-id="785ee-103">Information Protection overview</span></span>

<span data-ttu-id="785ee-104">Microsoft 信息保护可帮助组织根据[敏感度](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels)对数据进行分类、标记和保护。</span><span class="sxs-lookup"><span data-stu-id="785ee-104">Microsoft Information Protection helps organizations to classify, label, and protect data based on [sensitivity](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels).</span></span> 

<span data-ttu-id="785ee-105">组织使用标签来帮助：</span><span class="sxs-lookup"><span data-stu-id="785ee-105">Organizations use labels to aid:</span></span>

* <span data-ttu-id="785ee-106">了解正在处理的信息的重要性的用户。</span><span class="sxs-lookup"><span data-stu-id="785ee-106">Users in understanding the importance of information that is being handled.</span></span>
* <span data-ttu-id="785ee-107">在发现敏感信息所在的地方的合规管理员。</span><span class="sxs-lookup"><span data-stu-id="785ee-107">Compliance adminstrators in discovering where sensitive information lives.</span></span> 
* <span data-ttu-id="785ee-108">基于更丰富的标签信息部署数据访问和数据丢失防护策略的安全管理员。</span><span class="sxs-lookup"><span data-stu-id="785ee-108">Security administrators in deploying data access and data loss prevention policies based on more rich label information.</span></span>

## <a name="why-integrate-microsoft-information-protection"></a><span data-ttu-id="785ee-109">为什么要集成 Microsoft 信息保护？</span><span class="sxs-lookup"><span data-stu-id="785ee-109">Why integrate Microsoft Information Protection?</span></span> 

### <a name="integrate-with-the-ubiquitous-labeling-platform-servicing-millions-of-users-and-devices"></a><span data-ttu-id="785ee-110">与无处不在的用户和设备服务集成在一起使用的标签平台</span><span class="sxs-lookup"><span data-stu-id="785ee-110">Integrate with the ubiquitous labeling platform, servicing millions of users and devices</span></span>

<span data-ttu-id="785ee-111">拥有数十万个用户的多万个组织使用 Microsoft 信息保护对数据进行分类、添加标签和保护。</span><span class="sxs-lookup"><span data-stu-id="785ee-111">More than a million organizations with tens of millions of users use Microsoft Information Protection to classify, label, and protect data.</span></span>  <span data-ttu-id="785ee-112">除了 Office 365 之外，各种数据丢失防护（DLP）服务、商业智能平台和软件即用服务（SaaS）解决方案都采用[Microsoft 信息保护](https://www.microsoft.com/security/technology/information-protection)标签，以提供更丰富的数据分类体验.</span><span class="sxs-lookup"><span data-stu-id="785ee-112">In addition to Office 365, various data loss prevention (DLP) services, business intelligence platforms, and software-as-a-service (SaaS) solutions have [embraced Microsoft Information Protection](https://www.microsoft.com/security/technology/information-protection) labeling to provide a richer data classification experience.</span></span> 

### <a name="label-information-in-line-of-business-applications"></a><span data-ttu-id="785ee-113">在业务线应用程序中添加标签信息</span><span class="sxs-lookup"><span data-stu-id="785ee-113">Label information in line-of-business applications</span></span>

<span data-ttu-id="785ee-114">企业开发人员使用 Microsoft 信息保护在从业务线应用程序中导出时标记和保护敏感的客户信息，以确保客户信息的安全。</span><span class="sxs-lookup"><span data-stu-id="785ee-114">Enterprise developers use Microsoft Information Protection to label and protect sensitive customer information on export from line-of-business applications to ensure the safety of customer information.</span></span> <span data-ttu-id="785ee-115">将应用程序连接到 Microsoft 信息保护生态系统使应用程序能够在自己的应用程序数据中应用、更新和删除[敏感度标签](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels)，而不会导致集成完整 SDK 的开销。</span><span class="sxs-lookup"><span data-stu-id="785ee-115">Connecting your applications to the Microsoft Information Protection ecosystem enables applications to apply, update, and delete [sensitivity labels](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels) in your own application data, without the overhead of integrating a full SDK.</span></span>

## <a name="what-can-i-do-with-microsoft-information-protection-label-apis-in-microsoft-graph"></a><span data-ttu-id="785ee-116">在 Microsoft Graph 中，我可以使用 Microsoft 信息保护标签 Api 做什么？</span><span class="sxs-lookup"><span data-stu-id="785ee-116">What can I do with Microsoft Information Protection label APIs in Microsoft Graph?</span></span> 

### <a name="discover-labels-available-to-a-user-or-organization"></a><span data-ttu-id="785ee-117">发现用户或组织可以使用的标签</span><span class="sxs-lookup"><span data-stu-id="785ee-117">Discover labels available to a user or organization</span></span>

<span data-ttu-id="785ee-118">使用 Microsoft Graph，可以访问用户或组织可用的[敏感度标签](/graph/api/informationprotectionlabel?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="785ee-118">With Microsoft Graph you can access the [sensitivity labels](/graph/api/informationprotectionlabel?view=graph-rest-beta) available to a user or the organization.</span></span> <span data-ttu-id="785ee-119">标签由应用程序和服务应用于静止数据或移动数据，可帮助用户和下游应用程序和服务了解正在处理的信息的敏感度。</span><span class="sxs-lookup"><span data-stu-id="785ee-119">Labels are applied by applications and services to data at rest or in motion, helping users and downstream applications and services to understand the sensitivity of the information they're handling.</span></span>

### <a name="understand-how-to-apply-labels"></a><span data-ttu-id="785ee-120">了解如何应用标签</span><span class="sxs-lookup"><span data-stu-id="785ee-120">Understand how to apply labels</span></span>

<span data-ttu-id="785ee-121">通过提供有关现有和所需敏感度标签的信息，REST API 可智能地通知应用程序应采取的[操作](/graph/api/resources/informationprotectionaction?view=graph-rest-beta)才能正确应用标签。</span><span class="sxs-lookup"><span data-stu-id="785ee-121">By providing information on the existing and desired sensitivity label, the REST API can intelligently inform your application of the [actions](/graph/api/resources/informationprotectionaction?view=graph-rest-beta) that should be taken to correctly apply the label.</span></span> <span data-ttu-id="785ee-122">这包括[元数据](/graph/api/resources/metadataaction?view=graph-rest-beta)应用程序、[水印](/graph/api/resources/addwatermarkaction?view=graph-rest-beta)生成、[保护](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta)等操作。</span><span class="sxs-lookup"><span data-stu-id="785ee-122">This includes actions such as [metadata](/graph/api/resources/metadataaction?view=graph-rest-beta) application, [watermark](/graph/api/resources/addwatermarkaction?view=graph-rest-beta) generation, [protection](/graph/api/resources/protectbytemplateaction?view=graph-rest-beta), and more.</span></span>

### <a name="interpret-labels-applied-to-data"></a><span data-ttu-id="785ee-123">解释应用于数据的标签</span><span class="sxs-lookup"><span data-stu-id="785ee-123">Interpret labels applied to data</span></span>

<span data-ttu-id="785ee-124">如果应用程序使用已应用了[敏感性标签元数据](/graph/api/resources/metadataaction?view=graph-rest-beta)的信息，则可以使用**extractLabel** API 将标签元数据解析为 Microsoft 信息保护[灵敏度标签](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="785ee-124">Applications consuming information that already has [sensitivity label metadata](/graph/api/resources/metadataaction?view=graph-rest-beta) applied can use the **extractLabel** API to resolve label metadata to a Microsoft Information Protection [sensitivity label](/graph/api/resources/informationprotectionlabel.md?view=graph-rest-beta).</span></span> <span data-ttu-id="785ee-125">使用标签标识在处理或使用标记的数据时应由应用程序执行的操作。</span><span class="sxs-lookup"><span data-stu-id="785ee-125">Use the label to identify the actions that should be taken by the application when handling or consuming the labeled data.</span></span> 

## <a name="api-reference"></a><span data-ttu-id="785ee-126">API 参考</span><span class="sxs-lookup"><span data-stu-id="785ee-126">API reference</span></span>

<span data-ttu-id="785ee-127">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="785ee-127">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="785ee-128">Microsoft Graph beta 中的 microsoft 信息保护 API</span><span class="sxs-lookup"><span data-stu-id="785ee-128">Microsoft Information Protection API in Microsoft Graph beta</span></span>](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="785ee-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="785ee-129">Next steps</span></span>

- <span data-ttu-id="785ee-130">选择并尝试在[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中标记示例查询的信息保护。</span><span class="sxs-lookup"><span data-stu-id="785ee-130">Select and try Information Protection labeling sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="785ee-131">选择左侧列中的“显示更多示例”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="785ee-131">Choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="785ee-132">使用菜单打开 " **Microsoft 信息保护**"。</span><span class="sxs-lookup"><span data-stu-id="785ee-132">Use the menu to turn on **Microsoft Information Protection**.</span></span>
