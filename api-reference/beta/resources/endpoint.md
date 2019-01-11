---
title: 终结点资源类型
description: '终结点表示与实体相关联的资源的 Url。  例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。 包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。 现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。 这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。 '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871280"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="676fd-107">终结点资源类型</span><span class="sxs-lookup"><span data-stu-id="676fd-107">Endpoint resource type</span></span>

> <span data-ttu-id="676fd-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="676fd-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="676fd-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="676fd-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="676fd-110">终结点表示与实体相关联的资源的 Url。</span><span class="sxs-lookup"><span data-stu-id="676fd-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="676fd-111">例如，创建一个新的 Office 365 组后，其他资源还会创建作为 Office 365 组的一部分。</span><span class="sxs-lookup"><span data-stu-id="676fd-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="676fd-112">包括对话组邮箱和文档和文件组 OneDrive 文件夹等内容。</span><span class="sxs-lookup"><span data-stu-id="676fd-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="676fd-113">现在可以在组资源类型上使用的*终结点*导航读取这些 Office 365 group 资源，包括及其关联的资源的 Url 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="676fd-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="676fd-114">这样，应用程序以了解这些资源，然后甚至他们自己体验中的嵌入 URL 体验的资源。</span><span class="sxs-lookup"><span data-stu-id="676fd-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="676fd-115">方法</span><span class="sxs-lookup"><span data-stu-id="676fd-115">Methods</span></span>

| <span data-ttu-id="676fd-116">方法</span><span class="sxs-lookup"><span data-stu-id="676fd-116">Method</span></span>           | <span data-ttu-id="676fd-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="676fd-117">Return Type</span></span>    |<span data-ttu-id="676fd-118">说明</span><span class="sxs-lookup"><span data-stu-id="676fd-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="676fd-119">列出终结点</span><span class="sxs-lookup"><span data-stu-id="676fd-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="676fd-120">[终结点](endpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="676fd-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="676fd-121">获取一个终结点对象集合。</span><span class="sxs-lookup"><span data-stu-id="676fd-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="676fd-122">获取终结点</span><span class="sxs-lookup"><span data-stu-id="676fd-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="676fd-123">终结点</span><span class="sxs-lookup"><span data-stu-id="676fd-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="676fd-124">读取属性和终结点对象的关系。</span><span class="sxs-lookup"><span data-stu-id="676fd-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="676fd-125">属性</span><span class="sxs-lookup"><span data-stu-id="676fd-125">Properties</span></span>
| <span data-ttu-id="676fd-126">属性</span><span class="sxs-lookup"><span data-stu-id="676fd-126">Property</span></span>     | <span data-ttu-id="676fd-127">类型</span><span class="sxs-lookup"><span data-stu-id="676fd-127">Type</span></span>   |<span data-ttu-id="676fd-128">Description</span><span class="sxs-lookup"><span data-stu-id="676fd-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="676fd-129">功能</span><span class="sxs-lookup"><span data-stu-id="676fd-129">capability</span></span>     | <span data-ttu-id="676fd-130">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-130">String</span></span>  | <span data-ttu-id="676fd-131">介绍与此资源相关联的功能。</span><span class="sxs-lookup"><span data-stu-id="676fd-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="676fd-132">（如邮件、 对话等） 不可为空。</span><span class="sxs-lookup"><span data-stu-id="676fd-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="676fd-133">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="676fd-133">Read-only.</span></span> |
| <span data-ttu-id="676fd-134">id</span><span class="sxs-lookup"><span data-stu-id="676fd-134">id</span></span>             | <span data-ttu-id="676fd-135">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-135">String</span></span>  | <span data-ttu-id="676fd-136">终结点; 的唯一标识符键。</span><span class="sxs-lookup"><span data-stu-id="676fd-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="676fd-137">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="676fd-137">Not nullable.</span></span> <span data-ttu-id="676fd-138">只读。</span><span class="sxs-lookup"><span data-stu-id="676fd-138">Read-only.</span></span>|
| <span data-ttu-id="676fd-139">providerId</span><span class="sxs-lookup"><span data-stu-id="676fd-139">providerId</span></span>     | <span data-ttu-id="676fd-140">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-140">String</span></span>  | <span data-ttu-id="676fd-141">基础服务发布的应用程序 id。</span><span class="sxs-lookup"><span data-stu-id="676fd-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="676fd-142">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="676fd-142">Not nullable.</span></span> <span data-ttu-id="676fd-143">只读。</span><span class="sxs-lookup"><span data-stu-id="676fd-143">Read-only.</span></span>|
| <span data-ttu-id="676fd-144">providerName</span><span class="sxs-lookup"><span data-stu-id="676fd-144">providerName</span></span>   | <span data-ttu-id="676fd-145">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-145">String</span></span>  | <span data-ttu-id="676fd-146">发布基础服务的名称。</span><span class="sxs-lookup"><span data-stu-id="676fd-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="676fd-147">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="676fd-147">Read-only.</span></span>|
| <span data-ttu-id="676fd-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="676fd-148">providerResourceId</span></span>|<span data-ttu-id="676fd-149">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-149">String</span></span>| <span data-ttu-id="676fd-150">Office 365 组，这是设置为资源 （例如 Yammer.FeedURL 等。） 的已知名称。</span><span class="sxs-lookup"><span data-stu-id="676fd-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="676fd-151">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="676fd-151">Not nullable.</span></span> <span data-ttu-id="676fd-152">只读。</span><span class="sxs-lookup"><span data-stu-id="676fd-152">Read-only.</span></span>|
| <span data-ttu-id="676fd-153">uri</span><span class="sxs-lookup"><span data-stu-id="676fd-153">uri</span></span>            | <span data-ttu-id="676fd-154">字符串</span><span class="sxs-lookup"><span data-stu-id="676fd-154">String</span></span>  | <span data-ttu-id="676fd-155">已发布的资源的 URL。</span><span class="sxs-lookup"><span data-stu-id="676fd-155">URL of the published resource.</span></span> <span data-ttu-id="676fd-156">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="676fd-156">Not nullable.</span></span> <span data-ttu-id="676fd-157">只读。</span><span class="sxs-lookup"><span data-stu-id="676fd-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="676fd-158">Relationships</span><span class="sxs-lookup"><span data-stu-id="676fd-158">Relationships</span></span>

<span data-ttu-id="676fd-159">无。</span><span class="sxs-lookup"><span data-stu-id="676fd-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="676fd-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="676fd-160">JSON representation</span></span>
<span data-ttu-id="676fd-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="676fd-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
