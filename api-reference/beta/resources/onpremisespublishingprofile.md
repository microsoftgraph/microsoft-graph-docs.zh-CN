---
title: onPremisesPublishingProfile 资源类型
description: onPremisesPublishingProfile 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a4e1e40a5a8774be9498f6b89d235557ba2948e
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200024"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="8bac4-103">onPremisesPublishingProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bac4-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="8bac4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bac4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bac4-105">各种 Azure 服务（例如，Azure Active Directory Connect 直通身份验证、从 Workday 到 Azure AD 用户预配）允许有条件访问公司网络外部的各种本地资源。</span><span class="sxs-lookup"><span data-stu-id="8bac4-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="8bac4-106">可将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的[已发布资源](publishedresource.md)的请求。</span><span class="sxs-lookup"><span data-stu-id="8bac4-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="8bac4-107">通过[代理组](onpremisesagentgroup.md)，租户管理员可以分配特定的代理来服务特定的已发布内部部署资源。</span><span class="sxs-lookup"><span data-stu-id="8bac4-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="8bac4-108">租户管理员可以将许多代理组合在一起，然后将每个已发布的资源分配给一个组。</span><span class="sxs-lookup"><span data-stu-id="8bac4-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="8bac4-109">同一本地发布类型的整个实体集由**onPremisesPublishingProfile**表示。</span><span class="sxs-lookup"><span data-stu-id="8bac4-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="8bac4-110">方法</span><span class="sxs-lookup"><span data-stu-id="8bac4-110">Methods</span></span>

| <span data-ttu-id="8bac4-111">方法</span><span class="sxs-lookup"><span data-stu-id="8bac4-111">Method</span></span>       | <span data-ttu-id="8bac4-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="8bac4-112">Return Type</span></span> | <span data-ttu-id="8bac4-113">说明</span><span class="sxs-lookup"><span data-stu-id="8bac4-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8bac4-114">获取 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8bac4-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="8bac4-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8bac4-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="8bac4-116">读取**onPremisesPublishingProfile**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bac4-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="8bac4-117">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="8bac4-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="8bac4-118">无</span><span class="sxs-lookup"><span data-stu-id="8bac4-118">None</span></span> | <span data-ttu-id="8bac4-119">更新[onPremisesPublishingProfile](onpremisespublishingprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8bac4-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="8bac4-120">属性</span><span class="sxs-lookup"><span data-stu-id="8bac4-120">Properties</span></span>

| <span data-ttu-id="8bac4-121">属性</span><span class="sxs-lookup"><span data-stu-id="8bac4-121">Property</span></span>     | <span data-ttu-id="8bac4-122">类型</span><span class="sxs-lookup"><span data-stu-id="8bac4-122">Type</span></span>        | <span data-ttu-id="8bac4-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bac4-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bac4-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bac4-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="8bac4-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="8bac4-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="8bac4-126">表示一个**hybridAgentUpdaterConfiguration**对象。</span><span class="sxs-lookup"><span data-stu-id="8bac4-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="8bac4-127">id</span><span class="sxs-lookup"><span data-stu-id="8bac4-127">id</span></span>|<span data-ttu-id="8bac4-128">字符串</span><span class="sxs-lookup"><span data-stu-id="8bac4-128">String</span></span>| <span data-ttu-id="8bac4-129">表示发布类型。</span><span class="sxs-lookup"><span data-stu-id="8bac4-129">Represents a publishing type.</span></span> <span data-ttu-id="8bac4-130">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="8bac4-130">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="8bac4-131">只读。</span><span class="sxs-lookup"><span data-stu-id="8bac4-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bac4-132">关系</span><span class="sxs-lookup"><span data-stu-id="8bac4-132">Relationships</span></span>

| <span data-ttu-id="8bac4-133">关系</span><span class="sxs-lookup"><span data-stu-id="8bac4-133">Relationship</span></span> | <span data-ttu-id="8bac4-134">类型</span><span class="sxs-lookup"><span data-stu-id="8bac4-134">Type</span></span>        | <span data-ttu-id="8bac4-135">说明</span><span class="sxs-lookup"><span data-stu-id="8bac4-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bac4-136">agentGroups</span><span class="sxs-lookup"><span data-stu-id="8bac4-136">agentGroups</span></span>|<span data-ttu-id="8bac4-137">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bac4-137">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="8bac4-138">现有**onPremisesAgentGroup**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8bac4-138">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="8bac4-139">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="8bac4-139">Read-only.</span></span> <span data-ttu-id="8bac4-140">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8bac4-140">Nullable.</span></span>|
|<span data-ttu-id="8bac4-141">agent</span><span class="sxs-lookup"><span data-stu-id="8bac4-141">agents</span></span>|<span data-ttu-id="8bac4-142">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bac4-142">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="8bac4-143">已存在的**onPremisesAgent**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8bac4-143">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="8bac4-144">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="8bac4-144">Read-only.</span></span> <span data-ttu-id="8bac4-145">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8bac4-145">Nullable.</span></span>|
|<span data-ttu-id="8bac4-146">publishedResources</span><span class="sxs-lookup"><span data-stu-id="8bac4-146">publishedResources</span></span>|<span data-ttu-id="8bac4-147">[publishedResource](publishedresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bac4-147">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="8bac4-148">现有**publishedResource**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8bac4-148">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="8bac4-149">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="8bac4-149">Read-only.</span></span> <span data-ttu-id="8bac4-150">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8bac4-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bac4-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bac4-151">JSON representation</span></span>

<span data-ttu-id="8bac4-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bac4-152">The following is a JSON representation of the resource.</span></span>

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
