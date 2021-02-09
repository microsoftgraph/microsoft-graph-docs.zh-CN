---
title: chatMessageHostedContent 资源类型
description: 聊天消息中托管的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc4f61fb0b0e6c174be50c988d1cbb22576c4f27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159617"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="e7fea-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7fea-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="e7fea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7fea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fea-105">表示聊天消息中托管的 Teams 内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="e7fea-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="e7fea-106">[文件附件](chatmessageattachment.md) 不是托管内容;它们存储在 SharePoint 或 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="e7fea-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="e7fea-107">方法</span><span class="sxs-lookup"><span data-stu-id="e7fea-107">Methods</span></span>

| <span data-ttu-id="e7fea-108">方法</span><span class="sxs-lookup"><span data-stu-id="e7fea-108">Method</span></span>       | <span data-ttu-id="e7fea-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7fea-109">Return Type</span></span> | <span data-ttu-id="e7fea-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7fea-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7fea-111">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e7fea-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="e7fea-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e7fea-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="e7fea-113">检索消息的 **chatMessageHostedContent** 列表。</span><span class="sxs-lookup"><span data-stu-id="e7fea-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="e7fea-114">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e7fea-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="e7fea-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e7fea-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="e7fea-116">读取 **chatMessageHostedContent** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7fea-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7fea-117">属性</span><span class="sxs-lookup"><span data-stu-id="e7fea-117">Properties</span></span>

| <span data-ttu-id="e7fea-118">属性</span><span class="sxs-lookup"><span data-stu-id="e7fea-118">Property</span></span>     | <span data-ttu-id="e7fea-119">类型</span><span class="sxs-lookup"><span data-stu-id="e7fea-119">Type</span></span>        | <span data-ttu-id="e7fea-120">说明</span><span class="sxs-lookup"><span data-stu-id="e7fea-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7fea-121">id</span><span class="sxs-lookup"><span data-stu-id="e7fea-121">id</span></span>            |<span data-ttu-id="e7fea-122">String</span><span class="sxs-lookup"><span data-stu-id="e7fea-122">String</span></span>       | <span data-ttu-id="e7fea-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e7fea-123">Read-only.</span></span> <span data-ttu-id="e7fea-124">表示聊天消息托管的内容标识符。</span><span class="sxs-lookup"><span data-stu-id="e7fea-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="e7fea-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="e7fea-125">contentBytes</span></span>  |<span data-ttu-id="e7fea-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="e7fea-126">Edm.Binary</span></span>   | <span data-ttu-id="e7fea-127">只写。</span><span class="sxs-lookup"><span data-stu-id="e7fea-127">Write-only.</span></span> <span data-ttu-id="e7fea-128">发布新的聊天消息托管内容时，表示有效负载的字节数。</span><span class="sxs-lookup"><span data-stu-id="e7fea-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="e7fea-129">这些字符串表示为 base64Encoded 字符串。</span><span class="sxs-lookup"><span data-stu-id="e7fea-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="e7fea-130">contentType</span><span class="sxs-lookup"><span data-stu-id="e7fea-130">contentType</span></span>   |<span data-ttu-id="e7fea-131">String</span><span class="sxs-lookup"><span data-stu-id="e7fea-131">String</span></span>       | <span data-ttu-id="e7fea-132">只写。</span><span class="sxs-lookup"><span data-stu-id="e7fea-132">Write-only.</span></span> <span data-ttu-id="e7fea-133">发布新的聊天消息托管内容时，表示内容类型，如 image/png。</span><span class="sxs-lookup"><span data-stu-id="e7fea-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="e7fea-134">实例属性</span><span class="sxs-lookup"><span data-stu-id="e7fea-134">Instance attributes</span></span>

<span data-ttu-id="e7fea-135">实例属性是具有特殊行为的属性。</span><span class="sxs-lookup"><span data-stu-id="e7fea-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="e7fea-136">这些属性是临时的，可定义服务应执行的行为或提供短期属性值，如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e7fea-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="e7fea-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="e7fea-137">Property name</span></span>                     | <span data-ttu-id="e7fea-138">类型</span><span class="sxs-lookup"><span data-stu-id="e7fea-138">Type</span></span>   | <span data-ttu-id="e7fea-139">说明</span><span class="sxs-lookup"><span data-stu-id="e7fea-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="e7fea-140">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="e7fea-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="e7fea-141">string</span><span class="sxs-lookup"><span data-stu-id="e7fea-141">string</span></span> | <span data-ttu-id="e7fea-142">只写。</span><span class="sxs-lookup"><span data-stu-id="e7fea-142">Write-only.</span></span> <span data-ttu-id="e7fea-143">表示托管内容的 temporaryId，同时发布消息以引用正在发送的 **chatMessage** 资源中的托管内容。</span><span class="sxs-lookup"><span data-stu-id="e7fea-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7fea-144">关系</span><span class="sxs-lookup"><span data-stu-id="e7fea-144">Relationships</span></span>

<span data-ttu-id="e7fea-145">无。</span><span class="sxs-lookup"><span data-stu-id="e7fea-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7fea-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7fea-146">JSON representation</span></span>

<span data-ttu-id="e7fea-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7fea-147">The following is a JSON representation of the resource.</span></span>

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


