---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 url。  例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。 其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。 有关这些 Office 365 组资源的详细信息 (包括其关联的资源 url) 现在可以使用组资源类型中的*终结点*导航进行读取。 这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542939"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="87e10-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="87e10-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87e10-108">终结点表示与实体相关联的资源的 url。</span><span class="sxs-lookup"><span data-stu-id="87e10-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="87e10-109">例如, 在创建新的 Office 365 组时, 还会创建其他资源作为 Office 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="87e10-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="87e10-110">其中包括类似于对话的组邮箱和文档和文件的组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="87e10-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="87e10-111">有关这些 Office 365 组资源的详细信息 (包括其关联的资源 url) 现在可以使用组资源类型中的*终结点*导航进行读取。</span><span class="sxs-lookup"><span data-stu-id="87e10-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="87e10-112">这样, 应用程序可以了解这些资源, 甚至可以在自己的体验中嵌入资源 URL 体验。</span><span class="sxs-lookup"><span data-stu-id="87e10-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="87e10-113">方法</span><span class="sxs-lookup"><span data-stu-id="87e10-113">Methods</span></span>

| <span data-ttu-id="87e10-114">方法</span><span class="sxs-lookup"><span data-stu-id="87e10-114">Method</span></span>           | <span data-ttu-id="87e10-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="87e10-115">Return Type</span></span>    |<span data-ttu-id="87e10-116">说明</span><span class="sxs-lookup"><span data-stu-id="87e10-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87e10-117">List endpoints</span><span class="sxs-lookup"><span data-stu-id="87e10-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="87e10-118">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87e10-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="87e10-119">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="87e10-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="87e10-120">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="87e10-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="87e10-121">终结点</span><span class="sxs-lookup"><span data-stu-id="87e10-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="87e10-122">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87e10-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87e10-123">属性</span><span class="sxs-lookup"><span data-stu-id="87e10-123">Properties</span></span>
| <span data-ttu-id="87e10-124">属性</span><span class="sxs-lookup"><span data-stu-id="87e10-124">Property</span></span>     | <span data-ttu-id="87e10-125">类型</span><span class="sxs-lookup"><span data-stu-id="87e10-125">Type</span></span>   |<span data-ttu-id="87e10-126">说明</span><span class="sxs-lookup"><span data-stu-id="87e10-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87e10-127">性能</span><span class="sxs-lookup"><span data-stu-id="87e10-127">capability</span></span>     | <span data-ttu-id="87e10-128">String</span><span class="sxs-lookup"><span data-stu-id="87e10-128">String</span></span>  | <span data-ttu-id="87e10-129">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="87e10-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="87e10-130">(例如, 邮件、对话等) 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="87e10-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="87e10-131">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-131">Read-only.</span></span> |
| <span data-ttu-id="87e10-132">id</span><span class="sxs-lookup"><span data-stu-id="87e10-132">id</span></span>             | <span data-ttu-id="87e10-133">String</span><span class="sxs-lookup"><span data-stu-id="87e10-133">String</span></span>  | <span data-ttu-id="87e10-134">终结点的唯一标识符;主键.</span><span class="sxs-lookup"><span data-stu-id="87e10-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="87e10-135">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="87e10-135">Not nullable.</span></span> <span data-ttu-id="87e10-136">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-136">Read-only.</span></span>|
| <span data-ttu-id="87e10-137">providerId</span><span class="sxs-lookup"><span data-stu-id="87e10-137">providerId</span></span>     | <span data-ttu-id="87e10-138">String</span><span class="sxs-lookup"><span data-stu-id="87e10-138">String</span></span>  | <span data-ttu-id="87e10-139">发布基础服务的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="87e10-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="87e10-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="87e10-140">Not nullable.</span></span> <span data-ttu-id="87e10-141">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-141">Read-only.</span></span>|
| <span data-ttu-id="87e10-142">providerName</span><span class="sxs-lookup"><span data-stu-id="87e10-142">providerName</span></span>   | <span data-ttu-id="87e10-143">String</span><span class="sxs-lookup"><span data-stu-id="87e10-143">String</span></span>  | <span data-ttu-id="87e10-144">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="87e10-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="87e10-145">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-145">Read-only.</span></span>|
| <span data-ttu-id="87e10-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="87e10-146">providerResourceId</span></span>|<span data-ttu-id="87e10-147">String</span><span class="sxs-lookup"><span data-stu-id="87e10-147">String</span></span>| <span data-ttu-id="87e10-148">对于 Office 365 组, 此设置为资源的已知名称 (例如, FeedURL 等)。</span><span class="sxs-lookup"><span data-stu-id="87e10-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="87e10-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="87e10-149">Not nullable.</span></span> <span data-ttu-id="87e10-150">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-150">Read-only.</span></span>|
| <span data-ttu-id="87e10-151">url</span><span class="sxs-lookup"><span data-stu-id="87e10-151">uri</span></span>            | <span data-ttu-id="87e10-152">String</span><span class="sxs-lookup"><span data-stu-id="87e10-152">String</span></span>  | <span data-ttu-id="87e10-153">已发布资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="87e10-153">URL of the published resource.</span></span> <span data-ttu-id="87e10-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="87e10-154">Not nullable.</span></span> <span data-ttu-id="87e10-155">只读。</span><span class="sxs-lookup"><span data-stu-id="87e10-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87e10-156">关系</span><span class="sxs-lookup"><span data-stu-id="87e10-156">Relationships</span></span>

<span data-ttu-id="87e10-157">无。</span><span class="sxs-lookup"><span data-stu-id="87e10-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="87e10-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87e10-158">JSON representation</span></span>
<span data-ttu-id="87e10-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87e10-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
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
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
