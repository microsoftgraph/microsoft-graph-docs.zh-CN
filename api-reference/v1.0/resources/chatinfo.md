---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7cd56e21997daf4b88f25acc570f5c062959fa2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871081"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="f7358-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7358-103">chatInfo resource type</span></span>

<span data-ttu-id="f7358-104">这包含与 Microsoft 团队会议相关的信息。</span><span class="sxs-lookup"><span data-stu-id="f7358-104">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="f7358-105">属性</span><span class="sxs-lookup"><span data-stu-id="f7358-105">Properties</span></span>

| <span data-ttu-id="f7358-106">属性</span><span class="sxs-lookup"><span data-stu-id="f7358-106">Property</span></span>            | <span data-ttu-id="f7358-107">类型</span><span class="sxs-lookup"><span data-stu-id="f7358-107">Type</span></span>    | <span data-ttu-id="f7358-108">说明</span><span class="sxs-lookup"><span data-stu-id="f7358-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="f7358-109">messageId</span><span class="sxs-lookup"><span data-stu-id="f7358-109">messageId</span></span>           | <span data-ttu-id="f7358-110">String</span><span class="sxs-lookup"><span data-stu-id="f7358-110">String</span></span>  | <span data-ttu-id="f7358-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7358-111">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="f7358-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="f7358-112">replyChainMessageId</span></span> | <span data-ttu-id="f7358-113">String</span><span class="sxs-lookup"><span data-stu-id="f7358-113">String</span></span>  | <span data-ttu-id="f7358-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="f7358-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="f7358-115">threadId</span><span class="sxs-lookup"><span data-stu-id="f7358-115">threadId</span></span>            | <span data-ttu-id="f7358-116">String</span><span class="sxs-lookup"><span data-stu-id="f7358-116">String</span></span>  | <span data-ttu-id="f7358-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f7358-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7358-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7358-118">JSON representation</span></span>

<span data-ttu-id="f7358-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7358-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
