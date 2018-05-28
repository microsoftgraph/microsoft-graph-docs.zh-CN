# <a name="national-cloud-deployments"></a><span data-ttu-id="6ecce-101">区域云部署</span><span class="sxs-lookup"><span data-stu-id="6ecce-101">National cloud deployments</span></span>


<span data-ttu-id="6ecce-102">除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。</span><span class="sxs-lookup"><span data-stu-id="6ecce-102">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="6ecce-103">这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。</span><span class="sxs-lookup"><span data-stu-id="6ecce-103">Microsoft cloud services are available in three separate national clouds. These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel. To learn more, see Microsoft National Clouds.</span></span> <span data-ttu-id="6ecce-104">若要了解详细信息，请参阅[Microsoft 区域云](https://www.microsoft.com/zh-CN/TrustCenter/CloudServices/NationalCloud)。</span><span class="sxs-lookup"><span data-stu-id="6ecce-104">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/zh-CN/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="6ecce-105">当前区域云包括：</span><span class="sxs-lookup"><span data-stu-id="6ecce-105">Current national clouds include:</span></span>

- <span data-ttu-id="6ecce-106">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="6ecce-106">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="6ecce-107">Microsoft 云德国</span><span class="sxs-lookup"><span data-stu-id="6ecce-107">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="6ecce-108">由中国的世纪互联运营的 Azure 和 Office 365</span><span class="sxs-lookup"><span data-stu-id="6ecce-108">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="6ecce-109">本文提供了有关 Microsoft Graph 的不同区域云部署及每个部署内可供开发人员使用的功能信息。</span><span class="sxs-lookup"><span data-stu-id="6ecce-109">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="6ecce-110">Microsoft Graph 和 Microsoft Graph 浏览器服务根终结点</span><span class="sxs-lookup"><span data-stu-id="6ecce-110">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="6ecce-111">下表显示了每个区域云的 Microsoft Graph 和 Microsoft Graph 浏览器的服务根终结点。</span><span class="sxs-lookup"><span data-stu-id="6ecce-111">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="6ecce-112">区域云</span><span class="sxs-lookup"><span data-stu-id="6ecce-112">National Cloud</span></span> | <span data-ttu-id="6ecce-113">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6ecce-113">Microsoft Graph</span></span> | <span data-ttu-id="6ecce-114">Microsoft Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="6ecce-114">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="6ecce-115">由世纪互联运营的 Microsoft Graph 中国</span><span class="sxs-lookup"><span data-stu-id="6ecce-115">Microsoft Graph operated by 21Vianet in China</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="6ecce-116">Microsoft Graph 德国</span><span class="sxs-lookup"><span data-stu-id="6ecce-116">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="6ecce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ecce-117">Not supported.</span></span> |
| <span data-ttu-id="6ecce-118">Microsoft Graph for US Government</span><span class="sxs-lookup"><span data-stu-id="6ecce-118">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="6ecce-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ecce-119">Not supported.</span></span> |
| <span data-ttu-id="6ecce-120">Microsoft Graph 全局服务</span><span class="sxs-lookup"><span data-stu-id="6ecce-120">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="6ecce-121">**注意**：应用只能通过区域云终结点访问组织数据。</span><span class="sxs-lookup"><span data-stu-id="6ecce-121">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="6ecce-122">这意味着仅能访问在特定区域云中注册的租户内的数据。</span><span class="sxs-lookup"><span data-stu-id="6ecce-122">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="6ecce-123">尝试通过 Microsoft Graph 访问与个人 Microsoft 帐户关联的使用者数据的应用应使用全局服务 (https://graph.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="6ecce-123">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="6ecce-124">为区域云部署获取的访问令牌不可与为全局服务获取的访问令牌互换。</span><span class="sxs-lookup"><span data-stu-id="6ecce-124">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="6ecce-125">Azure AD OpenID Connect 和 OAuth2.0 终结点</span><span class="sxs-lookup"><span data-stu-id="6ecce-125">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="6ecce-126">下表列出了用于为每个区域云获取令牌以调用 Microsoft Graph 的 Azure Active Directory (Azure AD) 终结点的基本 URL。</span><span class="sxs-lookup"><span data-stu-id="6ecce-126">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="6ecce-127">区域云</span><span class="sxs-lookup"><span data-stu-id="6ecce-127">National Cloud</span></span> | <span data-ttu-id="6ecce-128">Azure AD 根终结点</span><span class="sxs-lookup"><span data-stu-id="6ecce-128">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="6ecce-129">由世纪互联运营的 Azure AD 中国</span><span class="sxs-lookup"><span data-stu-id="6ecce-129">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="6ecce-130">Azure AD 德国</span><span class="sxs-lookup"><span data-stu-id="6ecce-130">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="6ecce-131">Azure AD for US Government</span><span class="sxs-lookup"><span data-stu-id="6ecce-131">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="6ecce-132">Azure AD（全局服务）</span><span class="sxs-lookup"><span data-stu-id="6ecce-132">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="6ecce-p103">可以使用相应的区域特定的基本 URL 来生成对 Azure AD 授权或令牌终结点的请求。例如，在德国：</span><span class="sxs-lookup"><span data-stu-id="6ecce-p103">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="6ecce-135">授权常见终结点是 https://login.microsoftonline.de/common/oauth2/authorize。</span><span class="sxs-lookup"><span data-stu-id="6ecce-135">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="6ecce-136">令牌常见终结点是 https://login.microsoftonline.de/common/oauth2/token。</span><span class="sxs-lookup"><span data-stu-id="6ecce-136">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="6ecce-p104">可以通过使用租户 ID 或租户的验证域替换上述 URL 中的“common”来生成租户特定的终结点。是使用常用终结点还是租户特定的终结点将取决于应用的要求和用于获取令牌的身份验证流。要了解有关 Azure AD 访问令牌和 Microsoft Graph 的详细信息，请参阅[获取身份验证令牌](./auth_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="6ecce-p104">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth_overview.md).</span></span>

> <span data-ttu-id="6ecce-140">**注意：**[Azure AD v2.0 授权和令牌终结点](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview/)仅在全局服务中可用；它们尚不支持用于区域云部署。</span><span class="sxs-lookup"><span data-stu-id="6ecce-140">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="6ecce-141">支持的功能</span><span class="sxs-lookup"><span data-stu-id="6ecce-141">Supported features</span></span>

<span data-ttu-id="6ecce-142">除非另有说明，否则以下 Microsoft Graph 功能通常在所有区域云部署中（在 `/v1.0` 终结点上）可用：</span><span class="sxs-lookup"><span data-stu-id="6ecce-142">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="6ecce-143">用户</span><span class="sxs-lookup"><span data-stu-id="6ecce-143">Users</span></span>
* <span data-ttu-id="6ecce-144">组</span><span class="sxs-lookup"><span data-stu-id="6ecce-144">Groups</span></span>
* <span data-ttu-id="6ecce-145">Excel（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="6ecce-145">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="6ecce-146">OneDrive（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="6ecce-146">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="6ecce-147">Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="6ecce-147">Outlook Mail</span></span>
* <span data-ttu-id="6ecce-148">Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="6ecce-148">Outlook Calendar</span></span>
* <span data-ttu-id="6ecce-149">个人联系人</span><span class="sxs-lookup"><span data-stu-id="6ecce-149">Personal Contacts</span></span> 
* <span data-ttu-id="6ecce-150">SharePoint（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="6ecce-150">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="6ecce-151">Delta 查询（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="6ecce-151">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="6ecce-152">Webhook（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="6ecce-152">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="6ecce-153">除非另有说明，否则以下其他 Microsoft Graph 功能在所有区域云部署中（在 `/beta` 终结点上）可用于预览：</span><span class="sxs-lookup"><span data-stu-id="6ecce-153">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="6ecce-154">组织联系人</span><span class="sxs-lookup"><span data-stu-id="6ecce-154">Organizational Contacts</span></span>
* <span data-ttu-id="6ecce-155">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ecce-155">Applications</span></span>
* <span data-ttu-id="6ecce-156">服务主体</span><span class="sxs-lookup"><span data-stu-id="6ecce-156">Service Principals</span></span>

<span data-ttu-id="6ecce-157">区域云部署尚不支持以下 Microsoft Graph 功能：</span><span class="sxs-lookup"><span data-stu-id="6ecce-157">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="6ecce-158">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="6ecce-158">Microsoft Planner</span></span>
* <span data-ttu-id="6ecce-159">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="6ecce-159">Directory schema extensions</span></span>
* <span data-ttu-id="6ecce-160">开放类型扩展</span><span class="sxs-lookup"><span data-stu-id="6ecce-160">Open type extensions</span></span>
