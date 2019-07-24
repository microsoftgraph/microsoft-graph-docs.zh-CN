---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1eb442b6f3317ac7c0e2f130442e4a62c7f9c152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841323"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="e2af0-103">onPremisesPublishingProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2af0-103">onPremisesPublishingProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2af0-104">各种 Azure 服务 (例如, Azue Active Directory Connect 直通 Authentication、从 Workday 到 Azure AD 用户预配) 允许从公司网络外部对各种本地资源进行条件访问。</span><span class="sxs-lookup"><span data-stu-id="e2af0-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="e2af0-105">可将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="e2af0-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="e2af0-106">通过[代理组](onpremisesagentgroup.md), 租户管理员可以分配特定的代理来服务特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="e2af0-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="e2af0-107">租户管理员可以将许多代理组合在一起, 然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="e2af0-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="e2af0-108">同一本地发布类型的整个实体集由**onPremisesPublishingProfile**表示。</span><span class="sxs-lookup"><span data-stu-id="e2af0-108">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="e2af0-109">方法</span><span class="sxs-lookup"><span data-stu-id="e2af0-109">Methods</span></span>

| <span data-ttu-id="e2af0-110">方法</span><span class="sxs-lookup"><span data-stu-id="e2af0-110">Method</span></span>       | <span data-ttu-id="e2af0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2af0-111">Return Type</span></span> | <span data-ttu-id="e2af0-112">说明</span><span class="sxs-lookup"><span data-stu-id="e2af0-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e2af0-113">获取 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="e2af0-113">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="e2af0-114">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="e2af0-114">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="e2af0-115">读取**onPremisesPublishingProfile**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2af0-115">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="e2af0-116">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="e2af0-116">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="e2af0-117">无</span><span class="sxs-lookup"><span data-stu-id="e2af0-117">None</span></span> | <span data-ttu-id="e2af0-118">更新[onPremisesPublishingProfile](onpremisespublishingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2af0-118">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="e2af0-119">属性</span><span class="sxs-lookup"><span data-stu-id="e2af0-119">Properties</span></span>

| <span data-ttu-id="e2af0-120">属性</span><span class="sxs-lookup"><span data-stu-id="e2af0-120">Property</span></span>     | <span data-ttu-id="e2af0-121">类型</span><span class="sxs-lookup"><span data-stu-id="e2af0-121">Type</span></span>        | <span data-ttu-id="e2af0-122">说明</span><span class="sxs-lookup"><span data-stu-id="e2af0-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2af0-123">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2af0-123">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="e2af0-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2af0-124">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="e2af0-125">表示一个**hybridAgentUpdaterConfiguration**对象。</span><span class="sxs-lookup"><span data-stu-id="e2af0-125">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="e2af0-126">id</span><span class="sxs-lookup"><span data-stu-id="e2af0-126">id</span></span>|<span data-ttu-id="e2af0-127">String</span><span class="sxs-lookup"><span data-stu-id="e2af0-127">String</span></span>| <span data-ttu-id="e2af0-128">表示发布类型。</span><span class="sxs-lookup"><span data-stu-id="e2af0-128">Represents a publishing type.</span></span> <span data-ttu-id="e2af0-129">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="e2af0-129">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="e2af0-130">只读。</span><span class="sxs-lookup"><span data-stu-id="e2af0-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2af0-131">关系</span><span class="sxs-lookup"><span data-stu-id="e2af0-131">Relationships</span></span>

| <span data-ttu-id="e2af0-132">关系</span><span class="sxs-lookup"><span data-stu-id="e2af0-132">Relationship</span></span> | <span data-ttu-id="e2af0-133">类型</span><span class="sxs-lookup"><span data-stu-id="e2af0-133">Type</span></span>        | <span data-ttu-id="e2af0-134">说明</span><span class="sxs-lookup"><span data-stu-id="e2af0-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2af0-135">agentGroups</span><span class="sxs-lookup"><span data-stu-id="e2af0-135">agentGroups</span></span>|<span data-ttu-id="e2af0-136">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2af0-136">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="e2af0-137">现有**onPremisesAgentGroup**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e2af0-137">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="e2af0-138">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e2af0-138">Read-only.</span></span> <span data-ttu-id="e2af0-139">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e2af0-139">Nullable.</span></span>|
|<span data-ttu-id="e2af0-140">agent</span><span class="sxs-lookup"><span data-stu-id="e2af0-140">agents</span></span>|<span data-ttu-id="e2af0-141">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2af0-141">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="e2af0-142">已存在的**onPremisesAgent**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e2af0-142">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="e2af0-143">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e2af0-143">Read-only.</span></span> <span data-ttu-id="e2af0-144">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e2af0-144">Nullable.</span></span>|
|<span data-ttu-id="e2af0-145">publishedResources</span><span class="sxs-lookup"><span data-stu-id="e2af0-145">publishedResources</span></span>|<span data-ttu-id="e2af0-146">[publishedResource](publishedresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2af0-146">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="e2af0-147">现有**publishedResource**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e2af0-147">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="e2af0-148">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e2af0-148">Read-only.</span></span> <span data-ttu-id="e2af0-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e2af0-149">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2af0-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2af0-150">JSON representation</span></span>

<span data-ttu-id="e2af0-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2af0-151">The following is a JSON representation of the resource.</span></span>

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
