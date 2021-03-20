---
title: publishedResource 资源类型
description: publishedResource 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: e55abdad4a03319407b1c6e31e37e717739f0d10
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941762"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="bc2ff-103">publishedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc2ff-103">publishedResource resource type</span></span>

<span data-ttu-id="bc2ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc2ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc2ff-105">表示本地已发布资源。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-105">Represents on-premises published resource.</span></span> <span data-ttu-id="bc2ff-106">租户管理员可以发布各种类型的本地资源-企业应用程序、域控制器、服务器等。租户管理员安装本地代理可以配置为访问[](onpremisesagent.md)/处理对特定已发布资源的请求。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="bc2ff-107">Methods</span><span class="sxs-lookup"><span data-stu-id="bc2ff-107">Methods</span></span>

| <span data-ttu-id="bc2ff-108">方法</span><span class="sxs-lookup"><span data-stu-id="bc2ff-108">Method</span></span>       | <span data-ttu-id="bc2ff-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc2ff-109">Return Type</span></span> | <span data-ttu-id="bc2ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc2ff-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bc2ff-111">列出 publishedResources</span><span class="sxs-lookup"><span data-stu-id="bc2ff-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="bc2ff-112">[publishedResource](publishedresource.md) 对象集合</span><span class="sxs-lookup"><span data-stu-id="bc2ff-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="bc2ff-113">获取 **publishedResources** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="bc2ff-114">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="bc2ff-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="bc2ff-116">读取 **publishedResource 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="bc2ff-117">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="bc2ff-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="bc2ff-119">创建新的 **publishedResource**。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="bc2ff-120">更新 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="bc2ff-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="bc2ff-122">更新 **publishedResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="bc2ff-123">删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="bc2ff-124">无</span><span class="sxs-lookup"><span data-stu-id="bc2ff-124">None</span></span> | <span data-ttu-id="bc2ff-125">删除 **publishedResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="bc2ff-126">将 publishedResource 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="bc2ff-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="bc2ff-127">无</span><span class="sxs-lookup"><span data-stu-id="bc2ff-127">None</span></span> | <span data-ttu-id="bc2ff-128">将 **publishedResource** 对象分配给 **onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="bc2ff-129">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="bc2ff-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="bc2ff-130">无</span><span class="sxs-lookup"><span data-stu-id="bc2ff-130">None</span></span> |  <span data-ttu-id="bc2ff-131">从 **onPremisesAgentGroup** 中删除 **publishedResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc2ff-132">属性</span><span class="sxs-lookup"><span data-stu-id="bc2ff-132">Properties</span></span>

| <span data-ttu-id="bc2ff-133">属性</span><span class="sxs-lookup"><span data-stu-id="bc2ff-133">Property</span></span>     | <span data-ttu-id="bc2ff-134">类型</span><span class="sxs-lookup"><span data-stu-id="bc2ff-134">Type</span></span>        | <span data-ttu-id="bc2ff-135">说明</span><span class="sxs-lookup"><span data-stu-id="bc2ff-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc2ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bc2ff-136">displayName</span></span>|<span data-ttu-id="bc2ff-137">String</span><span class="sxs-lookup"><span data-stu-id="bc2ff-137">String</span></span>| <span data-ttu-id="bc2ff-138">publishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="bc2ff-139">id</span><span class="sxs-lookup"><span data-stu-id="bc2ff-139">id</span></span>|<span data-ttu-id="bc2ff-140">String</span><span class="sxs-lookup"><span data-stu-id="bc2ff-140">String</span></span>| <span data-ttu-id="bc2ff-141">publishedResource 的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-141">The object id of the publishedResource.</span></span> <span data-ttu-id="bc2ff-142">只读。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-142">Read-only.</span></span>|
|<span data-ttu-id="bc2ff-143">publishingType</span><span class="sxs-lookup"><span data-stu-id="bc2ff-143">publishingType</span></span>|<span data-ttu-id="bc2ff-144">String</span><span class="sxs-lookup"><span data-stu-id="bc2ff-144">String</span></span>| <span data-ttu-id="bc2ff-145">可取值为：`applicationProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="bc2ff-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="bc2ff-146">resourceName</span></span>|<span data-ttu-id="bc2ff-147">String</span><span class="sxs-lookup"><span data-stu-id="bc2ff-147">String</span></span>|<span data-ttu-id="bc2ff-148">publishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc2ff-149">关系</span><span class="sxs-lookup"><span data-stu-id="bc2ff-149">Relationships</span></span>

| <span data-ttu-id="bc2ff-150">关系</span><span class="sxs-lookup"><span data-stu-id="bc2ff-150">Relationship</span></span> | <span data-ttu-id="bc2ff-151">类型</span><span class="sxs-lookup"><span data-stu-id="bc2ff-151">Type</span></span>        | <span data-ttu-id="bc2ff-152">说明</span><span class="sxs-lookup"><span data-stu-id="bc2ff-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc2ff-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="bc2ff-153">agentGroups</span></span>|<span data-ttu-id="bc2ff-154">[onPremisesAgentGroup](onpremisesagentgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc2ff-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="bc2ff-155">**publishedResource** 分配到 **的 onPremisesAgentGroups** 的列表。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="bc2ff-156">只读。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-156">Read-only.</span></span> <span data-ttu-id="bc2ff-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc2ff-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc2ff-158">JSON representation</span></span>

<span data-ttu-id="bc2ff-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc2ff-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


