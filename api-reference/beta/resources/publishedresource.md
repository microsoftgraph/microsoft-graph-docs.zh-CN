---
title: publishedResource 资源类型
description: publishedResource 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841358"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="2bcfe-103">publishedResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bcfe-103">publishedResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcfe-104">表示本地发布的资源。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-104">Represents on-premises published resource.</span></span> <span data-ttu-id="2bcfe-105">租户管理员可以发布各种类型的本地资源-企业应用程序、域控制器、服务器等。可以将租户管理员安装的[本地代理](onpremisesagent.md)配置为访问/处理请求特定的已发布资源。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-105">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="2bcfe-106">方法</span><span class="sxs-lookup"><span data-stu-id="2bcfe-106">Methods</span></span>

| <span data-ttu-id="2bcfe-107">方法</span><span class="sxs-lookup"><span data-stu-id="2bcfe-107">Method</span></span>       | <span data-ttu-id="2bcfe-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bcfe-108">Return Type</span></span> | <span data-ttu-id="2bcfe-109">说明</span><span class="sxs-lookup"><span data-stu-id="2bcfe-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2bcfe-110">列出 publishedResources</span><span class="sxs-lookup"><span data-stu-id="2bcfe-110">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="2bcfe-111">[publishedResource](publishedresource.md)对象集合</span><span class="sxs-lookup"><span data-stu-id="2bcfe-111">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="2bcfe-112">获取**publishedResources**对象集合。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-112">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="2bcfe-113">获取 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-113">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="2bcfe-114">publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-114">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="2bcfe-115">读取**publishedResource**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-115">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="2bcfe-116">创建 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-116">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="2bcfe-117">publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-117">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="2bcfe-118">创建新的**publishedResource**。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-118">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="2bcfe-119">更新 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-119">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="2bcfe-120">publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-120">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="2bcfe-121">更新**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-121">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="2bcfe-122">删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-122">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="2bcfe-123">无</span><span class="sxs-lookup"><span data-stu-id="2bcfe-123">None</span></span> | <span data-ttu-id="2bcfe-124">删除**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-124">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="2bcfe-125">将 publishedResource 分配给 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="2bcfe-125">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="2bcfe-126">无</span><span class="sxs-lookup"><span data-stu-id="2bcfe-126">None</span></span> | <span data-ttu-id="2bcfe-127">将**publishedResource**对象分配给**onPremisesAgentGroup**。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-127">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="2bcfe-128">从 onPremisesAgentGroup 中删除 publishedResource</span><span class="sxs-lookup"><span data-stu-id="2bcfe-128">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="2bcfe-129">无</span><span class="sxs-lookup"><span data-stu-id="2bcfe-129">None</span></span> |  <span data-ttu-id="2bcfe-130">从**onPremisesAgentGroup**中删除**publishedResource**对象。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-130">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="2bcfe-131">属性</span><span class="sxs-lookup"><span data-stu-id="2bcfe-131">Properties</span></span>

| <span data-ttu-id="2bcfe-132">属性</span><span class="sxs-lookup"><span data-stu-id="2bcfe-132">Property</span></span>     | <span data-ttu-id="2bcfe-133">类型</span><span class="sxs-lookup"><span data-stu-id="2bcfe-133">Type</span></span>        | <span data-ttu-id="2bcfe-134">说明</span><span class="sxs-lookup"><span data-stu-id="2bcfe-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcfe-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2bcfe-135">displayName</span></span>|<span data-ttu-id="2bcfe-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2bcfe-136">String</span></span>| <span data-ttu-id="2bcfe-137">PublishedResource 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-137">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="2bcfe-138">id</span><span class="sxs-lookup"><span data-stu-id="2bcfe-138">id</span></span>|<span data-ttu-id="2bcfe-139">String</span><span class="sxs-lookup"><span data-stu-id="2bcfe-139">String</span></span>| <span data-ttu-id="2bcfe-140">PublishedResource 的对象 id。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-140">The object id of the publishedResource.</span></span> <span data-ttu-id="2bcfe-141">只读。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-141">Read-only.</span></span>|
|<span data-ttu-id="2bcfe-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="2bcfe-142">publishingType</span></span>|<span data-ttu-id="2bcfe-143">string</span><span class="sxs-lookup"><span data-stu-id="2bcfe-143">string</span></span>| <span data-ttu-id="2bcfe-144">可取值为：`appProxy`、`exchangeOnline`、`authentication`、`provisioning`、`adAdministration`。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="2bcfe-145">resourceName</span><span class="sxs-lookup"><span data-stu-id="2bcfe-145">resourceName</span></span>|<span data-ttu-id="2bcfe-146">String</span><span class="sxs-lookup"><span data-stu-id="2bcfe-146">String</span></span>|<span data-ttu-id="2bcfe-147">PublishedResource 的名称。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-147">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bcfe-148">关系</span><span class="sxs-lookup"><span data-stu-id="2bcfe-148">Relationships</span></span>

| <span data-ttu-id="2bcfe-149">关系</span><span class="sxs-lookup"><span data-stu-id="2bcfe-149">Relationship</span></span> | <span data-ttu-id="2bcfe-150">类型</span><span class="sxs-lookup"><span data-stu-id="2bcfe-150">Type</span></span>        | <span data-ttu-id="2bcfe-151">说明</span><span class="sxs-lookup"><span data-stu-id="2bcfe-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2bcfe-152">agentGroups</span><span class="sxs-lookup"><span data-stu-id="2bcfe-152">agentGroups</span></span>|<span data-ttu-id="2bcfe-153">[onPremisesAgentGroup](onpremisesagentgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="2bcfe-153">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="2bcfe-154">向其分配**publishedResource**的**onPremisesAgentGroups**的列表。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-154">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="2bcfe-155">只读。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-155">Read-only.</span></span> <span data-ttu-id="2bcfe-156">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bcfe-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bcfe-157">JSON representation</span></span>

<span data-ttu-id="2bcfe-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bcfe-158">The following is a JSON representation of the resource.</span></span>

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
