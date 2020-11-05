---
title: 本地发布配置文件
description: 各种 Azure 服务 (例如，Azure Active Directory Connect to Authentication，Workday 到 Azure AD 用户预配) 允许从公司网络外部对各种本地资源进行条件访问。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26395d5ac6f4afed11d2a53a3f37c7d5b7cfa9bd
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921520"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="999f7-103">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="999f7-103">On-premises publishing profiles</span></span>

<span data-ttu-id="999f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="999f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999f7-105">各种 Azure 服务 (例如，Azure Active Directory Connect [直通身份验证](/azure/active-directory/hybrid/how-to-connect-pta)、从 [WORKDAY 到 azure AD 用户设置](/azure/active-directory/saas-apps/workday-inbound-tutorial)以及 [应用程序代理](https://aka.ms/whyappproxy)  允许从公司网络外部访问各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="999f7-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="999f7-106">可将由租户管理员安装的应用程序代理) 的[本地代理](onpremisesagent.md) (或[连接器](connector.md)配置为将请求路由到特定的[已发布资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="999f7-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="999f7-107">[代理组](onpremisesagentgroup.md) (或 [连接器组](connectorgroup.md) 应用程序代理) 使租户管理员能够分配特定代理来满足特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="999f7-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="999f7-108">租户管理员可以将许多代理组合在一起，然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="999f7-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="999f7-109">同一本地发布类型的整个实体集由 [onPremisesPublishingProfile](onpremisespublishingprofile.md)表示。</span><span class="sxs-lookup"><span data-stu-id="999f7-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="999f7-110">租户管理员可以为每个 **onPremisesPublishingProfile** 配置一个 [时间](updatewindow.md) 段，在此时段内，代理可以接收更新或将更新推迟到代理。</span><span class="sxs-lookup"><span data-stu-id="999f7-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="999f7-111">为 **onPremisesPublishingProfile** 指定的 [更新配置](hybridagentupdaterconfiguration.md)适用于该 **onPremisesPublishingProfile** 中的所有代理。</span><span class="sxs-lookup"><span data-stu-id="999f7-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

<span data-ttu-id="999f7-112">有关配置应用程序代理的教程，请参阅 [使用 Microsoft GRAPH API 自动化应用程序代理的配置](/graph/application-proxy-configure-api)。</span><span class="sxs-lookup"><span data-stu-id="999f7-112">For a tutorial about configuring Application Proxy, see [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="999f7-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="999f7-113">See also</span></span>

- [<span data-ttu-id="999f7-114">内部部署代理</span><span class="sxs-lookup"><span data-stu-id="999f7-114">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="999f7-115">内部部署代理组</span><span class="sxs-lookup"><span data-stu-id="999f7-115">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="999f7-116">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="999f7-116">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="999f7-117">已发布资源</span><span class="sxs-lookup"><span data-stu-id="999f7-117">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="999f7-118">Connector</span><span class="sxs-lookup"><span data-stu-id="999f7-118">Connector</span></span>](connector.md)
- [<span data-ttu-id="999f7-119">连接器组</span><span class="sxs-lookup"><span data-stu-id="999f7-119">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


