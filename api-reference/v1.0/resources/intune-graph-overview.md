---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
author: tfitzmac
localization_priority: Priority
ms.openlocfilehash: 1222f064b075c8884f5c66c101ae0e15256221c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830679"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="b9620-103">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="b9620-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="b9620-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9620-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b9620-105">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="b9620-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="b9620-106">为移动设备管理 (MDM) 方案，Intune Microsoft Graph API 支持独立部署;不支持 Intune[混合部署](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="b9620-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="b9620-107">使用 Intune Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="b9620-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="b9620-108">Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。</span><span class="sxs-lookup"><span data-stu-id="b9620-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="b9620-109">使用 Microsoft Graph API 来合并来自其他服务和 Intune IT 专业人员或最终用户构建丰富跨服务应用程序的信息。</span><span class="sxs-lookup"><span data-stu-id="b9620-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="b9620-110">下面的示例演示如何确定用户的设备上是否安装了应用程序：</span><span class="sxs-lookup"><span data-stu-id="b9620-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="b9620-111">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="b9620-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="b9620-112">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="b9620-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="b9620-113">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="b9620-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="b9620-114">使用权限</span><span class="sxs-lookup"><span data-stu-id="b9620-114">Using permissions</span></span>

<span data-ttu-id="b9620-115">Microsoft Graph API 控制通过权限的资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b9620-115">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="b9620-116">作为开发人员，您必须指定需要访问 Intune 资源的权限。</span><span class="sxs-lookup"><span data-stu-id="b9620-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="b9620-117">通常情况下，您将在 Azure Active Directory 门户中指定的权限。</span><span class="sxs-lookup"><span data-stu-id="b9620-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="b9620-118">有关详细信息，请参阅[Microsoft Graph 权限参考](https://docs.microsoft.com/en-us/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9620-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9620-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b9620-119">Next Steps</span></span>

- <span data-ttu-id="b9620-120">了解[如何使用 Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis)以访问 Intune Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="b9620-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="b9620-121">浏览这些[PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，其中显示如何使用示例上下文中使用 Intune Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="b9620-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
