---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
author: dougeby
localization_priority: Priority
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: baad1c809bfd34dd60bab009b7b83c5fcb46dddf
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732400"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="cadeb-103">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="cadeb-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="cadeb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cadeb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="cadeb-105">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户** 执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="cadeb-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="cadeb-106">就移动设备管理 (MDM) 应用场景而言，适用于 Intune 的 Microsoft Graph API 支持独立部署；不支持 Intune [混合部署](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="cadeb-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="cadeb-107">使用适用于 Intune 的 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="cadeb-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="cadeb-108">Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。</span><span class="sxs-lookup"><span data-stu-id="cadeb-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span> <span data-ttu-id="cadeb-109">使用 Microsoft Graph API 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。</span><span class="sxs-lookup"><span data-stu-id="cadeb-109">Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="cadeb-110">以下示例说明如何能够确定是否在用户的设备上安装了应用程序：</span><span class="sxs-lookup"><span data-stu-id="cadeb-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="cadeb-111">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="cadeb-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="cadeb-112">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="cadeb-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="cadeb-113">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="cadeb-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="cadeb-114">访问适用于 Intune 的 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="cadeb-114">Accessing the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="cadeb-115">Intune 同时支持[委托的权限](/graph/auth-v2-user)和[应用程序权限](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="cadeb-115">Intune supports both [delegated permissions](/graph/auth-v2-user) and [application permissions](/graph/auth-v2-service).</span></span> <span data-ttu-id="cadeb-116">委托的权限和应用程序权限都支持读取和写入操作。</span><span class="sxs-lookup"><span data-stu-id="cadeb-116">Delegated and application permissions support both read and write operations.</span></span> <span data-ttu-id="cadeb-117">委托的权限和应用程序权限都支持单租户应用程序和多租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="cadeb-117">Delegated and application permissions support both single tenant applications, as well as multi-tenant applications.</span></span> <span data-ttu-id="cadeb-118">若要详细了解可通过 Microsoft Graph 获取的权限，请参阅 [ Microsoft Graph 权限参考](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cadeb-118">For more information about the permissions available through Microsoft Graph, see [Microsoft Graph permissions reference](/graph/permissions-reference).</span></span>

## <a name="using-permissions"></a><span data-ttu-id="cadeb-119">使用权限</span><span class="sxs-lookup"><span data-stu-id="cadeb-119">Using permissions</span></span>

<span data-ttu-id="cadeb-120">Microsoft Graph API 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="cadeb-120">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="cadeb-121">作为开发者，你必须指定访问 Intune 资源需要的权限。</span><span class="sxs-lookup"><span data-stu-id="cadeb-121">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="cadeb-122">通常是在 Azure Active Directory 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="cadeb-122">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="cadeb-123">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cadeb-123">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="cadeb-124">最近更新</span><span class="sxs-lookup"><span data-stu-id="cadeb-124">What's new</span></span>
<span data-ttu-id="cadeb-125">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="cadeb-125">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cadeb-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cadeb-126">Next Steps</span></span>

- <span data-ttu-id="cadeb-127">了解[如何使用 Azure AD](/intune/intune-graph-apis) 访问适用于 Intune 的 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="cadeb-127">Learn [how to use Azure AD](/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="cadeb-128">浏览 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，这些示例演示如何在工作示例上下文中使用适用于 Intune 的 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="cadeb-128">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>