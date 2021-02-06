---
title: 本地发布配置文件
description: 各种 Azure (例如，Azure Active Directory Connect Passthrough Authentication、Workday 到预配) 的 Azure AD 用户允许从企业网络外部对各种本地资源进行条件访问。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 44d09da274413b23092afea6290c0c32a64f8500
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134874"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="bdb85-103">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="bdb85-103">On-premises publishing profiles</span></span>

<span data-ttu-id="bdb85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdb85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdb85-105">各种 Azure (例如，Azure Active Directory Connect [Passthrough](/azure/active-directory/hybrid/how-to-connect-pta)Authentication、Workday [to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial)和应用程序 [代理](https://aka.ms/whyappproxy)  允许从企业网络外部访问各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="bdb85-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="bdb85-106">[可以将租户](onpremisesagent.md) (安装的应用程序代理或) 连接器[](connector.md)配置为将请求路由到特定的[已发布资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="bdb85-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="bdb85-107">[通过应用程序](onpremisesagentgroup.md) (代理) 代理组[](connectorgroup.md)或连接器组，租户管理员能够分配特定代理，为发布的特定本地资源提供服务。</span><span class="sxs-lookup"><span data-stu-id="bdb85-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="bdb85-108">租户管理员可以将多个代理组合在一起，然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="bdb85-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="bdb85-109">同一本地发布类型的整个实体集由 [onPremisesPublishingProfile 表示](onpremisespublishingprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="bdb85-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="bdb85-110">租户管理员可以为每个 **onPremisesPublishingProfile** 配置代理可以 [](updatewindow.md)接收更新或延迟代理更新的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="bdb85-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="bdb85-111">为 **onPremisesPublishingProfile** 指定的更新程序配置适用于该 **onPremisesPublishingProfile 内的所有代理**。 [](hybridagentupdaterconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdb85-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

<span data-ttu-id="bdb85-112">有关配置应用程序代理的教程，请参阅使用 [Microsoft Graph API 自动配置应用程序代理](/graph/application-proxy-configure-api)。</span><span class="sxs-lookup"><span data-stu-id="bdb85-112">For a tutorial about configuring Application Proxy, see [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="bdb85-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bdb85-113">See also</span></span>

- [<span data-ttu-id="bdb85-114">本地代理</span><span class="sxs-lookup"><span data-stu-id="bdb85-114">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="bdb85-115">本地代理组</span><span class="sxs-lookup"><span data-stu-id="bdb85-115">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="bdb85-116">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="bdb85-116">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="bdb85-117">已发布资源</span><span class="sxs-lookup"><span data-stu-id="bdb85-117">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="bdb85-118">Connector</span><span class="sxs-lookup"><span data-stu-id="bdb85-118">Connector</span></span>](connector.md)
- [<span data-ttu-id="bdb85-119">连接器组</span><span class="sxs-lookup"><span data-stu-id="bdb85-119">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



