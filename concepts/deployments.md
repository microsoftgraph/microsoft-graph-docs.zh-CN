---
title: 区域云部署
description: 除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。 这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。 若要了解详细信息，请参阅“Microsoft 区域云”。
ms.openlocfilehash: b0f2ab257773faa14fe59566992bb1ed0dd77959
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091754"
---
# <a name="national-cloud-deployments"></a><span data-ttu-id="2a9b6-105">区域云部署</span><span class="sxs-lookup"><span data-stu-id="2a9b6-105">National cloud deployments</span></span>


<span data-ttu-id="2a9b6-106">除了全球的数据中心网络外，Microsoft 云服务还可用于三个独立的区域云。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-106">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="2a9b6-107">这些区域云版本是 Microsoft 企业云服务的物理和逻辑网络隔离实例，它们仅限于特定国家/地区的地理边界内，由当地人员运营。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-107">These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel.</span></span> <span data-ttu-id="2a9b6-108">若要了解详细信息，请参阅[Microsoft 区域云](https://www.microsoft.com/zh-CN/TrustCenter/CloudServices/NationalCloud)。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-108">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/zh-CN/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="2a9b6-109">当前区域云包括：</span><span class="sxs-lookup"><span data-stu-id="2a9b6-109">Current national clouds include:</span></span>

- <span data-ttu-id="2a9b6-110">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="2a9b6-110">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="2a9b6-111">Microsoft 云德国</span><span class="sxs-lookup"><span data-stu-id="2a9b6-111">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="2a9b6-112">由中国的世纪互联运营的 Azure 和 Office 365</span><span class="sxs-lookup"><span data-stu-id="2a9b6-112">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="2a9b6-113">本文提供了有关 Microsoft Graph 的不同区域云部署及每个部署内可供开发人员使用的功能信息。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-113">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="2a9b6-114">Microsoft Graph 和 Microsoft Graph 浏览器服务根终结点</span><span class="sxs-lookup"><span data-stu-id="2a9b6-114">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="2a9b6-115">下表显示了每个区域云的 Microsoft Graph 和 Microsoft Graph 浏览器的服务根终结点。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-115">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="2a9b6-116">区域云</span><span class="sxs-lookup"><span data-stu-id="2a9b6-116">National Cloud</span></span> | <span data-ttu-id="2a9b6-117">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2a9b6-117">Microsoft Graph</span></span> | <span data-ttu-id="2a9b6-118">Microsoft Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="2a9b6-118">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="2a9b6-119">由世纪互联运营的 Microsoft Graph 中国</span><span class="sxs-lookup"><span data-stu-id="2a9b6-119">Microsoft Graph China operated by 21Vianet</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="2a9b6-120">Microsoft Graph 德国</span><span class="sxs-lookup"><span data-stu-id="2a9b6-120">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="2a9b6-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-121">Not supported.</span></span> |
| <span data-ttu-id="2a9b6-122">Microsoft Graph for US Government</span><span class="sxs-lookup"><span data-stu-id="2a9b6-122">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="2a9b6-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-123">Not supported.</span></span> |
| <span data-ttu-id="2a9b6-124">Microsoft Graph 全局服务</span><span class="sxs-lookup"><span data-stu-id="2a9b6-124">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="2a9b6-125">**注意**：应用只能通过区域云终结点访问组织数据。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-125">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="2a9b6-126">这意味着仅能访问在特定区域云中注册的租户内的数据。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-126">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="2a9b6-127">尝试通过 Microsoft Graph 访问与个人 Microsoft 帐户关联的使用者数据的应用应使用全局服务 (https://graph.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-127">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="2a9b6-128">为区域云部署获取的访问令牌不可与为全局服务获取的访问令牌互换。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-128">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="2a9b6-129">Azure AD OpenID Connect 和 OAuth2.0 终结点</span><span class="sxs-lookup"><span data-stu-id="2a9b6-129">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="2a9b6-130">下表列出了用于为每个区域云获取令牌以调用 Microsoft Graph 的 Azure Active Directory (Azure AD) 终结点的基本 URL。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-130">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="2a9b6-131">区域云</span><span class="sxs-lookup"><span data-stu-id="2a9b6-131">National Cloud</span></span> | <span data-ttu-id="2a9b6-132">Azure AD 根终结点</span><span class="sxs-lookup"><span data-stu-id="2a9b6-132">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="2a9b6-133">由世纪互联运营的 Azure AD 中国</span><span class="sxs-lookup"><span data-stu-id="2a9b6-133">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="2a9b6-134">Azure AD 德国</span><span class="sxs-lookup"><span data-stu-id="2a9b6-134">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="2a9b6-135">Azure AD for US Government</span><span class="sxs-lookup"><span data-stu-id="2a9b6-135">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="2a9b6-136">Azure AD（全局服务）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-136">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="2a9b6-p104">可以使用相应的区域特定的基本 URL 来生成对 Azure AD 授权或令牌终结点的请求。例如，在德国：</span><span class="sxs-lookup"><span data-stu-id="2a9b6-p104">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="2a9b6-139">授权常见终结点是 https://login.microsoftonline.de/common/oauth2/authorize。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-139">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="2a9b6-140">令牌常见终结点是 https://login.microsoftonline.de/common/oauth2/token。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-140">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="2a9b6-p105">可以通过使用租户 ID 或租户的验证域替换上述 URL 中的“common”来生成租户特定的终结点。是使用常用终结点还是租户特定的终结点将取决于应用的要求和用于获取令牌的身份验证流。要了解有关 Azure AD 访问令牌和 Microsoft Graph 的详细信息，请参阅[获取身份验证令牌](./auth-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-p105">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth-overview.md).</span></span>

> <span data-ttu-id="2a9b6-144">**注意：**[Azure AD v2.0 授权和令牌终结点](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview/)仅在全局服务中可用；它们尚不支持用于区域云部署。</span><span class="sxs-lookup"><span data-stu-id="2a9b6-144">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="2a9b6-145">支持的功能</span><span class="sxs-lookup"><span data-stu-id="2a9b6-145">Supported features</span></span>

<span data-ttu-id="2a9b6-146">除非另有说明，否则以下 Microsoft Graph 功能通常在所有区域云部署中（在 `/v1.0` 终结点上）可用：</span><span class="sxs-lookup"><span data-stu-id="2a9b6-146">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="2a9b6-147">用户</span><span class="sxs-lookup"><span data-stu-id="2a9b6-147">Users</span></span>
* <span data-ttu-id="2a9b6-148">组</span><span class="sxs-lookup"><span data-stu-id="2a9b6-148">Groups</span></span>
* <span data-ttu-id="2a9b6-149">Excel（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-149">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="2a9b6-150">OneDrive（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-150">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="2a9b6-151">Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="2a9b6-151">Outlook Mail</span></span>
* <span data-ttu-id="2a9b6-152">Outlook 日历</span><span class="sxs-lookup"><span data-stu-id="2a9b6-152">Outlook Calendar</span></span>
* <span data-ttu-id="2a9b6-153">个人联系人</span><span class="sxs-lookup"><span data-stu-id="2a9b6-153">Personal Contacts</span></span> 
* <span data-ttu-id="2a9b6-154">SharePoint（在由中国世纪互联运营的 Microsoft Graph 上支持的功能受限。）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-154">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="2a9b6-155">Delta 查询（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-155">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="2a9b6-156">Webhook（对每个区域云部署上的不同资源的支持各不相同。）</span><span class="sxs-lookup"><span data-stu-id="2a9b6-156">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="2a9b6-157">除非另有说明，否则以下其他 Microsoft Graph 功能在所有区域云部署中（在 `/beta` 终结点上）可用于预览：</span><span class="sxs-lookup"><span data-stu-id="2a9b6-157">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="2a9b6-158">组织联系人</span><span class="sxs-lookup"><span data-stu-id="2a9b6-158">Organizational Contacts</span></span>
* <span data-ttu-id="2a9b6-159">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a9b6-159">Applications</span></span>
* <span data-ttu-id="2a9b6-160">服务主体</span><span class="sxs-lookup"><span data-stu-id="2a9b6-160">Service Principals</span></span>

<span data-ttu-id="2a9b6-161">区域云部署尚不支持以下 Microsoft Graph 功能：</span><span class="sxs-lookup"><span data-stu-id="2a9b6-161">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="2a9b6-162">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="2a9b6-162">Microsoft Planner</span></span>
* <span data-ttu-id="2a9b6-163">目录架构扩展</span><span class="sxs-lookup"><span data-stu-id="2a9b6-163">Directory schema extensions</span></span>
* <span data-ttu-id="2a9b6-164">开放类型扩展</span><span class="sxs-lookup"><span data-stu-id="2a9b6-164">Open type extensions</span></span>
