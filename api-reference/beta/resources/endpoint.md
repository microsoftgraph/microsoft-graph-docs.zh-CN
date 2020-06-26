---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的*终结点*导航进行读取。 这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 77a0ddc0a91f1269ed5e62393c32b85af49264aa
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44893849"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="96c15-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="96c15-107">Endpoint resource type</span></span>

<span data-ttu-id="96c15-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96c15-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96c15-109">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="96c15-109">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="96c15-110">例如，在创建新的 Microsoft 365 组时，还会创建其他资源作为 Microsoft 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="96c15-110">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="96c15-111">其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="96c15-111">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="96c15-112">有关这些 Microsoft 365 组资源的详细信息（包括其关联的资源 Url）现在可以使用组资源类型中的*终结点*导航进行读取。</span><span class="sxs-lookup"><span data-stu-id="96c15-112">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="96c15-113">这样，应用程序可以了解这些资源，甚至可以在自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="96c15-113">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="96c15-114">方法</span><span class="sxs-lookup"><span data-stu-id="96c15-114">Methods</span></span>

| <span data-ttu-id="96c15-115">方法</span><span class="sxs-lookup"><span data-stu-id="96c15-115">Method</span></span>           | <span data-ttu-id="96c15-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="96c15-116">Return Type</span></span>    |<span data-ttu-id="96c15-117">说明</span><span class="sxs-lookup"><span data-stu-id="96c15-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96c15-118">List endpoints</span><span class="sxs-lookup"><span data-stu-id="96c15-118">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="96c15-119">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96c15-119">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="96c15-120">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96c15-120">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="96c15-121">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="96c15-121">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="96c15-122">终结点</span><span class="sxs-lookup"><span data-stu-id="96c15-122">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="96c15-123">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96c15-123">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96c15-124">属性</span><span class="sxs-lookup"><span data-stu-id="96c15-124">Properties</span></span>
| <span data-ttu-id="96c15-125">属性</span><span class="sxs-lookup"><span data-stu-id="96c15-125">Property</span></span>     | <span data-ttu-id="96c15-126">类型</span><span class="sxs-lookup"><span data-stu-id="96c15-126">Type</span></span>   |<span data-ttu-id="96c15-127">说明</span><span class="sxs-lookup"><span data-stu-id="96c15-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96c15-128">性能</span><span class="sxs-lookup"><span data-stu-id="96c15-128">capability</span></span>     | <span data-ttu-id="96c15-129">String</span><span class="sxs-lookup"><span data-stu-id="96c15-129">String</span></span>  | <span data-ttu-id="96c15-130">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="96c15-130">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="96c15-131">（例如，邮件、对话等） 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="96c15-131">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="96c15-132">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-132">Read-only.</span></span> |
| <span data-ttu-id="96c15-133">id</span><span class="sxs-lookup"><span data-stu-id="96c15-133">id</span></span>             | <span data-ttu-id="96c15-134">String</span><span class="sxs-lookup"><span data-stu-id="96c15-134">String</span></span>  | <span data-ttu-id="96c15-135">终结点的唯一标识符;主键.</span><span class="sxs-lookup"><span data-stu-id="96c15-135">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="96c15-136">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="96c15-136">Not nullable.</span></span> <span data-ttu-id="96c15-137">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-137">Read-only.</span></span>|
| <span data-ttu-id="96c15-138">providerId</span><span class="sxs-lookup"><span data-stu-id="96c15-138">providerId</span></span>     | <span data-ttu-id="96c15-139">String</span><span class="sxs-lookup"><span data-stu-id="96c15-139">String</span></span>  | <span data-ttu-id="96c15-140">发布基础服务的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="96c15-140">Application id of the publishing underlying service.</span></span> <span data-ttu-id="96c15-141">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="96c15-141">Not nullable.</span></span> <span data-ttu-id="96c15-142">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-142">Read-only.</span></span>|
| <span data-ttu-id="96c15-143">providerName</span><span class="sxs-lookup"><span data-stu-id="96c15-143">providerName</span></span>   | <span data-ttu-id="96c15-144">String</span><span class="sxs-lookup"><span data-stu-id="96c15-144">String</span></span>  | <span data-ttu-id="96c15-145">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="96c15-145">Name of the publishing underlying service.</span></span> <span data-ttu-id="96c15-146">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-146">Read-only.</span></span>|
| <span data-ttu-id="96c15-147">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="96c15-147">providerResourceId</span></span>|<span data-ttu-id="96c15-148">String</span><span class="sxs-lookup"><span data-stu-id="96c15-148">String</span></span>| <span data-ttu-id="96c15-149">对于 Microsoft 365 组，此设置为资源的已知名称（例如，FeedURL 等）。</span><span class="sxs-lookup"><span data-stu-id="96c15-149">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="96c15-150">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="96c15-150">Not nullable.</span></span> <span data-ttu-id="96c15-151">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-151">Read-only.</span></span>|
| <span data-ttu-id="96c15-152">url</span><span class="sxs-lookup"><span data-stu-id="96c15-152">uri</span></span>            | <span data-ttu-id="96c15-153">String</span><span class="sxs-lookup"><span data-stu-id="96c15-153">String</span></span>  | <span data-ttu-id="96c15-154">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="96c15-154">URL of the published resource.</span></span> <span data-ttu-id="96c15-155">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="96c15-155">Not nullable.</span></span> <span data-ttu-id="96c15-156">只读。</span><span class="sxs-lookup"><span data-stu-id="96c15-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96c15-157">关系</span><span class="sxs-lookup"><span data-stu-id="96c15-157">Relationships</span></span>

<span data-ttu-id="96c15-158">无。</span><span class="sxs-lookup"><span data-stu-id="96c15-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="96c15-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96c15-159">JSON representation</span></span>
<span data-ttu-id="96c15-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96c15-160">Here is a JSON representation of the resource.</span></span>

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
