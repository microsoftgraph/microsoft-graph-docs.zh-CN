---
title: publishedResource 资源类型
description: publishedResource 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7b6f81f9e3a6b399f7e029e21330fe83b533af87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521290"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="9a09a-103">publishedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a09a-103">publishedResource resource type</span></span>

<span data-ttu-id="9a09a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a09a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a09a-105">表示本地发布的资源。</span><span class="sxs-lookup"><span data-stu-id="9a09a-105">Represents on-premises published resource.</span></span> <span data-ttu-id="9a09a-106">租户管理员可以发布各种类型的本地资源-企业应用程序、域控制器、服务器等。可以将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理特定的已发布资源的请求。</span><span class="sxs-lookup"><span data-stu-id="9a09a-106">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="9a09a-107">Methods</span><span class="sxs-lookup"><span data-stu-id="9a09a-107">Methods</span></span>

| <span data-ttu-id="9a09a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9a09a-108">Method</span></span>       | <span data-ttu-id="9a09a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a09a-109">Return Type</span></span> | <span data-ttu-id="9a09a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a09a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9a09a-111">列出 publishedResources</span><span class="sxs-lookup"><span data-stu-id="9a09a-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="9a09a-112">[publishedResource](publishedresource.md)对象集合</span><span class="sxs-lookup"><span data-stu-id="9a09a-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="9a09a-113">获取**publishedResources**对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a09a-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="9a09a-114">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="9a09a-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="9a09a-116">读取**publishedResource**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a09a-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="9a09a-117">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="9a09a-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="9a09a-119">创建新的**publishedResource**。</span><span class="sxs-lookup"><span data-stu-id="9a09a-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="9a09a-120">更新 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="9a09a-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="9a09a-122">更新**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="9a09a-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="9a09a-123">删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="9a09a-124">无</span><span class="sxs-lookup"><span data-stu-id="9a09a-124">None</span></span> | <span data-ttu-id="9a09a-125">删除**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="9a09a-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="9a09a-126">将 publishedResource 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="9a09a-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="9a09a-127">无</span><span class="sxs-lookup"><span data-stu-id="9a09a-127">None</span></span> | <span data-ttu-id="9a09a-128">将**publishedResource**对象分配给**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="9a09a-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="9a09a-129">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="9a09a-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="9a09a-130">无</span><span class="sxs-lookup"><span data-stu-id="9a09a-130">None</span></span> |  <span data-ttu-id="9a09a-131">从**onPremisesAgentGroup**中删除**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="9a09a-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a09a-132">属性</span><span class="sxs-lookup"><span data-stu-id="9a09a-132">Properties</span></span>

| <span data-ttu-id="9a09a-133">属性</span><span class="sxs-lookup"><span data-stu-id="9a09a-133">Property</span></span>     | <span data-ttu-id="9a09a-134">类型</span><span class="sxs-lookup"><span data-stu-id="9a09a-134">Type</span></span>        | <span data-ttu-id="9a09a-135">说明</span><span class="sxs-lookup"><span data-stu-id="9a09a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a09a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9a09a-136">displayName</span></span>|<span data-ttu-id="9a09a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9a09a-137">String</span></span>| <span data-ttu-id="9a09a-138">PublishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9a09a-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="9a09a-139">id</span><span class="sxs-lookup"><span data-stu-id="9a09a-139">id</span></span>|<span data-ttu-id="9a09a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9a09a-140">String</span></span>| <span data-ttu-id="9a09a-141">PublishedResource 的对象 id。</span><span class="sxs-lookup"><span data-stu-id="9a09a-141">The object id of the publishedResource.</span></span> <span data-ttu-id="9a09a-142">只读。</span><span class="sxs-lookup"><span data-stu-id="9a09a-142">Read-only.</span></span>|
|<span data-ttu-id="9a09a-143">publishingType</span><span class="sxs-lookup"><span data-stu-id="9a09a-143">publishingType</span></span>|<span data-ttu-id="9a09a-144">字符串</span><span class="sxs-lookup"><span data-stu-id="9a09a-144">string</span></span>| <span data-ttu-id="9a09a-145">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="9a09a-145">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="9a09a-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="9a09a-146">resourceName</span></span>|<span data-ttu-id="9a09a-147">String</span><span class="sxs-lookup"><span data-stu-id="9a09a-147">String</span></span>|<span data-ttu-id="9a09a-148">PublishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="9a09a-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a09a-149">关系</span><span class="sxs-lookup"><span data-stu-id="9a09a-149">Relationships</span></span>

| <span data-ttu-id="9a09a-150">关系</span><span class="sxs-lookup"><span data-stu-id="9a09a-150">Relationship</span></span> | <span data-ttu-id="9a09a-151">类型</span><span class="sxs-lookup"><span data-stu-id="9a09a-151">Type</span></span>        | <span data-ttu-id="9a09a-152">说明</span><span class="sxs-lookup"><span data-stu-id="9a09a-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a09a-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="9a09a-153">agentGroups</span></span>|<span data-ttu-id="9a09a-154">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="9a09a-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="9a09a-155">向其分配**publishedResource**的**onPremisesAgentGroups**的列表。</span><span class="sxs-lookup"><span data-stu-id="9a09a-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="9a09a-156">只读。</span><span class="sxs-lookup"><span data-stu-id="9a09a-156">Read-only.</span></span> <span data-ttu-id="9a09a-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9a09a-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a09a-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a09a-158">JSON representation</span></span>

<span data-ttu-id="9a09a-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a09a-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
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
