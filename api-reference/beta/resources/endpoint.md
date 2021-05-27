---
title: 终结点资源类型
description: 终结点表示与实体关联的资源的 URL。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: groups
author: Jordanndahl
ms.openlocfilehash: 1b5c9f401a659f1461cb9c2185dd412154dbeeda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680407"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="514f2-103">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="514f2-103">Endpoint resource type</span></span>

<span data-ttu-id="514f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="514f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514f2-105">终结点表示与实体关联的资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="514f2-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="514f2-106">例如，当新建Microsoft 365组时，其他资源也会创建为组Microsoft 365的一部分。</span><span class="sxs-lookup"><span data-stu-id="514f2-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="514f2-107">其中包括对话的组邮箱和文档OneDrive文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="514f2-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="514f2-108">有关这些资源Microsoft 365，包括其关联的资源 URL）现在可以使用组资源类型上的终结点导航进行读取。 </span><span class="sxs-lookup"><span data-stu-id="514f2-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="514f2-109">这使应用程序能够了解这些资源，甚至可以在其自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="514f2-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="514f2-110">方法</span><span class="sxs-lookup"><span data-stu-id="514f2-110">Methods</span></span>

| <span data-ttu-id="514f2-111">方法</span><span class="sxs-lookup"><span data-stu-id="514f2-111">Method</span></span>           | <span data-ttu-id="514f2-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="514f2-112">Return Type</span></span>    |<span data-ttu-id="514f2-113">说明</span><span class="sxs-lookup"><span data-stu-id="514f2-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="514f2-114">List endpoints</span><span class="sxs-lookup"><span data-stu-id="514f2-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="514f2-115">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="514f2-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="514f2-116">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="514f2-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="514f2-117">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="514f2-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="514f2-118">终结点</span><span class="sxs-lookup"><span data-stu-id="514f2-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="514f2-119">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="514f2-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="514f2-120">属性</span><span class="sxs-lookup"><span data-stu-id="514f2-120">Properties</span></span>
| <span data-ttu-id="514f2-121">属性</span><span class="sxs-lookup"><span data-stu-id="514f2-121">Property</span></span>     | <span data-ttu-id="514f2-122">类型</span><span class="sxs-lookup"><span data-stu-id="514f2-122">Type</span></span>   |<span data-ttu-id="514f2-123">说明</span><span class="sxs-lookup"><span data-stu-id="514f2-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="514f2-124">capability</span><span class="sxs-lookup"><span data-stu-id="514f2-124">capability</span></span>     | <span data-ttu-id="514f2-125">String</span><span class="sxs-lookup"><span data-stu-id="514f2-125">String</span></span>  | <span data-ttu-id="514f2-126">描述与此资源关联的功能。</span><span class="sxs-lookup"><span data-stu-id="514f2-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="514f2-127"> (，例如消息、对话等) 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="514f2-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="514f2-128">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-128">Read-only.</span></span> |
| <span data-ttu-id="514f2-129">id</span><span class="sxs-lookup"><span data-stu-id="514f2-129">id</span></span>             | <span data-ttu-id="514f2-130">String</span><span class="sxs-lookup"><span data-stu-id="514f2-130">String</span></span>  | <span data-ttu-id="514f2-131">终结点的唯一标识符;键。</span><span class="sxs-lookup"><span data-stu-id="514f2-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="514f2-132">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="514f2-132">Not nullable.</span></span> <span data-ttu-id="514f2-133">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-133">Read-only.</span></span>|
| <span data-ttu-id="514f2-134">providerId</span><span class="sxs-lookup"><span data-stu-id="514f2-134">providerId</span></span>     | <span data-ttu-id="514f2-135">String</span><span class="sxs-lookup"><span data-stu-id="514f2-135">String</span></span>  | <span data-ttu-id="514f2-136">发布基础服务的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="514f2-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="514f2-137">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="514f2-137">Not nullable.</span></span> <span data-ttu-id="514f2-138">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-138">Read-only.</span></span>|
| <span data-ttu-id="514f2-139">providerName</span><span class="sxs-lookup"><span data-stu-id="514f2-139">providerName</span></span>   | <span data-ttu-id="514f2-140">String</span><span class="sxs-lookup"><span data-stu-id="514f2-140">String</span></span>  | <span data-ttu-id="514f2-141">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="514f2-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="514f2-142">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-142">Read-only.</span></span>|
| <span data-ttu-id="514f2-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="514f2-143">providerResourceId</span></span>|<span data-ttu-id="514f2-144">String</span><span class="sxs-lookup"><span data-stu-id="514f2-144">String</span></span>| <span data-ttu-id="514f2-145">对于Microsoft 365组，此名称设置为资源组的已知名称 (例如Yammer。FeedURL 等) 。</span><span class="sxs-lookup"><span data-stu-id="514f2-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="514f2-146">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="514f2-146">Not nullable.</span></span> <span data-ttu-id="514f2-147">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-147">Read-only.</span></span>|
| <span data-ttu-id="514f2-148">uri</span><span class="sxs-lookup"><span data-stu-id="514f2-148">uri</span></span>            | <span data-ttu-id="514f2-149">String</span><span class="sxs-lookup"><span data-stu-id="514f2-149">String</span></span>  | <span data-ttu-id="514f2-150">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="514f2-150">URL of the published resource.</span></span> <span data-ttu-id="514f2-151">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="514f2-151">Not nullable.</span></span> <span data-ttu-id="514f2-152">只读。</span><span class="sxs-lookup"><span data-stu-id="514f2-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="514f2-153">关系</span><span class="sxs-lookup"><span data-stu-id="514f2-153">Relationships</span></span>

<span data-ttu-id="514f2-154">无。</span><span class="sxs-lookup"><span data-stu-id="514f2-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="514f2-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="514f2-155">JSON representation</span></span>
<span data-ttu-id="514f2-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="514f2-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


