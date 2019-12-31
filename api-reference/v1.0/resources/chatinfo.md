---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de48737299a940db545e46daabd129ee7443c60a
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913252"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="31f9b-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="31f9b-103">chatInfo resource type</span></span>

<span data-ttu-id="31f9b-104">这包含与 Microsoft 团队会议相关的信息。</span><span class="sxs-lookup"><span data-stu-id="31f9b-104">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="31f9b-105">属性</span><span class="sxs-lookup"><span data-stu-id="31f9b-105">Properties</span></span>

| <span data-ttu-id="31f9b-106">属性</span><span class="sxs-lookup"><span data-stu-id="31f9b-106">Property</span></span>            | <span data-ttu-id="31f9b-107">类型</span><span class="sxs-lookup"><span data-stu-id="31f9b-107">Type</span></span>    | <span data-ttu-id="31f9b-108">说明</span><span class="sxs-lookup"><span data-stu-id="31f9b-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="31f9b-109">messageId</span><span class="sxs-lookup"><span data-stu-id="31f9b-109">messageId</span></span>           | <span data-ttu-id="31f9b-110">String</span><span class="sxs-lookup"><span data-stu-id="31f9b-110">String</span></span>  | <span data-ttu-id="31f9b-111">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31f9b-111">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="31f9b-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="31f9b-112">replyChainMessageId</span></span> | <span data-ttu-id="31f9b-113">String</span><span class="sxs-lookup"><span data-stu-id="31f9b-113">String</span></span>  | <span data-ttu-id="31f9b-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="31f9b-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="31f9b-115">threadId</span><span class="sxs-lookup"><span data-stu-id="31f9b-115">threadId</span></span>            | <span data-ttu-id="31f9b-116">String</span><span class="sxs-lookup"><span data-stu-id="31f9b-116">String</span></span>  | <span data-ttu-id="31f9b-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31f9b-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31f9b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31f9b-118">JSON representation</span></span>

<span data-ttu-id="31f9b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31f9b-119">The following is a JSON representation of the resource.</span></span>

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
