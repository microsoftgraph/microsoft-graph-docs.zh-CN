---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4299ddec6a05e079d86a070b939c2220087281a0
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921527"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="39680-103">onPremisesPublishingProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="39680-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="39680-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39680-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39680-105">各种 Azure 服务 (例如，Azure Active Directory Connect [直通身份验证](/azure/active-directory/hybrid/how-to-connect-pta)、从 [WORKDAY 到 azure AD 用户设置](/azure/active-directory/saas-apps/workday-inbound-tutorial)以及 [应用程序代理](https://aka.ms/whyappproxy) 允许从公司网络外部访问各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="39680-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="39680-106">可将[本地代理](onpremisesagent.md) (或[连接器](connector.md)，以供管理员安装的应用程序代理) 配置为将请求路由到特定的[已发布资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="39680-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="39680-107">[代理组](onpremisesagentgroup.md) (或 [连接器组](connectorgroup.md) 应用程序代理) 使管理员能够分配特定的代理来满足特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="39680-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="39680-108">管理员还可以将多个代理组合在一起，然后将每个已发布的资源分配给一个代理组。</span><span class="sxs-lookup"><span data-stu-id="39680-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="39680-109">同一本地发布类型的整个实体集由 **onPremisesPublishingProfile** 表示。</span><span class="sxs-lookup"><span data-stu-id="39680-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="39680-110">方法</span><span class="sxs-lookup"><span data-stu-id="39680-110">Methods</span></span>

| <span data-ttu-id="39680-111">方法</span><span class="sxs-lookup"><span data-stu-id="39680-111">Method</span></span>       | <span data-ttu-id="39680-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="39680-112">Return Type</span></span> | <span data-ttu-id="39680-113">说明</span><span class="sxs-lookup"><span data-stu-id="39680-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="39680-114">获取 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="39680-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="39680-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="39680-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="39680-116">读取 **onPremisesPublishingProfile** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39680-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="39680-117">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="39680-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="39680-118">无</span><span class="sxs-lookup"><span data-stu-id="39680-118">None</span></span> | <span data-ttu-id="39680-119">更新 [onPremisesPublishingProfile](onpremisespublishingprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39680-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="39680-120">属性</span><span class="sxs-lookup"><span data-stu-id="39680-120">Properties</span></span>

| <span data-ttu-id="39680-121">属性</span><span class="sxs-lookup"><span data-stu-id="39680-121">Property</span></span>     | <span data-ttu-id="39680-122">类型</span><span class="sxs-lookup"><span data-stu-id="39680-122">Type</span></span>        | <span data-ttu-id="39680-123">说明</span><span class="sxs-lookup"><span data-stu-id="39680-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39680-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="39680-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="39680-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="39680-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="39680-126">表示一个 **hybridAgentUpdaterConfiguration** 对象。</span><span class="sxs-lookup"><span data-stu-id="39680-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="39680-127">id</span><span class="sxs-lookup"><span data-stu-id="39680-127">id</span></span>|<span data-ttu-id="39680-128">String</span><span class="sxs-lookup"><span data-stu-id="39680-128">String</span></span>| <span data-ttu-id="39680-129">表示发布类型。</span><span class="sxs-lookup"><span data-stu-id="39680-129">Represents a publishing type.</span></span> <span data-ttu-id="39680-130">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="39680-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="39680-131">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-131">Read-only.</span></span>|
|<span data-ttu-id="39680-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="39680-132">isEnabled</span></span>|<span data-ttu-id="39680-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="39680-133">Boolean</span></span>| <span data-ttu-id="39680-134">表示是否为租户启用了 [AZURE AD 应用程序代理](https://aka.ms/whyappproxy) 。</span><span class="sxs-lookup"><span data-stu-id="39680-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="39680-135">关系</span><span class="sxs-lookup"><span data-stu-id="39680-135">Relationships</span></span>

| <span data-ttu-id="39680-136">关系</span><span class="sxs-lookup"><span data-stu-id="39680-136">Relationship</span></span> | <span data-ttu-id="39680-137">类型</span><span class="sxs-lookup"><span data-stu-id="39680-137">Type</span></span>        | <span data-ttu-id="39680-138">说明</span><span class="sxs-lookup"><span data-stu-id="39680-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39680-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="39680-139">agentGroups</span></span>|<span data-ttu-id="39680-140">[onPremisesAgentGroup](onpremisesagentgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39680-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="39680-141">现有 **onPremisesAgentGroup** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="39680-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="39680-142">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-142">Read-only.</span></span> <span data-ttu-id="39680-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="39680-143">Nullable.</span></span>|
|<span data-ttu-id="39680-144">agent</span><span class="sxs-lookup"><span data-stu-id="39680-144">agents</span></span>|<span data-ttu-id="39680-145">[onPremisesAgent](onpremisesagent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39680-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="39680-146">现有 **onPremisesAgent** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="39680-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="39680-147">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-147">Read-only.</span></span> <span data-ttu-id="39680-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="39680-148">Nullable.</span></span>|
|<span data-ttu-id="39680-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="39680-149">connectorGroups</span></span>|<span data-ttu-id="39680-150">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39680-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="39680-151">通过应用程序代理发布的应用程序的现有 **connectorGroup** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="39680-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="39680-152">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-152">Read-only.</span></span> <span data-ttu-id="39680-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="39680-153">Nullable.</span></span>|
|<span data-ttu-id="39680-154">插槽</span><span class="sxs-lookup"><span data-stu-id="39680-154">connectors</span></span>|<span data-ttu-id="39680-155">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39680-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="39680-156">通过应用程序代理发布的应用程序的现有 **连接器** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="39680-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="39680-157">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-157">Read-only.</span></span> <span data-ttu-id="39680-158">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="39680-158">Nullable.</span></span>|
|<span data-ttu-id="39680-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="39680-159">publishedResources</span></span>|<span data-ttu-id="39680-160">[publishedResource](publishedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39680-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="39680-161">现有 **publishedResource** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="39680-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="39680-162">只读。</span><span class="sxs-lookup"><span data-stu-id="39680-162">Read-only.</span></span> <span data-ttu-id="39680-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="39680-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39680-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39680-164">JSON representation</span></span>

<span data-ttu-id="39680-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39680-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


