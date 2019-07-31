---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Office 365 组资源的详细信息 (包括其关联的资源 Url) 现在可以使用组资源类型中的*终结点*导航进行读取。 这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: db9904c4c668ff86e56be85835c2752ab0d17525
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972122"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="299c3-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="299c3-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="299c3-108">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="299c3-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="299c3-109">例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="299c3-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="299c3-110">其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="299c3-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="299c3-111">有关这些 Office 365 组资源的详细信息 (包括其关联的资源 Url) 现在可以使用组资源类型中的*终结点*导航进行读取。</span><span class="sxs-lookup"><span data-stu-id="299c3-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="299c3-112">这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="299c3-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="299c3-113">方法</span><span class="sxs-lookup"><span data-stu-id="299c3-113">Methods</span></span>

| <span data-ttu-id="299c3-114">方法</span><span class="sxs-lookup"><span data-stu-id="299c3-114">Method</span></span>           | <span data-ttu-id="299c3-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="299c3-115">Return Type</span></span>    |<span data-ttu-id="299c3-116">说明</span><span class="sxs-lookup"><span data-stu-id="299c3-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="299c3-117">List endpoints</span><span class="sxs-lookup"><span data-stu-id="299c3-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="299c3-118">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="299c3-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="299c3-119">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="299c3-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="299c3-120">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="299c3-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="299c3-121">终结点</span><span class="sxs-lookup"><span data-stu-id="299c3-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="299c3-122">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="299c3-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="299c3-123">属性</span><span class="sxs-lookup"><span data-stu-id="299c3-123">Properties</span></span>
| <span data-ttu-id="299c3-124">属性</span><span class="sxs-lookup"><span data-stu-id="299c3-124">Property</span></span>     | <span data-ttu-id="299c3-125">类型</span><span class="sxs-lookup"><span data-stu-id="299c3-125">Type</span></span>   |<span data-ttu-id="299c3-126">说明</span><span class="sxs-lookup"><span data-stu-id="299c3-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="299c3-127">性能</span><span class="sxs-lookup"><span data-stu-id="299c3-127">capability</span></span>     | <span data-ttu-id="299c3-128">String</span><span class="sxs-lookup"><span data-stu-id="299c3-128">String</span></span>  | <span data-ttu-id="299c3-129">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="299c3-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="299c3-130">(例如, 邮件、对话等) 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="299c3-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="299c3-131">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-131">Read-only.</span></span> |
| <span data-ttu-id="299c3-132">id</span><span class="sxs-lookup"><span data-stu-id="299c3-132">id</span></span>             | <span data-ttu-id="299c3-133">String</span><span class="sxs-lookup"><span data-stu-id="299c3-133">String</span></span>  | <span data-ttu-id="299c3-134">终结点的唯一标识符;主键.</span><span class="sxs-lookup"><span data-stu-id="299c3-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="299c3-135">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="299c3-135">Not nullable.</span></span> <span data-ttu-id="299c3-136">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-136">Read-only.</span></span>|
| <span data-ttu-id="299c3-137">providerId</span><span class="sxs-lookup"><span data-stu-id="299c3-137">providerId</span></span>     | <span data-ttu-id="299c3-138">String</span><span class="sxs-lookup"><span data-stu-id="299c3-138">String</span></span>  | <span data-ttu-id="299c3-139">发布基础服务的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="299c3-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="299c3-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="299c3-140">Not nullable.</span></span> <span data-ttu-id="299c3-141">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-141">Read-only.</span></span>|
| <span data-ttu-id="299c3-142">providerName</span><span class="sxs-lookup"><span data-stu-id="299c3-142">providerName</span></span>   | <span data-ttu-id="299c3-143">String</span><span class="sxs-lookup"><span data-stu-id="299c3-143">String</span></span>  | <span data-ttu-id="299c3-144">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="299c3-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="299c3-145">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-145">Read-only.</span></span>|
| <span data-ttu-id="299c3-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="299c3-146">providerResourceId</span></span>|<span data-ttu-id="299c3-147">String</span><span class="sxs-lookup"><span data-stu-id="299c3-147">String</span></span>| <span data-ttu-id="299c3-148">对于 Office 365 组, 此设置为资源的已知名称 (例如, FeedURL 等)。</span><span class="sxs-lookup"><span data-stu-id="299c3-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="299c3-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="299c3-149">Not nullable.</span></span> <span data-ttu-id="299c3-150">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-150">Read-only.</span></span>|
| <span data-ttu-id="299c3-151">url</span><span class="sxs-lookup"><span data-stu-id="299c3-151">uri</span></span>            | <span data-ttu-id="299c3-152">String</span><span class="sxs-lookup"><span data-stu-id="299c3-152">String</span></span>  | <span data-ttu-id="299c3-153">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="299c3-153">URL of the published resource.</span></span> <span data-ttu-id="299c3-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="299c3-154">Not nullable.</span></span> <span data-ttu-id="299c3-155">只读。</span><span class="sxs-lookup"><span data-stu-id="299c3-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="299c3-156">关系</span><span class="sxs-lookup"><span data-stu-id="299c3-156">Relationships</span></span>

<span data-ttu-id="299c3-157">无。</span><span class="sxs-lookup"><span data-stu-id="299c3-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="299c3-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="299c3-158">JSON representation</span></span>
<span data-ttu-id="299c3-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="299c3-159">Here is a JSON representation of the resource.</span></span>

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
