---
title: 终结点资源类型
description: 终结点表示与实体相关联的资源的 Url。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 43843a3b6847c261326574e7a73f607b10e5e05d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895613"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="79796-103">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="79796-103">Endpoint resource type</span></span>

<span data-ttu-id="79796-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79796-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79796-105">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="79796-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="79796-106">例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="79796-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="79796-107">其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="79796-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="79796-108">有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的*终结点*导航进行读取。</span><span class="sxs-lookup"><span data-stu-id="79796-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="79796-109">这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="79796-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="79796-110">方法</span><span class="sxs-lookup"><span data-stu-id="79796-110">Methods</span></span>

| <span data-ttu-id="79796-111">方法</span><span class="sxs-lookup"><span data-stu-id="79796-111">Method</span></span>           | <span data-ttu-id="79796-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="79796-112">Return Type</span></span>    |<span data-ttu-id="79796-113">说明</span><span class="sxs-lookup"><span data-stu-id="79796-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79796-114">List endpoints</span><span class="sxs-lookup"><span data-stu-id="79796-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="79796-115">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79796-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="79796-116">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="79796-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="79796-117">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="79796-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="79796-118">终结点</span><span class="sxs-lookup"><span data-stu-id="79796-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="79796-119">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79796-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79796-120">属性</span><span class="sxs-lookup"><span data-stu-id="79796-120">Properties</span></span>
| <span data-ttu-id="79796-121">属性</span><span class="sxs-lookup"><span data-stu-id="79796-121">Property</span></span>     | <span data-ttu-id="79796-122">类型</span><span class="sxs-lookup"><span data-stu-id="79796-122">Type</span></span>   |<span data-ttu-id="79796-123">说明</span><span class="sxs-lookup"><span data-stu-id="79796-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79796-124">性能</span><span class="sxs-lookup"><span data-stu-id="79796-124">capability</span></span>     | <span data-ttu-id="79796-125">String</span><span class="sxs-lookup"><span data-stu-id="79796-125">String</span></span>  | <span data-ttu-id="79796-126">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="79796-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="79796-127">（例如，邮件、对话等） 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="79796-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="79796-128">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-128">Read-only.</span></span> |
| <span data-ttu-id="79796-129">id</span><span class="sxs-lookup"><span data-stu-id="79796-129">id</span></span>             | <span data-ttu-id="79796-130">String</span><span class="sxs-lookup"><span data-stu-id="79796-130">String</span></span>  | <span data-ttu-id="79796-131">终结点的唯一标识符;主键.</span><span class="sxs-lookup"><span data-stu-id="79796-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="79796-132">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="79796-132">Not nullable.</span></span> <span data-ttu-id="79796-133">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-133">Read-only.</span></span>|
| <span data-ttu-id="79796-134">providerId</span><span class="sxs-lookup"><span data-stu-id="79796-134">providerId</span></span>     | <span data-ttu-id="79796-135">String</span><span class="sxs-lookup"><span data-stu-id="79796-135">String</span></span>  | <span data-ttu-id="79796-136">发布基础服务的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="79796-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="79796-137">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="79796-137">Not nullable.</span></span> <span data-ttu-id="79796-138">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-138">Read-only.</span></span>|
| <span data-ttu-id="79796-139">providerName</span><span class="sxs-lookup"><span data-stu-id="79796-139">providerName</span></span>   | <span data-ttu-id="79796-140">String</span><span class="sxs-lookup"><span data-stu-id="79796-140">String</span></span>  | <span data-ttu-id="79796-141">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="79796-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="79796-142">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-142">Read-only.</span></span>|
| <span data-ttu-id="79796-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="79796-143">providerResourceId</span></span>|<span data-ttu-id="79796-144">String</span><span class="sxs-lookup"><span data-stu-id="79796-144">String</span></span>| <span data-ttu-id="79796-145">对于 Microsoft 365 组，此设置为资源的已知名称（例如，FeedURL 等）。</span><span class="sxs-lookup"><span data-stu-id="79796-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="79796-146">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="79796-146">Not nullable.</span></span> <span data-ttu-id="79796-147">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-147">Read-only.</span></span>|
| <span data-ttu-id="79796-148">url</span><span class="sxs-lookup"><span data-stu-id="79796-148">uri</span></span>            | <span data-ttu-id="79796-149">String</span><span class="sxs-lookup"><span data-stu-id="79796-149">String</span></span>  | <span data-ttu-id="79796-150">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="79796-150">URL of the published resource.</span></span> <span data-ttu-id="79796-151">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="79796-151">Not nullable.</span></span> <span data-ttu-id="79796-152">只读。</span><span class="sxs-lookup"><span data-stu-id="79796-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79796-153">关系</span><span class="sxs-lookup"><span data-stu-id="79796-153">Relationships</span></span>

<span data-ttu-id="79796-154">无。</span><span class="sxs-lookup"><span data-stu-id="79796-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="79796-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79796-155">JSON representation</span></span>
<span data-ttu-id="79796-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79796-156">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
     "Error: microsoft.graph.servicePrincipal/endpoints:\r\n      Referenced type microsoft.graph.endPoint is not defined in the doc  set! Potential suggestion: microsoft.graph.callRecords.endpoint"
    ]
}
-->
