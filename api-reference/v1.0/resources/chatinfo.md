---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b69905a0e1d8937c582df3373a4e981f8d8405ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533079"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="8a052-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a052-103">chatInfo resource type</span></span>

<span data-ttu-id="8a052-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a052-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a052-105">这包含与 Microsoft 团队会议相关的信息。</span><span class="sxs-lookup"><span data-stu-id="8a052-105">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="8a052-106">属性</span><span class="sxs-lookup"><span data-stu-id="8a052-106">Properties</span></span>

| <span data-ttu-id="8a052-107">属性</span><span class="sxs-lookup"><span data-stu-id="8a052-107">Property</span></span>            | <span data-ttu-id="8a052-108">类型</span><span class="sxs-lookup"><span data-stu-id="8a052-108">Type</span></span>    | <span data-ttu-id="8a052-109">说明</span><span class="sxs-lookup"><span data-stu-id="8a052-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="8a052-110">messageId</span><span class="sxs-lookup"><span data-stu-id="8a052-110">messageId</span></span>           | <span data-ttu-id="8a052-111">字符串</span><span class="sxs-lookup"><span data-stu-id="8a052-111">String</span></span>  | <span data-ttu-id="8a052-112">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a052-112">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="8a052-113">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="8a052-113">replyChainMessageId</span></span> | <span data-ttu-id="8a052-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8a052-114">String</span></span>  | <span data-ttu-id="8a052-115">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a052-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="8a052-116">threadId</span><span class="sxs-lookup"><span data-stu-id="8a052-116">threadId</span></span>            | <span data-ttu-id="8a052-117">字符串</span><span class="sxs-lookup"><span data-stu-id="8a052-117">String</span></span>  | <span data-ttu-id="8a052-118">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a052-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a052-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a052-119">JSON representation</span></span>

<span data-ttu-id="8a052-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a052-120">The following is a JSON representation of the resource.</span></span>

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
