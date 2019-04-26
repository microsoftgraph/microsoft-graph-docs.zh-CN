---
title: 使用 Intune Graph API - Microsoft Graph API
description: 列出你可用于管理租户组织及其设备、应用、访问权限和资源的 Intune 终结点 (REST) 的 Microsoft Graph API。
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: fc254772a5b4db131a5cda45fc83b336bf12f993
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575959"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="9f85c-103">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="9f85c-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="9f85c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f85c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f85c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f85c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f85c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f85c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="9f85c-107">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="9f85c-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="9f85c-108">就移动设备管理 (MDM) 应用场景而言，适用于 Intune 的 Microsoft Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="9f85c-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="9f85c-109">使用适用于 Intune 的 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="9f85c-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="9f85c-110">Intune 向 Microsoft Graph 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。</span><span class="sxs-lookup"><span data-stu-id="9f85c-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="9f85c-111">使用 Microsoft Graph 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。</span><span class="sxs-lookup"><span data-stu-id="9f85c-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="9f85c-112">以下示例说明如何能够确定是否在用户的设备上安装了应用程序：</span><span class="sxs-lookup"><span data-stu-id="9f85c-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="9f85c-113">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="9f85c-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="9f85c-114">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="9f85c-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="9f85c-115">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="9f85c-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="9f85c-116">使用 Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="9f85c-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="9f85c-117">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="9f85c-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="9f85c-118">作为开发者，你必须指定访问 Intune 资源需要的权限。</span><span class="sxs-lookup"><span data-stu-id="9f85c-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="9f85c-119">通常是在 Azure Active Directory 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="9f85c-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="9f85c-120">有关详细信息，请参阅 [Microsoft Graph 权限参考](https://docs.microsoft.com/zh-CN/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f85c-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/zh-CN/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="9f85c-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9f85c-121">Next Steps</span></span>

- <span data-ttu-id="9f85c-122">了解[如何使用 Azure AD](https://docs.microsoft.com/zh-CN/intune/intune-graph-apis) 访问适用于 Intune 的 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="9f85c-122">Learn [how to use Azure AD](https://docs.microsoft.com/zh-CN/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="9f85c-123">浏览 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，这些示例演示如何在工作示例上下文中使用适用于 Intune 的 Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="9f85c-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

