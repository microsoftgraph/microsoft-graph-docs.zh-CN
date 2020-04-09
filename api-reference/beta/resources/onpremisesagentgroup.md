---
title: onPremisesAgentGroup 资源类型
description: onPremisesAgentGroup 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a211fb4245e8f4e4ef23158c0f553876303ea9c9
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199716"
---
# <a name="onpremisesagentgroup-resource-type"></a><span data-ttu-id="ec333-103">onPremisesAgentGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec333-103">onPremisesAgentGroup resource type</span></span>

<span data-ttu-id="ec333-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec333-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec333-105">表示本地代理组。</span><span class="sxs-lookup"><span data-stu-id="ec333-105">Represents on-premises agents group.</span></span> <span data-ttu-id="ec333-106">通过代理组，租户管理员可以分配特定的[代理](onpremisesagent.md)来服务特定[的已发布内部部署资源](publishedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="ec333-106">Agent groups enable a tenant admin to assign specific [agents](onpremisesagent.md) to serve specific [published on-premises resources](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ec333-107">方法</span><span class="sxs-lookup"><span data-stu-id="ec333-107">Methods</span></span>

| <span data-ttu-id="ec333-108">方法</span><span class="sxs-lookup"><span data-stu-id="ec333-108">Method</span></span>       | <span data-ttu-id="ec333-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ec333-109">Return Type</span></span> | <span data-ttu-id="ec333-110">说明</span><span class="sxs-lookup"><span data-stu-id="ec333-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ec333-111">列出 onPremisesAgentGroups</span><span class="sxs-lookup"><span data-stu-id="ec333-111">List onPremisesAgentGroups</span></span>](../api/onpremisesagentgroup-list.md) | <span data-ttu-id="ec333-112">onPremisesAgentGroups 集合</span><span class="sxs-lookup"><span data-stu-id="ec333-112">onPremisesAgentGroups collection</span></span> | <span data-ttu-id="ec333-113">获取**onPremisesAgentGroup**对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec333-113">Get an **onPremisesAgentGroup** objects collection.</span></span> |
| [<span data-ttu-id="ec333-114">获取 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-114">Get onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-get.md) | [<span data-ttu-id="ec333-115">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-115">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="ec333-116">读取**onPremisesAgentGroup**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec333-116">Read the properties and relationships of an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="ec333-117">创建 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-117">Create onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-post.md)  | [<span data-ttu-id="ec333-118">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-118">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="ec333-119">创建新的**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="ec333-119">Create a new **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="ec333-120">更新 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-120">Update onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-update.md) | [<span data-ttu-id="ec333-121">onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-121">onPremisesAgentGroup</span></span>](onpremisesagentgroup.md) | <span data-ttu-id="ec333-122">更新**onPremisesAgentGroup**对象。</span><span class="sxs-lookup"><span data-stu-id="ec333-122">Update an **onPremisesAgentGroup** object.</span></span> |
| [<span data-ttu-id="ec333-123">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="ec333-123">Delete  onPremisesAgentGroup</span></span>](../api/onpremisesagentgroup-delete.md) | <span data-ttu-id="ec333-124">无</span><span class="sxs-lookup"><span data-stu-id="ec333-124">None</span></span> | <span data-ttu-id="ec333-125">删除**onPremisesAgentGroup**对象。</span><span class="sxs-lookup"><span data-stu-id="ec333-125">Delete an **onPremisesAgentGroup** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec333-126">属性</span><span class="sxs-lookup"><span data-stu-id="ec333-126">Properties</span></span>

| <span data-ttu-id="ec333-127">属性</span><span class="sxs-lookup"><span data-stu-id="ec333-127">Property</span></span>     | <span data-ttu-id="ec333-128">类型</span><span class="sxs-lookup"><span data-stu-id="ec333-128">Type</span></span>        | <span data-ttu-id="ec333-129">说明</span><span class="sxs-lookup"><span data-stu-id="ec333-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec333-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ec333-130">displayName</span></span>|<span data-ttu-id="ec333-131">String</span><span class="sxs-lookup"><span data-stu-id="ec333-131">String</span></span>|<span data-ttu-id="ec333-132">**OnPremisesAgentGroup**的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ec333-132">Display name of the **onPremisesAgentGroup**.</span></span>|
|<span data-ttu-id="ec333-133">id</span><span class="sxs-lookup"><span data-stu-id="ec333-133">id</span></span>|<span data-ttu-id="ec333-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ec333-134">String</span></span>| <span data-ttu-id="ec333-135">**OnPremisesAgentGroup**的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="ec333-135">The object ID of the **onPremisesAgentGroup**.</span></span> <span data-ttu-id="ec333-136">只读。</span><span class="sxs-lookup"><span data-stu-id="ec333-136">Read-only.</span></span>|
|<span data-ttu-id="ec333-137">isDefault</span><span class="sxs-lookup"><span data-stu-id="ec333-137">isDefault</span></span>|<span data-ttu-id="ec333-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec333-138">Boolean</span></span>|<span data-ttu-id="ec333-139">指示**onPremisesAgentGroup**是否为默认代理组。</span><span class="sxs-lookup"><span data-stu-id="ec333-139">Indicates if the **onPremisesAgentGroup** is the default agent group.</span></span> <span data-ttu-id="ec333-140">只有一个代理组可以是默认的**onPremisesAgentGroup** ，并由系统进行设置。</span><span class="sxs-lookup"><span data-stu-id="ec333-140">Only a single agent group can be the default **onPremisesAgentGroup** and is set by the system.</span></span>|
|<span data-ttu-id="ec333-141">publishingType</span><span class="sxs-lookup"><span data-stu-id="ec333-141">publishingType</span></span>|<span data-ttu-id="ec333-142">string</span><span class="sxs-lookup"><span data-stu-id="ec333-142">string</span></span>| <span data-ttu-id="ec333-143">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="ec333-143">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec333-144">关系</span><span class="sxs-lookup"><span data-stu-id="ec333-144">Relationships</span></span>

| <span data-ttu-id="ec333-145">关系</span><span class="sxs-lookup"><span data-stu-id="ec333-145">Relationship</span></span> | <span data-ttu-id="ec333-146">类型</span><span class="sxs-lookup"><span data-stu-id="ec333-146">Type</span></span>        | <span data-ttu-id="ec333-147">说明</span><span class="sxs-lookup"><span data-stu-id="ec333-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec333-148">agent</span><span class="sxs-lookup"><span data-stu-id="ec333-148">agents</span></span>|<span data-ttu-id="ec333-149">[onPremisesAgent](onpremisesagent.md)集合</span><span class="sxs-lookup"><span data-stu-id="ec333-149">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="ec333-150">分配给**onPremisesAgentGroup**的**onPremisesAgent**的列表。</span><span class="sxs-lookup"><span data-stu-id="ec333-150">List of **onPremisesAgent** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="ec333-151">只读。</span><span class="sxs-lookup"><span data-stu-id="ec333-151">Read-only.</span></span> <span data-ttu-id="ec333-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ec333-152">Nullable.</span></span>|
|<span data-ttu-id="ec333-153">publishedResources</span><span class="sxs-lookup"><span data-stu-id="ec333-153">publishedResources</span></span>|<span data-ttu-id="ec333-154">[publishedResource](publishedresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ec333-154">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="ec333-155">分配给**onPremisesAgentGroup**的**publishedResource**的列表。</span><span class="sxs-lookup"><span data-stu-id="ec333-155">List of **publishedResource** that are assigned to an **onPremisesAgentGroup**.</span></span> <span data-ttu-id="ec333-156">只读。</span><span class="sxs-lookup"><span data-stu-id="ec333-156">Read-only.</span></span> <span data-ttu-id="ec333-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ec333-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec333-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec333-158">JSON representation</span></span>

<span data-ttu-id="ec333-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec333-159">The following is a JSON representation of the resource.</span></span>

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
