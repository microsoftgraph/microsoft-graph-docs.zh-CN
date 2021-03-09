---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3519caeade4c50514fb2d725f21b10ff6efcada3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578806"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="99bde-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="99bde-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="99bde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99bde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99bde-105">表示聊天消息中托管的 Teams 内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="99bde-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="99bde-106">[文件附件](chatmessageattachment.md) 不是托管内容;它们存储在 SharePoint 或 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="99bde-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="99bde-107">方法</span><span class="sxs-lookup"><span data-stu-id="99bde-107">Methods</span></span>

| <span data-ttu-id="99bde-108">方法</span><span class="sxs-lookup"><span data-stu-id="99bde-108">Method</span></span>       | <span data-ttu-id="99bde-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="99bde-109">Return Type</span></span> | <span data-ttu-id="99bde-110">说明</span><span class="sxs-lookup"><span data-stu-id="99bde-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="99bde-111">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="99bde-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="99bde-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="99bde-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="99bde-113">检索消息的 **chatMessageHostedContent** 列表。</span><span class="sxs-lookup"><span data-stu-id="99bde-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="99bde-114">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="99bde-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="99bde-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="99bde-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="99bde-116">读取 **chatMessageHostedContent** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99bde-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99bde-117">属性</span><span class="sxs-lookup"><span data-stu-id="99bde-117">Properties</span></span>

<span data-ttu-id="99bde-118">chatMessageHostedContent 派生自 [teamworkHostedContent](teamworkhostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="99bde-118">chatMessageHostedContent derives from [teamworkHostedContent](teamworkhostedcontent.md)</span></span>

| <span data-ttu-id="99bde-119">属性</span><span class="sxs-lookup"><span data-stu-id="99bde-119">Property</span></span>     | <span data-ttu-id="99bde-120">类型</span><span class="sxs-lookup"><span data-stu-id="99bde-120">Type</span></span>        | <span data-ttu-id="99bde-121">说明</span><span class="sxs-lookup"><span data-stu-id="99bde-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99bde-122">id</span><span class="sxs-lookup"><span data-stu-id="99bde-122">id</span></span>            |<span data-ttu-id="99bde-123">字符串</span><span class="sxs-lookup"><span data-stu-id="99bde-123">String</span></span>       | <span data-ttu-id="99bde-124">只读。</span><span class="sxs-lookup"><span data-stu-id="99bde-124">Read-only.</span></span> <span data-ttu-id="99bde-125">表示聊天消息托管的内容标识符。</span><span class="sxs-lookup"><span data-stu-id="99bde-125">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="99bde-126">contentBytes</span><span class="sxs-lookup"><span data-stu-id="99bde-126">contentBytes</span></span>  |<span data-ttu-id="99bde-127">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="99bde-127">Edm.Binary</span></span>   | <span data-ttu-id="99bde-128">只写。</span><span class="sxs-lookup"><span data-stu-id="99bde-128">Write-only.</span></span> <span data-ttu-id="99bde-129">发布新的聊天消息托管内容时，表示有效负载的字节数。</span><span class="sxs-lookup"><span data-stu-id="99bde-129">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="99bde-130">这些字符串表示为 base64Encoded 字符串。</span><span class="sxs-lookup"><span data-stu-id="99bde-130">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="99bde-131">contentType</span><span class="sxs-lookup"><span data-stu-id="99bde-131">contentType</span></span>   |<span data-ttu-id="99bde-132">String</span><span class="sxs-lookup"><span data-stu-id="99bde-132">String</span></span>       | <span data-ttu-id="99bde-133">只写。</span><span class="sxs-lookup"><span data-stu-id="99bde-133">Write-only.</span></span> <span data-ttu-id="99bde-134">发布新的聊天消息托管内容时，表示内容类型，如图像/png。</span><span class="sxs-lookup"><span data-stu-id="99bde-134">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="99bde-135">实例属性</span><span class="sxs-lookup"><span data-stu-id="99bde-135">Instance attributes</span></span>

<span data-ttu-id="99bde-136">实例属性是具有特殊行为的属性。</span><span class="sxs-lookup"><span data-stu-id="99bde-136">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="99bde-137">这些属性是临时的，可定义服务应执行的行为或提供短期属性值，如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="99bde-137">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="99bde-138">属性名称</span><span class="sxs-lookup"><span data-stu-id="99bde-138">Property name</span></span>                     | <span data-ttu-id="99bde-139">类型</span><span class="sxs-lookup"><span data-stu-id="99bde-139">Type</span></span>   | <span data-ttu-id="99bde-140">说明</span><span class="sxs-lookup"><span data-stu-id="99bde-140">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="99bde-141">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="99bde-141">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="99bde-142">string</span><span class="sxs-lookup"><span data-stu-id="99bde-142">string</span></span> | <span data-ttu-id="99bde-143">只写。</span><span class="sxs-lookup"><span data-stu-id="99bde-143">Write-only.</span></span> <span data-ttu-id="99bde-144">表示托管内容的 temporaryId，同时发布消息以引用要发送的 **chatMessage** 资源中的托管内容。</span><span class="sxs-lookup"><span data-stu-id="99bde-144">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99bde-145">关系</span><span class="sxs-lookup"><span data-stu-id="99bde-145">Relationships</span></span>

<span data-ttu-id="99bde-146">无。</span><span class="sxs-lookup"><span data-stu-id="99bde-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99bde-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99bde-147">JSON representation</span></span>

<span data-ttu-id="99bde-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99bde-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


