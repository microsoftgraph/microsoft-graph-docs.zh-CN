# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="8f19f-101">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="8f19f-101">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="8f19f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f19f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8f19f-103">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="8f19f-103">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="8f19f-104">对于移动设备管理 (MDM) 场景，适用于 Intune 的 Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="8f19f-104">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="8f19f-105">使用 Intune Graph API</span><span class="sxs-lookup"><span data-stu-id="8f19f-105">Using the Intune Graph API</span></span>

<span data-ttu-id="8f19f-106">Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。</span><span class="sxs-lookup"><span data-stu-id="8f19f-106">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="8f19f-107">使用 Microsoft Graph API 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。</span><span class="sxs-lookup"><span data-stu-id="8f19f-107">  Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="8f19f-108">以下是如何能够确定是否在用户的设备上安装了应用程序的方法示例：</span><span class="sxs-lookup"><span data-stu-id="8f19f-108">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="8f19f-109">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="8f19f-109">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="8f19f-110">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="8f19f-110">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="8f19f-111">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="8f19f-111">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a><span data-ttu-id="8f19f-112">使用权限范围</span><span class="sxs-lookup"><span data-stu-id="8f19f-112">Using permission scopes</span></span>

<span data-ttu-id="8f19f-113">Microsoft Graph API 可以使用权限范围控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="8f19f-113">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="8f19f-114">作为开发者，你必须指定访问 Intune 资源需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="8f19f-114">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="8f19f-115">通常情况下，可以在 Azure Active Directory 门户中指定需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="8f19f-115">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="8f19f-116">有关详细信息，请参阅 [Microsoft Graph 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)和 [Intune 权限范围](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)。</span><span class="sxs-lookup"><span data-stu-id="8f19f-116">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8f19f-117">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8f19f-117">Next Steps</span></span>

- <span data-ttu-id="8f19f-118">了解[如何使用 Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis)以访问 Intune Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="8f19f-118">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="8f19f-119">浏览这些[PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)，其中显示如何为 Intune 工作示例上下文中使用图形 API。</span><span class="sxs-lookup"><span data-stu-id="8f19f-119">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use Graph API for Intune in context of working examples.</span></span>