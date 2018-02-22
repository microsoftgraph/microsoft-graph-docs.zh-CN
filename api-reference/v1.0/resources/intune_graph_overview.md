# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="31373-101">在 Microsoft Graph 中使用 Intune</span><span class="sxs-lookup"><span data-stu-id="31373-101">Working with files in Microsoft Graph</span></span>  

> <span data-ttu-id="31373-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31373-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="31373-103">适用于 Intune 的 Microsoft Graph API 允许以编程方式访问租户的 Intune 信息；API 会执行与可通过 **Azure 门户**执行的相同 Intune 操作。</span><span class="sxs-lookup"><span data-stu-id="31373-103">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="31373-104">对于移动设备管理 (MDM) 场景，适用于 Intune 的 Graph API 支持独立部署；不支持 Intune [混合部署](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)。</span><span class="sxs-lookup"><span data-stu-id="31373-104">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/zh-CN/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="31373-105">使用 Intune Graph API</span><span class="sxs-lookup"><span data-stu-id="31373-105">Using the Intune Graph API</span></span>

<span data-ttu-id="31373-106">Intune 向 Microsoft Graph API 提供数据的方式与其他云服务相同，具有丰富的实体信息和关系导航。</span><span class="sxs-lookup"><span data-stu-id="31373-106">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span>  <span data-ttu-id="31373-107">使用 Microsoft Graph API 将来自其他服务和 Intune 的信息进行组合，为 IT 专业人员和最终用户构建丰富的跨服务应用程序。</span><span class="sxs-lookup"><span data-stu-id="31373-107">Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="31373-108">以下是如何能够确定是否在用户的设备上安装了应用程序的方法示例：</span><span class="sxs-lookup"><span data-stu-id="31373-108">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="31373-109">从 Azure Active Directory 获取注册到用户的设备列表：</span><span class="sxs-lookup"><span data-stu-id="31373-109">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    <span data-ttu-id="31373-110">https://graph.microsoft.com/users/{user}/ownedDevices</span><span class="sxs-lookup"><span data-stu-id="31373-110">https://graph.microsoft.com</span></span> 

2. <span data-ttu-id="31373-111">然后，查看租户的应用程序列表：</span><span class="sxs-lookup"><span data-stu-id="31373-111">Then view the list of applications for your tenant:</span></span> 

    <span data-ttu-id="31373-112">https://graph.microsoft.com/deviceAppManagement/mobileApps</span><span class="sxs-lookup"><span data-stu-id="31373-112">https://graph.microsoft.com</span></span>  

3. <span data-ttu-id="31373-113">从应用程序中获取 ID，并确定应用程序（以及用户）的安装状态：</span><span class="sxs-lookup"><span data-stu-id="31373-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    <span data-ttu-id="31373-114">https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/</span><span class="sxs-lookup"><span data-stu-id="31373-114">https://graph.microsoft.com</span></span>


## <a name="using-permission-scopes"></a><span data-ttu-id="31373-115">使用权限范围</span><span class="sxs-lookup"><span data-stu-id="31373-115">Using permission scopes</span></span>

<span data-ttu-id="31373-116">Microsoft Graph API 可以使用权限范围控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="31373-116">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="31373-117">作为开发者，你必须指定访问 Intune 资源需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="31373-117">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="31373-118">通常情况下，可以在 Azure Active Directory 门户中指定需要的权限范围。</span><span class="sxs-lookup"><span data-stu-id="31373-118">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="31373-119">有关详细信息，请参阅 [Microsoft Graph 权限范围](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes)和 [Intune 权限范围](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)。</span><span class="sxs-lookup"><span data-stu-id="31373-119">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/zh-CN/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

