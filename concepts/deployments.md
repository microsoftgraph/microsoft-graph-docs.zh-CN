# <a name="national-cloud-deployments"></a><span data-ttu-id="66e19-101">区域云部署</span><span class="sxs-lookup"><span data-stu-id="66e19-101">National cloud deployments</span></span>


<span data-ttu-id="66e19-p101">Microsoft 云服务可用于三个独立的区域云。这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。若要了解详细信息，请参阅[Microsoft 区域云](https://www.microsoft.com/en-us/TrustCenter/CloudServices/NationalCloud)。</span><span class="sxs-lookup"><span data-stu-id="66e19-p101">Microsoft cloud services are available in three separate national clouds. These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel. To learn more, see [Microsoft National Clouds](https://www.microsoft.com/en-us/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="66e19-105">当前区域云包括：</span><span class="sxs-lookup"><span data-stu-id="66e19-105">Current national clouds include:</span></span>

- <span data-ttu-id="66e19-106">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="66e19-106">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="66e19-107">Microsoft 云德国</span><span class="sxs-lookup"><span data-stu-id="66e19-107">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="66e19-108">由中国的世纪互联运营的 Azure 和 Office 365</span><span class="sxs-lookup"><span data-stu-id="66e19-108">Submit apps for Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="66e19-109">本文提供了有关 Microsoft Graph 的不同区域云部署及每个部署内可供开发人员使用的功能信息。</span><span class="sxs-lookup"><span data-stu-id="66e19-109">This article provides information about the different sovereign cloud instances of Microsoft Graph and the capabilities that are available to developers.</span></span> 

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="66e19-110">Microsoft Graph 和 Microsoft Graph 浏览器服务根终结点</span><span class="sxs-lookup"><span data-stu-id="66e19-110">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="66e19-111">下表显示了每个区域云的 Microsoft Graph 和 Microsoft Graph 浏览器的服务根终结点。</span><span class="sxs-lookup"><span data-stu-id="66e19-111">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span> 

| <span data-ttu-id="66e19-112">区域云</span><span class="sxs-lookup"><span data-stu-id="66e19-112">National Cloud</span></span> | <span data-ttu-id="66e19-113">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="66e19-113">Microsoft Graph</span></span> | <span data-ttu-id="66e19-114">Microsoft Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="66e19-114">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="66e19-115">由世纪互联运营的 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="66e19-115">Microsoft Graph operated by 21Vianet</span></span> | <span data-ttu-id="66e19-116">https://microsoftgraph.chinacloudapi.cn</span><span class="sxs-lookup"><span data-stu-id="66e19-116">https://microsoftgraph.chinacloudapi.cn</span></span> | <span data-ttu-id="66e19-117">https://developer.microsoft.com/zh-cn/graph/graph-explorer-china</span><span class="sxs-lookup"><span data-stu-id="66e19-117">https://developer.microsoft.com/zh-cn/graph/graph-explorer-china</span></span> |
| <span data-ttu-id="66e19-118">Microsoft Graph 德国</span><span class="sxs-lookup"><span data-stu-id="66e19-118">Microsoft Graph Germany</span></span> | <span data-ttu-id="66e19-119">https://graph.microsoft.de</span><span class="sxs-lookup"><span data-stu-id="66e19-119">https://graph.microsoft.de</span></span> | <span data-ttu-id="66e19-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="66e19-120">Not supported.</span></span> |
| <span data-ttu-id="66e19-121">Microsoft Graph for US Government</span><span class="sxs-lookup"><span data-stu-id="66e19-121">Microsoft Graph for US Government</span></span> | <span data-ttu-id="66e19-122">https://graph.microsoft.com</span><span class="sxs-lookup"><span data-stu-id="66e19-122">https://graph.microsoft.com</span></span> | <span data-ttu-id="66e19-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="66e19-123">Not supported.</span></span> |
| <span data-ttu-id="66e19-124">Microsoft Graph 全局服务</span><span class="sxs-lookup"><span data-stu-id="66e19-124">Microsoft Graph global service</span></span> | <span data-ttu-id="66e19-125">https://graph.microsoft.com</span><span class="sxs-lookup"><span data-stu-id="66e19-125">https://graph.microsoft.com</span></span> | <span data-ttu-id="66e19-126">https://developer.microsoft.com/graph/graph-explorer</span><span class="sxs-lookup"><span data-stu-id="66e19-126">https://developer.microsoft.com/graph/graph-explorer</span></span> |

> <span data-ttu-id="66e19-p102">**注意**：应用只能通过区域云终结点访问组织数据。这意味着仅能访问在特定区域云中注册的租户内的数据。尝试通过 Microsoft Graph 访问与个人 Microsoft 帐户关联的使用者数据的应用应使用全局服务 (https://graph.microsoft.com)。为区域云部署获取的访问令牌不可与为全局服务获取的访问令牌互换。</span><span class="sxs-lookup"><span data-stu-id="66e19-p102">**Note**: Apps can only access organizational data through the national cloud endpoints. This means that only data in tenants registered in the specific national cloud can be accessed. Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com). Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="66e19-131">Azure AD OpenID Connect 和 OAuth2.0 终结点</span><span class="sxs-lookup"><span data-stu-id="66e19-131">Azure OpenID Connect and OAuth2.0</span></span>

<span data-ttu-id="66e19-132">下表列出了用于为每个区域云获取令牌以调用 Microsoft Graph 的 Azure Active Directory (Azure AD) 终结点的基本 URL。</span><span class="sxs-lookup"><span data-stu-id="66e19-132">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span> 

| <span data-ttu-id="66e19-133">区域云</span><span class="sxs-lookup"><span data-stu-id="66e19-133">National Cloud</span></span> | <span data-ttu-id="66e19-134">Azure AD 根终结点</span><span class="sxs-lookup"><span data-stu-id="66e19-134">Azure AD endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="66e19-135">由世纪互联运营的 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="66e19-135">Microsoft Graph operated by 21Vianet</span></span> |<span data-ttu-id="66e19-136">https://login.chinacloudapi.cn</span><span class="sxs-lookup"><span data-stu-id="66e19-136">https://login.chinacloudapi.cn</span></span> | 
| <span data-ttu-id="66e19-137">Microsoft Graph 德国</span><span class="sxs-lookup"><span data-stu-id="66e19-137">Microsoft Graph Germany</span></span> | <span data-ttu-id="66e19-138">https://login.microsoftonline.de</span><span class="sxs-lookup"><span data-stu-id="66e19-138">https://login.microsoftonline.de</span></span> | 
| <span data-ttu-id="66e19-139">Microsoft Graph for US Government</span><span class="sxs-lookup"><span data-stu-id="66e19-139">Microsoft Graph for US Government</span></span> | <span data-ttu-id="66e19-140">https://login-us.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="66e19-140">https://login-us.microsoftonline.com</span></span> | 
| <span data-ttu-id="66e19-141">Microsoft Graph（全局服务）</span><span class="sxs-lookup"><span data-stu-id="66e19-141">Microsoft Graph (global service)</span></span> | <span data-ttu-id="66e19-142">https://login.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="66e19-142">https://login.microsoftonline.com</span></span> | 

<span data-ttu-id="66e19-p103">可以使用相应的区域特定的基本 URL 来生成对 Azure AD 授权或令牌终结点的请求。例如，对于德国来说：</span><span class="sxs-lookup"><span data-stu-id="66e19-p103">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="66e19-145">授权常用终结点是 https://login.microsoftonline.de/common/oauth2/authorize。</span><span class="sxs-lookup"><span data-stu-id="66e19-145">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="66e19-146">令牌常用终结点是 https://login.microsoftonline.de/common/oauth2/authorize。</span><span class="sxs-lookup"><span data-stu-id="66e19-146">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="66e19-p104">可以通过使用租户 ID 或租户的验证域替换上述 URL 中的“common”来生成租户特定的终结点。是使用常用终结点还是租户特定的终结点将取决于应用的要求和用于获取令牌的身份验证流。要了解有关 Azure AD 访问令牌和 Microsoft Graph 的详细信息，请参阅[获取身份验证令牌](./auth_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="66e19-p104">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth_overview.md).</span></span>

> <span data-ttu-id="66e19-150">**注意：**[Azure AD v2.0 授权和令牌终结点](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/)仅在全局服务中可用；它们尚不支持用于区域云部署。</span><span class="sxs-lookup"><span data-stu-id="66e19-150">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/en-us/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span> 

## <a name="supported-features"></a><span data-ttu-id="66e19-151">支持的功能</span><span class="sxs-lookup"><span data-stu-id="66e19-151">Supported API features</span></span>

<span data-ttu-id="66e19-152">除非另有说明，否则以下 Microsoft Graph 功能通常在所有区域云部署中（在 `/v1.0` 终结点上）可用：</span><span class="sxs-lookup"><span data-stu-id="66e19-152">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="66e19-153">用户</span><span class="sxs-lookup"><span data-stu-id="66e19-153">Users</span></span>
* <span data-ttu-id="66e19-154">组</span><span class="sxs-lookup"><span data-stu-id="66e19-154">Groups</span></span>
* <span data-ttu-id="66e19-155">Excel（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="66e19-155">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="66e19-156">OneDrive（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="66e19-156">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="66e19-157">Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="66e19-157">Outlook mail</span></span>
* <span data-ttu-id="66e19-158">Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="66e19-158">Outlook Calendar</span></span>
* <span data-ttu-id="66e19-159">个人联系人</span><span class="sxs-lookup"><span data-stu-id="66e19-159">Personal Contacts</span></span> 
* <span data-ttu-id="66e19-160">SharePoint（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="66e19-160">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="66e19-161">Delta 查询（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="66e19-161">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="66e19-162">Webhook（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="66e19-162">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="66e19-163">除非另有说明，否则以下其他 Microsoft Graph 功能在所有区域云部署中（在 `/beta` 终结点上）可用于预览：</span><span class="sxs-lookup"><span data-stu-id="66e19-163">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="66e19-164">组织联系人</span><span class="sxs-lookup"><span data-stu-id="66e19-164">Organizational Contacts</span></span>
* <span data-ttu-id="66e19-165">应用程序</span><span class="sxs-lookup"><span data-stu-id="66e19-165">Applications</span></span>
* <span data-ttu-id="66e19-166">服务主体</span><span class="sxs-lookup"><span data-stu-id="66e19-166">Service Principals</span></span>

<span data-ttu-id="66e19-167">区域云部署尚不支持以下 Microsoft Graph 功能：</span><span class="sxs-lookup"><span data-stu-id="66e19-167">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="66e19-168">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="66e19-168">Microsoft Planner</span></span>
* <span data-ttu-id="66e19-169">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="66e19-169">Directory schema extensions</span></span>
* <span data-ttu-id="66e19-170">开放类型扩展</span><span class="sxs-lookup"><span data-stu-id="66e19-170">Open type extensions</span></span>
