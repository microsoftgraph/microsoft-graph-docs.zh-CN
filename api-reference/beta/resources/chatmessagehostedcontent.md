---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8f1577ab7ded60dfd3cad88641bfb11f83d6ad5b
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630289"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="7ecfc-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ecfc-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="7ecfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ecfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ecfc-105">表示在聊天消息中托管的团队内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="7ecfc-106">[文件附件](chatmessageattachment.md)不是托管内容;它们存储在 SharePoint 或 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="7ecfc-107">方法</span><span class="sxs-lookup"><span data-stu-id="7ecfc-107">Methods</span></span>

| <span data-ttu-id="7ecfc-108">方法</span><span class="sxs-lookup"><span data-stu-id="7ecfc-108">Method</span></span>       | <span data-ttu-id="7ecfc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ecfc-109">Return Type</span></span> | <span data-ttu-id="7ecfc-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ecfc-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7ecfc-111">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7ecfc-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="7ecfc-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7ecfc-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="7ecfc-113">检索邮件的**chatMessageHostedContent**列表。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="7ecfc-114">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7ecfc-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="7ecfc-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7ecfc-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="7ecfc-116">读取**chatMessageHostedContent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ecfc-117">属性</span><span class="sxs-lookup"><span data-stu-id="7ecfc-117">Properties</span></span>

| <span data-ttu-id="7ecfc-118">属性</span><span class="sxs-lookup"><span data-stu-id="7ecfc-118">Property</span></span>     | <span data-ttu-id="7ecfc-119">类型</span><span class="sxs-lookup"><span data-stu-id="7ecfc-119">Type</span></span>        | <span data-ttu-id="7ecfc-120">说明</span><span class="sxs-lookup"><span data-stu-id="7ecfc-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ecfc-121">id</span><span class="sxs-lookup"><span data-stu-id="7ecfc-121">id</span></span>            |<span data-ttu-id="7ecfc-122">字符串</span><span class="sxs-lookup"><span data-stu-id="7ecfc-122">String</span></span>       | <span data-ttu-id="7ecfc-123">只读。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-123">Read-only.</span></span> <span data-ttu-id="7ecfc-124">表示聊天消息承载的内容标识符。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="7ecfc-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="7ecfc-125">contentBytes</span></span>  |<span data-ttu-id="7ecfc-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="7ecfc-126">Edm.Binary</span></span>   | <span data-ttu-id="7ecfc-127">只写。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-127">Write-only.</span></span> <span data-ttu-id="7ecfc-128">发布新的聊天邮件承载的内容时，表示有效负载的字节数。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="7ecfc-129">它们表示为 base64Encoded 字符串。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="7ecfc-130">contentType</span><span class="sxs-lookup"><span data-stu-id="7ecfc-130">contentType</span></span>   |<span data-ttu-id="7ecfc-131">String</span><span class="sxs-lookup"><span data-stu-id="7ecfc-131">String</span></span>       | <span data-ttu-id="7ecfc-132">只写。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-132">Write-only.</span></span> <span data-ttu-id="7ecfc-133">发布新的聊天邮件承载的内容时，表示内容的类型，如 image/png。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="7ecfc-134">实例属性</span><span class="sxs-lookup"><span data-stu-id="7ecfc-134">Instance attributes</span></span>

<span data-ttu-id="7ecfc-135">实例属性是具有特殊行为的属性。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="7ecfc-136">这些属性是临时性的，可定义服务应执行的行为，也可以提供短期属性值，如项目的下载 URL 过期。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="7ecfc-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="7ecfc-137">Property name</span></span>                     | <span data-ttu-id="7ecfc-138">类型</span><span class="sxs-lookup"><span data-stu-id="7ecfc-138">Type</span></span>   | <span data-ttu-id="7ecfc-139">说明</span><span class="sxs-lookup"><span data-stu-id="7ecfc-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="7ecfc-140">@microsoft temporaryId</span><span class="sxs-lookup"><span data-stu-id="7ecfc-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="7ecfc-141">string</span><span class="sxs-lookup"><span data-stu-id="7ecfc-141">string</span></span> | <span data-ttu-id="7ecfc-142">只写。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-142">Write-only.</span></span> <span data-ttu-id="7ecfc-143">表示在发布邮件时承载的内容的 temporaryId，以引用正在发送的**了 chatmessage**资源中的托管内容。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ecfc-144">关系</span><span class="sxs-lookup"><span data-stu-id="7ecfc-144">Relationships</span></span>

<span data-ttu-id="7ecfc-145">无。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ecfc-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ecfc-146">JSON representation</span></span>

<span data-ttu-id="7ecfc-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ecfc-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String",
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
