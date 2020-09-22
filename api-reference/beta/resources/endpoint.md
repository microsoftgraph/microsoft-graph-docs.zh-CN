---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的 *终结点* 导航进行读取。 这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: 683ef1140105666d96c83249876266db204b1b47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979423"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="f9dbf-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="f9dbf-107">Endpoint resource type</span></span>

<span data-ttu-id="f9dbf-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9dbf-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9dbf-109">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-109">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="f9dbf-110">例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-110">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="f9dbf-111">其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-111">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="f9dbf-112">有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的 *终结点* 导航进行读取。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-112">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="f9dbf-113">这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-113">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="f9dbf-114">方法</span><span class="sxs-lookup"><span data-stu-id="f9dbf-114">Methods</span></span>

| <span data-ttu-id="f9dbf-115">方法</span><span class="sxs-lookup"><span data-stu-id="f9dbf-115">Method</span></span>           | <span data-ttu-id="f9dbf-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9dbf-116">Return Type</span></span>    |<span data-ttu-id="f9dbf-117">说明</span><span class="sxs-lookup"><span data-stu-id="f9dbf-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f9dbf-118">List endpoints</span><span class="sxs-lookup"><span data-stu-id="f9dbf-118">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="f9dbf-119">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f9dbf-119">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="f9dbf-120">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-120">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="f9dbf-121">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="f9dbf-121">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="f9dbf-122">终结点</span><span class="sxs-lookup"><span data-stu-id="f9dbf-122">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="f9dbf-123">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-123">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9dbf-124">属性</span><span class="sxs-lookup"><span data-stu-id="f9dbf-124">Properties</span></span>
| <span data-ttu-id="f9dbf-125">属性</span><span class="sxs-lookup"><span data-stu-id="f9dbf-125">Property</span></span>     | <span data-ttu-id="f9dbf-126">类型</span><span class="sxs-lookup"><span data-stu-id="f9dbf-126">Type</span></span>   |<span data-ttu-id="f9dbf-127">说明</span><span class="sxs-lookup"><span data-stu-id="f9dbf-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9dbf-128">性能</span><span class="sxs-lookup"><span data-stu-id="f9dbf-128">capability</span></span>     | <span data-ttu-id="f9dbf-129">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-129">String</span></span>  | <span data-ttu-id="f9dbf-130">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-130">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="f9dbf-131"> (，例如邮件、对话等 ) 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-131">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="f9dbf-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-132">Read-only.</span></span> |
| <span data-ttu-id="f9dbf-133">id</span><span class="sxs-lookup"><span data-stu-id="f9dbf-133">id</span></span>             | <span data-ttu-id="f9dbf-134">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-134">String</span></span>  | <span data-ttu-id="f9dbf-135">终结点的唯一标识符;主键.</span><span class="sxs-lookup"><span data-stu-id="f9dbf-135">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="f9dbf-136">不可为空。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-136">Not nullable.</span></span> <span data-ttu-id="f9dbf-137">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-137">Read-only.</span></span>|
| <span data-ttu-id="f9dbf-138">providerId</span><span class="sxs-lookup"><span data-stu-id="f9dbf-138">providerId</span></span>     | <span data-ttu-id="f9dbf-139">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-139">String</span></span>  | <span data-ttu-id="f9dbf-140">发布基础服务的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-140">Application id of the publishing underlying service.</span></span> <span data-ttu-id="f9dbf-141">不可为空。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-141">Not nullable.</span></span> <span data-ttu-id="f9dbf-142">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-142">Read-only.</span></span>|
| <span data-ttu-id="f9dbf-143">providerName</span><span class="sxs-lookup"><span data-stu-id="f9dbf-143">providerName</span></span>   | <span data-ttu-id="f9dbf-144">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-144">String</span></span>  | <span data-ttu-id="f9dbf-145">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-145">Name of the publishing underlying service.</span></span> <span data-ttu-id="f9dbf-146">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-146">Read-only.</span></span>|
| <span data-ttu-id="f9dbf-147">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="f9dbf-147">providerResourceId</span></span>|<span data-ttu-id="f9dbf-148">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-148">String</span></span>| <span data-ttu-id="f9dbf-149">对于 Microsoft 365 组，它设置为资源的已知名称 (例如，FeedURL 等 ) 。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-149">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="f9dbf-150">不可为空。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-150">Not nullable.</span></span> <span data-ttu-id="f9dbf-151">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-151">Read-only.</span></span>|
| <span data-ttu-id="f9dbf-152">url</span><span class="sxs-lookup"><span data-stu-id="f9dbf-152">uri</span></span>            | <span data-ttu-id="f9dbf-153">String</span><span class="sxs-lookup"><span data-stu-id="f9dbf-153">String</span></span>  | <span data-ttu-id="f9dbf-154">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-154">URL of the published resource.</span></span> <span data-ttu-id="f9dbf-155">不可为空。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-155">Not nullable.</span></span> <span data-ttu-id="f9dbf-156">只读。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9dbf-157">关系</span><span class="sxs-lookup"><span data-stu-id="f9dbf-157">Relationships</span></span>

<span data-ttu-id="f9dbf-158">无。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f9dbf-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9dbf-159">JSON representation</span></span>
<span data-ttu-id="f9dbf-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9dbf-160">Here is a JSON representation of the resource.</span></span>

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


