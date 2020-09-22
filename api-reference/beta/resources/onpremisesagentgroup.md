---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f0236c2c2e52742a84f19eae8eb7693f1b559b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052597"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="2bffb-103">onPremisesAgentGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bffb-103">onPremisesAgentGroup resource type</span></span>

<span data-ttu-id="2bffb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bffb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bffb-105">表示本地代理组。</span><span class="sxs-lookup"><span data-stu-id="2bffb-105">Represents on-premises agents group.</span></span> <span data-ttu-id="2bffb-106">通过代理组，租户管理员可以分配特定的 [代理](onpremisesagent.md) 来服务特定 [的已发布内部部署资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="2bffb-106">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2bffb-107">方法</span><span class="sxs-lookup"><span data-stu-id="2bffb-107">Methods</span></span>

| <span data-ttu-id="2bffb-108">方法</span><span class="sxs-lookup"><span data-stu-id="2bffb-108">Method</span></span>       | <span data-ttu-id="2bffb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bffb-109">Return Type</span></span> | <span data-ttu-id="2bffb-110">说明</span><span class="sxs-lookup"><span data-stu-id="2bffb-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2bffb-111">列出 onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="2bffb-111">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="2bffb-112">onPremisesAgentGroups 集合</span><span class="sxs-lookup"><span data-stu-id="2bffb-112">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="2bffb-113">获取 **onPremisesAgentGroup** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2bffb-113">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="2bffb-114">获取 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-114">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="2bffb-115">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-115">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="2bffb-116">读取 **onPremisesAgentGroup** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bffb-116">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="2bffb-117">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-117">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="2bffb-118">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-118">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="2bffb-119">创建新的 **onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="2bffb-119">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="2bffb-120">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-120">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="2bffb-121">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-121">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="2bffb-122">更新 **onPremisesAgentGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="2bffb-122">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="2bffb-123">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bffb-123">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="2bffb-124">无</span><span class="sxs-lookup"><span data-stu-id="2bffb-124">None</span></span> | <span data-ttu-id="2bffb-125">删除 **onPremisesAgentGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="2bffb-125">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2bffb-126">属性</span><span class="sxs-lookup"><span data-stu-id="2bffb-126">Properties</span></span>

| <span data-ttu-id="2bffb-127">属性</span><span class="sxs-lookup"><span data-stu-id="2bffb-127">Property</span></span>     | <span data-ttu-id="2bffb-128">类型</span><span class="sxs-lookup"><span data-stu-id="2bffb-128">Type</span></span>        | <span data-ttu-id="2bffb-129">说明</span><span class="sxs-lookup"><span data-stu-id="2bffb-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bffb-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2bffb-130">displayName</span></span>|<span data-ttu-id="2bffb-131">String</span><span class="sxs-lookup"><span data-stu-id="2bffb-131">String</span></span>|<span data-ttu-id="2bffb-132">**OnPremisesAgentGroup**的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2bffb-132">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="2bffb-133">id</span><span class="sxs-lookup"><span data-stu-id="2bffb-133">id</span></span>|<span data-ttu-id="2bffb-134">String</span><span class="sxs-lookup"><span data-stu-id="2bffb-134">String</span></span>| <span data-ttu-id="2bffb-135">**OnPremisesAgentGroup**的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="2bffb-135">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="2bffb-136">只读。</span><span class="sxs-lookup"><span data-stu-id="2bffb-136">Read-only.</span></span>|
|<span data-ttu-id="2bffb-137">isDefault</span><span class="sxs-lookup"><span data-stu-id="2bffb-137">isDefault</span></span>|<span data-ttu-id="2bffb-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bffb-138">Boolean</span></span>|<span data-ttu-id="2bffb-139">指示 **onPremisesAgentGroup** 是否为默认代理组。</span><span class="sxs-lookup"><span data-stu-id="2bffb-139">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="2bffb-140">只有一个代理组可以是默认的 **onPremisesAgentGroup** ，并由系统进行设置。</span><span class="sxs-lookup"><span data-stu-id="2bffb-140">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="2bffb-141">publishingType</span><span class="sxs-lookup"><span data-stu-id="2bffb-141">publishingType</span></span>|<span data-ttu-id="2bffb-142">string</span><span class="sxs-lookup"><span data-stu-id="2bffb-142">string</span></span>| <span data-ttu-id="2bffb-143">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="2bffb-143">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bffb-144">关系</span><span class="sxs-lookup"><span data-stu-id="2bffb-144">Relationships</span></span>

| <span data-ttu-id="2bffb-145">关系</span><span class="sxs-lookup"><span data-stu-id="2bffb-145">Relationship</span></span> | <span data-ttu-id="2bffb-146">类型</span><span class="sxs-lookup"><span data-stu-id="2bffb-146">Type</span></span>        | <span data-ttu-id="2bffb-147">说明</span><span class="sxs-lookup"><span data-stu-id="2bffb-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bffb-148">agent</span><span class="sxs-lookup"><span data-stu-id="2bffb-148">agents</span></span>|<span data-ttu-id="2bffb-149">[onPremisesAgent](onpremisesagent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2bffb-149">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="2bffb-150">分配给**onPremisesAgentGroup**的**onPremisesAgent**的列表。</span><span class="sxs-lookup"><span data-stu-id="2bffb-150">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="2bffb-151">只读。</span><span class="sxs-lookup"><span data-stu-id="2bffb-151">Read-only.</span></span> <span data-ttu-id="2bffb-152">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="2bffb-152">Nullable.</span></span>|
|<span data-ttu-id="2bffb-153">publishedResources</span><span class="sxs-lookup"><span data-stu-id="2bffb-153">publishedResources</span></span>|<span data-ttu-id="2bffb-154">[publishedResource](publishedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2bffb-154">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="2bffb-155">分配给**onPremisesAgentGroup**的**publishedResource**的列表。</span><span class="sxs-lookup"><span data-stu-id="2bffb-155">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="2bffb-156">只读。</span><span class="sxs-lookup"><span data-stu-id="2bffb-156">Read-only.</span></span> <span data-ttu-id="2bffb-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2bffb-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bffb-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bffb-158">JSON representation</span></span>

<span data-ttu-id="2bffb-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bffb-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "publishingType": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgentGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


