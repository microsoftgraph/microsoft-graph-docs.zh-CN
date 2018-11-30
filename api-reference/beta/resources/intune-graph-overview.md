---
title: 使用 Intune Graph API
description: " 不支持 Intune 混合部署。 "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046317"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="00bb5-103">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="00bb5-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="00bb5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00bb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00bb5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00bb5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00bb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="00bb5-107">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="00bb5-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="00bb5-108">对于移动设备管理 (MDM) 场景，适用于 Intune 的 Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="00bb5-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="00bb5-109">使用 Intune Graph API</span><span class="sxs-lookup"><span data-stu-id="00bb5-109">Using the Intune Graph API</span></span>

<span data-ttu-id="00bb5-110">Intune 提供数据到 Microsoft Graph 相同的方式其他云服务一样，具有丰富的实体信息的关系，以及导航。</span><span class="sxs-lookup"><span data-stu-id="00bb5-110">Intune provides data into the Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="00bb5-111">使用 Microsoft Graph 来合并来自其他服务和 Intune IT 专业人员或最终用户构建丰富跨服务应用程序的信息。</span><span class="sxs-lookup"><span data-stu-id="00bb5-111">  Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="00bb5-112">以下是如何能够确定是否在用户的设备上安装了应用程序的方法示例：</span><span class="sxs-lookup"><span data-stu-id="00bb5-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="00bb5-113">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="00bb5-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="00bb5-114">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="00bb5-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="00bb5-115">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="00bb5-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a><span data-ttu-id="00bb5-116">使用图权限范围</span><span class="sxs-lookup"><span data-stu-id="00bb5-116">Using Graph permission scopes</span></span>

<span data-ttu-id="00bb5-117">Microsof 图控制使用权限作用域的资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="00bb5-117">Microsof Graph controls access to resources using permission scopes.</span></span> <span data-ttu-id="00bb5-118">作为开发者，你必须指定访问 Intune 资源需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="00bb5-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="00bb5-119">通常情况下，可以在 Azure Active Directory 门户中指定需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="00bb5-119">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="00bb5-120">有关详细信息，请参阅 [Microsoft Graph 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)和 [Intune 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)。</span><span class="sxs-lookup"><span data-stu-id="00bb5-120">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a><span data-ttu-id="00bb5-121">若要使用 Microsoft Graph 网站上的目录</span><span class="sxs-lookup"><span data-stu-id="00bb5-121">To use the Table of Contents on the Microsoft Graph site</span></span>
  
<span data-ttu-id="00bb5-122">可以浏览目录 （在网站的左窗格中） 以查找您想要查看的 Intune 图形 API 和资源文档的部分。</span><span class="sxs-lookup"><span data-stu-id="00bb5-122">You can browse the Table of Contents (in the left pane of the site) to find the parts of the Intune Graph API and resource documentation you want to see.</span></span>

1. <span data-ttu-id="00bb5-123">单击 **/Beta 引用**以打开 beta 文档。</span><span class="sxs-lookup"><span data-stu-id="00bb5-123">Click **/Beta Reference** to open the beta docs.</span></span>
2. <span data-ttu-id="00bb5-124">向下滚动并单击**Intune**。</span><span class="sxs-lookup"><span data-stu-id="00bb5-124">Scroll down and click **Intune**.</span></span>
3. <span data-ttu-id="00bb5-125">继续单击下方**Intune**的小节的 API 的部件您</span><span class="sxs-lookup"><span data-stu-id="00bb5-125">Continue to click subsections below **Intune** for the parts of the API you</span></span> 
