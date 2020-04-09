---
title: 本地发布配置文件
description: 各种 Azure 服务（例如，Azure Active Directory Connect 直通身份验证、从 Workday 到 Azure AD 用户预配）允许有条件访问公司网络外部的各种本地资源。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ea9e4b617bdf0b4a34633a3ce2379c3a4d438074
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200031"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="e0db7-103">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="e0db7-103">On-premises publishing profiles</span></span>

<span data-ttu-id="e0db7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0db7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0db7-105">各种 Azure 服务（例如，Azure Active Directory Connect 直通身份验证、从 Workday 到 Azure AD 用户预配）允许有条件访问公司网络外部的各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="e0db7-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="e0db7-106">可将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="e0db7-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="e0db7-107">通过[代理组](onpremisesagentgroup.md)，租户管理员可以分配特定的代理来服务特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="e0db7-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="e0db7-108">租户管理员可以将许多代理组合在一起，然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="e0db7-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="e0db7-109">同一本地发布类型的整个实体集由[onPremisesPublishingProfile](onpremisespublishingprofile.md)表示。</span><span class="sxs-lookup"><span data-stu-id="e0db7-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="e0db7-110">租户管理员可以为每个**onPremisesPublishingProfile**配置一个[时间](updatewindow.md)段，在此时段内，代理可以接收更新或将更新推迟到代理。</span><span class="sxs-lookup"><span data-stu-id="e0db7-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="e0db7-111">为**onPremisesPublishingProfile**指定的[更新配置](hybridagentupdaterconfiguration.md)适用于该**onPremisesPublishingProfile**中的所有代理。</span><span class="sxs-lookup"><span data-stu-id="e0db7-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="e0db7-112">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e0db7-112">See also</span></span>

- [<span data-ttu-id="e0db7-113">内部部署代理</span><span class="sxs-lookup"><span data-stu-id="e0db7-113">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="e0db7-114">内部部署代理组</span><span class="sxs-lookup"><span data-stu-id="e0db7-114">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="e0db7-115">本地发布配置文件</span><span class="sxs-lookup"><span data-stu-id="e0db7-115">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="e0db7-116">已发布资源</span><span class="sxs-lookup"><span data-stu-id="e0db7-116">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
