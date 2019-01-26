---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 '
localization_priority: Normal
ms.openlocfilehash: 39a6a2d8213e809f426c492654272aa994c25a6d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574480"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="603b7-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="603b7-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="603b7-108">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="603b7-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="603b7-109">例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="603b7-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="603b7-110">包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="603b7-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="603b7-111">现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="603b7-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="603b7-112">这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。</span><span class="sxs-lookup"><span data-stu-id="603b7-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="603b7-113">方法</span><span class="sxs-lookup"><span data-stu-id="603b7-113">Methods</span></span>

| <span data-ttu-id="603b7-114">方法</span><span class="sxs-lookup"><span data-stu-id="603b7-114">Method</span></span>           | <span data-ttu-id="603b7-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="603b7-115">Return Type</span></span>    |<span data-ttu-id="603b7-116">说明</span><span class="sxs-lookup"><span data-stu-id="603b7-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="603b7-117">List endpoints</span><span class="sxs-lookup"><span data-stu-id="603b7-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="603b7-118">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="603b7-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="603b7-119">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="603b7-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="603b7-120">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="603b7-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="603b7-121">终结点</span><span class="sxs-lookup"><span data-stu-id="603b7-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="603b7-122">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="603b7-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="603b7-123">属性</span><span class="sxs-lookup"><span data-stu-id="603b7-123">Properties</span></span>
| <span data-ttu-id="603b7-124">属性</span><span class="sxs-lookup"><span data-stu-id="603b7-124">Property</span></span>     | <span data-ttu-id="603b7-125">类型</span><span class="sxs-lookup"><span data-stu-id="603b7-125">Type</span></span>   |<span data-ttu-id="603b7-126">说明</span><span class="sxs-lookup"><span data-stu-id="603b7-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="603b7-127">功能</span><span class="sxs-lookup"><span data-stu-id="603b7-127">capability</span></span>     | <span data-ttu-id="603b7-128">String</span><span class="sxs-lookup"><span data-stu-id="603b7-128">String</span></span>  | <span data-ttu-id="603b7-129">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="603b7-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="603b7-130">（如邮件、 对话等） 不可为空。</span><span class="sxs-lookup"><span data-stu-id="603b7-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="603b7-131">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-131">Read-only.</span></span> |
| <span data-ttu-id="603b7-132">id</span><span class="sxs-lookup"><span data-stu-id="603b7-132">id</span></span>             | <span data-ttu-id="603b7-133">String</span><span class="sxs-lookup"><span data-stu-id="603b7-133">String</span></span>  | <span data-ttu-id="603b7-134">终结点; 的唯一标识符键。</span><span class="sxs-lookup"><span data-stu-id="603b7-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="603b7-135">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="603b7-135">Not nullable.</span></span> <span data-ttu-id="603b7-136">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-136">Read-only.</span></span>|
| <span data-ttu-id="603b7-137">providerId</span><span class="sxs-lookup"><span data-stu-id="603b7-137">providerId</span></span>     | <span data-ttu-id="603b7-138">String</span><span class="sxs-lookup"><span data-stu-id="603b7-138">String</span></span>  | <span data-ttu-id="603b7-139">基础服务发布的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="603b7-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="603b7-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="603b7-140">Not nullable.</span></span> <span data-ttu-id="603b7-141">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-141">Read-only.</span></span>|
| <span data-ttu-id="603b7-142">providerName</span><span class="sxs-lookup"><span data-stu-id="603b7-142">providerName</span></span>   | <span data-ttu-id="603b7-143">String</span><span class="sxs-lookup"><span data-stu-id="603b7-143">String</span></span>  | <span data-ttu-id="603b7-144">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="603b7-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="603b7-145">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-145">Read-only.</span></span>|
| <span data-ttu-id="603b7-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="603b7-146">providerResourceId</span></span>|<span data-ttu-id="603b7-147">String</span><span class="sxs-lookup"><span data-stu-id="603b7-147">String</span></span>| <span data-ttu-id="603b7-148">Office 365 组，这是设置为资源 （例如 Yammer.FeedURL 等。） 的已知名称。</span><span class="sxs-lookup"><span data-stu-id="603b7-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="603b7-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="603b7-149">Not nullable.</span></span> <span data-ttu-id="603b7-150">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-150">Read-only.</span></span>|
| <span data-ttu-id="603b7-151">uri</span><span class="sxs-lookup"><span data-stu-id="603b7-151">uri</span></span>            | <span data-ttu-id="603b7-152">String</span><span class="sxs-lookup"><span data-stu-id="603b7-152">String</span></span>  | <span data-ttu-id="603b7-153">已发布的资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="603b7-153">URL of the published resource.</span></span> <span data-ttu-id="603b7-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="603b7-154">Not nullable.</span></span> <span data-ttu-id="603b7-155">只读。</span><span class="sxs-lookup"><span data-stu-id="603b7-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="603b7-156">关系</span><span class="sxs-lookup"><span data-stu-id="603b7-156">Relationships</span></span>

<span data-ttu-id="603b7-157">无。</span><span class="sxs-lookup"><span data-stu-id="603b7-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="603b7-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="603b7-158">JSON representation</span></span>
<span data-ttu-id="603b7-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="603b7-159">Here is a JSON representation of the resource.</span></span>

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
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
