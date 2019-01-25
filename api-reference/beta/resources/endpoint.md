---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512057"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="751c0-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="751c0-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="751c0-108">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="751c0-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="751c0-109">例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="751c0-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="751c0-110">包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="751c0-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="751c0-111">现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="751c0-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="751c0-112">这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。</span><span class="sxs-lookup"><span data-stu-id="751c0-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="751c0-113">方法</span><span class="sxs-lookup"><span data-stu-id="751c0-113">Methods</span></span>

| <span data-ttu-id="751c0-114">方法</span><span class="sxs-lookup"><span data-stu-id="751c0-114">Method</span></span>           | <span data-ttu-id="751c0-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="751c0-115">Return Type</span></span>    |<span data-ttu-id="751c0-116">说明</span><span class="sxs-lookup"><span data-stu-id="751c0-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="751c0-117">List endpoints</span><span class="sxs-lookup"><span data-stu-id="751c0-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="751c0-118">[Endpoint](endpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="751c0-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="751c0-119">获取 endpoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="751c0-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="751c0-120">Get endpoint</span><span class="sxs-lookup"><span data-stu-id="751c0-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="751c0-121">终结点</span><span class="sxs-lookup"><span data-stu-id="751c0-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="751c0-122">读取 endpoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="751c0-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="751c0-123">属性</span><span class="sxs-lookup"><span data-stu-id="751c0-123">Properties</span></span>
| <span data-ttu-id="751c0-124">属性</span><span class="sxs-lookup"><span data-stu-id="751c0-124">Property</span></span>     | <span data-ttu-id="751c0-125">类型</span><span class="sxs-lookup"><span data-stu-id="751c0-125">Type</span></span>   |<span data-ttu-id="751c0-126">说明</span><span class="sxs-lookup"><span data-stu-id="751c0-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="751c0-127">Capability</span><span class="sxs-lookup"><span data-stu-id="751c0-127">capability</span></span>     | <span data-ttu-id="751c0-128">String</span><span class="sxs-lookup"><span data-stu-id="751c0-128">String</span></span>  | <span data-ttu-id="751c0-129">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="751c0-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="751c0-130">（如邮件、 对话等） 不可为空。</span><span class="sxs-lookup"><span data-stu-id="751c0-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="751c0-131">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-131">Read-only.</span></span> |
| <span data-ttu-id="751c0-132">id</span><span class="sxs-lookup"><span data-stu-id="751c0-132">id</span></span>             | <span data-ttu-id="751c0-133">String</span><span class="sxs-lookup"><span data-stu-id="751c0-133">String</span></span>  | <span data-ttu-id="751c0-134">终结点; 的唯一标识符键。</span><span class="sxs-lookup"><span data-stu-id="751c0-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="751c0-135">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="751c0-135">Not nullable.</span></span> <span data-ttu-id="751c0-136">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-136">Read-only.</span></span>|
| <span data-ttu-id="751c0-137">ProviderID</span><span class="sxs-lookup"><span data-stu-id="751c0-137">providerId</span></span>     | <span data-ttu-id="751c0-138">String</span><span class="sxs-lookup"><span data-stu-id="751c0-138">String</span></span>  | <span data-ttu-id="751c0-139">基础服务发布的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="751c0-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="751c0-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="751c0-140">Not nullable.</span></span> <span data-ttu-id="751c0-141">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-141">Read-only.</span></span>|
| <span data-ttu-id="751c0-142">ProviderName</span><span class="sxs-lookup"><span data-stu-id="751c0-142">providerName</span></span>   | <span data-ttu-id="751c0-143">String</span><span class="sxs-lookup"><span data-stu-id="751c0-143">String</span></span>  | <span data-ttu-id="751c0-144">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="751c0-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="751c0-145">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-145">Read-only.</span></span>|
| <span data-ttu-id="751c0-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="751c0-146">providerResourceId</span></span>|<span data-ttu-id="751c0-147">String</span><span class="sxs-lookup"><span data-stu-id="751c0-147">String</span></span>| <span data-ttu-id="751c0-148">Office 365 组，这是设置为资源 （例如 Yammer.FeedURL 等。） 的已知名称。</span><span class="sxs-lookup"><span data-stu-id="751c0-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="751c0-149">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="751c0-149">Not nullable.</span></span> <span data-ttu-id="751c0-150">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-150">Read-only.</span></span>|
| <span data-ttu-id="751c0-151">uri</span><span class="sxs-lookup"><span data-stu-id="751c0-151">uri</span></span>            | <span data-ttu-id="751c0-152">String</span><span class="sxs-lookup"><span data-stu-id="751c0-152">String</span></span>  | <span data-ttu-id="751c0-153">已发布的资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="751c0-153">URL of the published resource.</span></span> <span data-ttu-id="751c0-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="751c0-154">Not nullable.</span></span> <span data-ttu-id="751c0-155">只读。</span><span class="sxs-lookup"><span data-stu-id="751c0-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="751c0-156">关系</span><span class="sxs-lookup"><span data-stu-id="751c0-156">Relationships</span></span>

<span data-ttu-id="751c0-157">无。</span><span class="sxs-lookup"><span data-stu-id="751c0-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="751c0-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="751c0-158">JSON representation</span></span>
<span data-ttu-id="751c0-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="751c0-159">Here is a JSON representation of the resource.</span></span>

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
