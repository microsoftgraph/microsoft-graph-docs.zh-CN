---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e74a49a9a8c4b57232ed90cef232fa8b7feb998
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841316"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="3c860-103">onPremisesAgentGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c860-103">onPremisesAgentGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c860-104">表示本地代理组。</span><span class="sxs-lookup"><span data-stu-id="3c860-104">Represents on-premises agents group.</span></span> <span data-ttu-id="3c860-105">通过代理组, 租户管理员可以分配特定的[代理](onpremisesagent.md)来服务特定[的已发布内部部署资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="3c860-105">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3c860-106">方法</span><span class="sxs-lookup"><span data-stu-id="3c860-106">Methods</span></span>

| <span data-ttu-id="3c860-107">方法</span><span class="sxs-lookup"><span data-stu-id="3c860-107">Method</span></span>       | <span data-ttu-id="3c860-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c860-108">Return Type</span></span> | <span data-ttu-id="3c860-109">说明</span><span class="sxs-lookup"><span data-stu-id="3c860-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3c860-110">列出 onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="3c860-110">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="3c860-111">onPremisesAgentGroups 集合</span><span class="sxs-lookup"><span data-stu-id="3c860-111">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="3c860-112">获取**onPremisesAgentGroup**对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c860-112">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="3c860-113">获取 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-113">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="3c860-114">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-114">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="3c860-115">读取**onPremisesAgentGroup**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c860-115">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="3c860-116">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-116">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="3c860-117">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-117">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="3c860-118">创建新的**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="3c860-118">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="3c860-119">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-119">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="3c860-120">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-120">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="3c860-121">更新**onPremisesAgentGroup**对象。</span><span class="sxs-lookup"><span data-stu-id="3c860-121">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="3c860-122">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3c860-122">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="3c860-123">无</span><span class="sxs-lookup"><span data-stu-id="3c860-123">None</span></span> | <span data-ttu-id="3c860-124">删除**onPremisesAgentGroup**对象。</span><span class="sxs-lookup"><span data-stu-id="3c860-124">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3c860-125">属性</span><span class="sxs-lookup"><span data-stu-id="3c860-125">Properties</span></span>

| <span data-ttu-id="3c860-126">属性</span><span class="sxs-lookup"><span data-stu-id="3c860-126">Property</span></span>     | <span data-ttu-id="3c860-127">类型</span><span class="sxs-lookup"><span data-stu-id="3c860-127">Type</span></span>        | <span data-ttu-id="3c860-128">说明</span><span class="sxs-lookup"><span data-stu-id="3c860-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c860-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3c860-129">displayName</span></span>|<span data-ttu-id="3c860-130">String</span><span class="sxs-lookup"><span data-stu-id="3c860-130">String</span></span>|<span data-ttu-id="3c860-131">**OnPremisesAgentGroup**的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3c860-131">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="3c860-132">id</span><span class="sxs-lookup"><span data-stu-id="3c860-132">id</span></span>|<span data-ttu-id="3c860-133">String</span><span class="sxs-lookup"><span data-stu-id="3c860-133">String</span></span>| <span data-ttu-id="3c860-134">**OnPremisesAgentGroup**的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="3c860-134">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="3c860-135">只读。</span><span class="sxs-lookup"><span data-stu-id="3c860-135">Read-only.</span></span>|
|<span data-ttu-id="3c860-136">isDefault</span><span class="sxs-lookup"><span data-stu-id="3c860-136">isDefault</span></span>|<span data-ttu-id="3c860-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c860-137">Boolean</span></span>|<span data-ttu-id="3c860-138">指示**onPremisesAgentGroup**是否为默认代理组。</span><span class="sxs-lookup"><span data-stu-id="3c860-138">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="3c860-139">只有一个代理组可以是默认的**onPremisesAgentGroup** , 并由系统进行设置。</span><span class="sxs-lookup"><span data-stu-id="3c860-139">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="3c860-140">publishingType</span><span class="sxs-lookup"><span data-stu-id="3c860-140">publishingType</span></span>|<span data-ttu-id="3c860-141">string</span><span class="sxs-lookup"><span data-stu-id="3c860-141">string</span></span>| <span data-ttu-id="3c860-142">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="3c860-142">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c860-143">关系</span><span class="sxs-lookup"><span data-stu-id="3c860-143">Relationships</span></span>

| <span data-ttu-id="3c860-144">关系</span><span class="sxs-lookup"><span data-stu-id="3c860-144">Relationship</span></span> | <span data-ttu-id="3c860-145">类型</span><span class="sxs-lookup"><span data-stu-id="3c860-145">Type</span></span>        | <span data-ttu-id="3c860-146">说明</span><span class="sxs-lookup"><span data-stu-id="3c860-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c860-147">agent</span><span class="sxs-lookup"><span data-stu-id="3c860-147">agents</span></span>|<span data-ttu-id="3c860-148">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c860-148">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="3c860-149">分配给**onPremisesAgentGroup**的**onPremisesAgent**的列表。</span><span class="sxs-lookup"><span data-stu-id="3c860-149">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="3c860-150">只读。</span><span class="sxs-lookup"><span data-stu-id="3c860-150">Read-only.</span></span> <span data-ttu-id="3c860-151">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3c860-151">Nullable.</span></span>|
|<span data-ttu-id="3c860-152">publishedResources</span><span class="sxs-lookup"><span data-stu-id="3c860-152">publishedResources</span></span>|<span data-ttu-id="3c860-153">[publishedResource](publishedresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c860-153">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="3c860-154">分配给**onPremisesAgentGroup**的**publishedResource**的列表。</span><span class="sxs-lookup"><span data-stu-id="3c860-154">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="3c860-155">只读。</span><span class="sxs-lookup"><span data-stu-id="3c860-155">Read-only.</span></span> <span data-ttu-id="3c860-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3c860-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c860-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c860-157">JSON representation</span></span>

<span data-ttu-id="3c860-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c860-158">The following is a JSON representation of the resource.</span></span>

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
