---
title: 本地发布配置文件
description: 各种 Azure 服务 (例如, Azue Active Directory Connect 直通 Authentication、从 Workday 到 Azure AD 用户预配) 允许从公司网络外部对各种本地资源进行条件访问。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b0e975d932226adfa2c455baaa396c1d580f6ff
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841330"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="2d8b0-103">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="2d8b0-103">On-premises publishing profiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d8b0-104">各种 Azure 服务 (例如, Azue Active Directory Connect 直通 Authentication、从 Workday 到 Azure AD 用户预配) 允许从公司网络外部对各种本地资源进行条件访问。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="2d8b0-105">可将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="2d8b0-106">通过[代理组](onpremisesagentgroup.md), 租户管理员可以分配特定的代理来服务特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="2d8b0-107">租户管理员可以将许多代理组合在一起, 然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="2d8b0-108">同一本地发布类型的整个实体集由[onPremisesPublishingProfile](onpremisespublishingprofile.md)表示。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-108">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="2d8b0-109">租户管理员可以为每个**onPremisesPublishingProfile**配置一个[时间](updatewindow.md)段, 在此时段内, 代理可以接收更新或将更新推迟到代理。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-109">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="2d8b0-110">为**onPremisesPublishingProfile**指定的[更新配置](hybridagentupdaterconfiguration.md)适用于该**onPremisesPublishingProfile**中的所有代理。</span><span class="sxs-lookup"><span data-stu-id="2d8b0-110">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="2d8b0-111">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2d8b0-111">See also</span></span>

- [<span data-ttu-id="2d8b0-112">内部部署代理</span><span class="sxs-lookup"><span data-stu-id="2d8b0-112">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="2d8b0-113">内部部署代理组</span><span class="sxs-lookup"><span data-stu-id="2d8b0-113">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="2d8b0-114">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="2d8b0-114">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="2d8b0-115">已发布资源</span><span class="sxs-lookup"><span data-stu-id="2d8b0-115">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
