---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: da089ba198b5056bdecdceba96be572366618a23
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158343"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="e7ee0-103">onPremisesAgentGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7ee0-103">onPremisesAgentGroup resource type</span></span>

<span data-ttu-id="e7ee0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7ee0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7ee0-105">代表本地代理组。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-105">Represents on-premises agents group.</span></span> <span data-ttu-id="e7ee0-106">代理组使租户管理员能够分配特定 [代理](onpremisesagent.md) ，为 [发布的特定本地资源提供服务](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-106">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e7ee0-107">方法</span><span class="sxs-lookup"><span data-stu-id="e7ee0-107">Methods</span></span>

| <span data-ttu-id="e7ee0-108">方法</span><span class="sxs-lookup"><span data-stu-id="e7ee0-108">Method</span></span>       | <span data-ttu-id="e7ee0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7ee0-109">Return Type</span></span> | <span data-ttu-id="e7ee0-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7ee0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7ee0-111">列出 onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="e7ee0-111">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="e7ee0-112">onPremisesAgentGroups 集合</span><span class="sxs-lookup"><span data-stu-id="e7ee0-112">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="e7ee0-113">获取 **onPremisesAgentGroup** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-113">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="e7ee0-114">获取 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-114">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="e7ee0-115">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-115">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7ee0-116">读取 **onPremisesAgentGroup** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-116">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="e7ee0-117">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-117">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="e7ee0-118">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-118">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7ee0-119">创建新的 **onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-119">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="e7ee0-120">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-120">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="e7ee0-121">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-121">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="e7ee0-122">更新 **onPremisesAgentGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-122">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="e7ee0-123">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="e7ee0-123">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="e7ee0-124">无</span><span class="sxs-lookup"><span data-stu-id="e7ee0-124">None</span></span> | <span data-ttu-id="e7ee0-125">删除 **onPremisesAgentGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-125">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7ee0-126">属性</span><span class="sxs-lookup"><span data-stu-id="e7ee0-126">Properties</span></span>

| <span data-ttu-id="e7ee0-127">属性</span><span class="sxs-lookup"><span data-stu-id="e7ee0-127">Property</span></span>     | <span data-ttu-id="e7ee0-128">类型</span><span class="sxs-lookup"><span data-stu-id="e7ee0-128">Type</span></span>        | <span data-ttu-id="e7ee0-129">说明</span><span class="sxs-lookup"><span data-stu-id="e7ee0-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7ee0-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e7ee0-130">displayName</span></span>|<span data-ttu-id="e7ee0-131">String</span><span class="sxs-lookup"><span data-stu-id="e7ee0-131">String</span></span>|<span data-ttu-id="e7ee0-132">**onPremisesAgentGroup 的显示名称**。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-132">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="e7ee0-133">id</span><span class="sxs-lookup"><span data-stu-id="e7ee0-133">id</span></span>|<span data-ttu-id="e7ee0-134">String</span><span class="sxs-lookup"><span data-stu-id="e7ee0-134">String</span></span>| <span data-ttu-id="e7ee0-135">**onPremisesAgentGroup 的对象** ID。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-135">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7ee0-136">只读。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-136">Read-only.</span></span>|
|<span data-ttu-id="e7ee0-137">isDefault</span><span class="sxs-lookup"><span data-stu-id="e7ee0-137">isDefault</span></span>|<span data-ttu-id="e7ee0-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7ee0-138">Boolean</span></span>|<span data-ttu-id="e7ee0-139">指示 **onPremisesAgentGroup** 是否默认代理组。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-139">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="e7ee0-140">只有一个代理组可以是默认的 **onPremisesAgentGroup，** 并且由系统设置。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-140">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="e7ee0-141">publishingType</span><span class="sxs-lookup"><span data-stu-id="e7ee0-141">publishingType</span></span>|<span data-ttu-id="e7ee0-142">string</span><span class="sxs-lookup"><span data-stu-id="e7ee0-142">string</span></span>| <span data-ttu-id="e7ee0-143">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-143">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7ee0-144">关系</span><span class="sxs-lookup"><span data-stu-id="e7ee0-144">Relationships</span></span>

| <span data-ttu-id="e7ee0-145">关系</span><span class="sxs-lookup"><span data-stu-id="e7ee0-145">Relationship</span></span> | <span data-ttu-id="e7ee0-146">类型</span><span class="sxs-lookup"><span data-stu-id="e7ee0-146">Type</span></span>        | <span data-ttu-id="e7ee0-147">说明</span><span class="sxs-lookup"><span data-stu-id="e7ee0-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7ee0-148">agents</span><span class="sxs-lookup"><span data-stu-id="e7ee0-148">agents</span></span>|<span data-ttu-id="e7ee0-149">[onPremisesAgent](onpremisesagent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7ee0-149">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="e7ee0-150">分配给 **onPremisesAgentGroup** **的 onPremisesAgent 列表**。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-150">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7ee0-151">只读。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-151">Read-only.</span></span> <span data-ttu-id="e7ee0-152">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-152">Nullable.</span></span>|
|<span data-ttu-id="e7ee0-153">publishedResources</span><span class="sxs-lookup"><span data-stu-id="e7ee0-153">publishedResources</span></span>|<span data-ttu-id="e7ee0-154">[publishedResource](publishedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7ee0-154">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="e7ee0-155">分配给 **onPremisesAgentGroup** 的 **publishedResource** 列表。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-155">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="e7ee0-156">只读。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-156">Read-only.</span></span> <span data-ttu-id="e7ee0-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7ee0-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7ee0-158">JSON representation</span></span>

<span data-ttu-id="e7ee0-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7ee0-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
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



