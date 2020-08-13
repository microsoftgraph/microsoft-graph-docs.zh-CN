---
title: chatInfo 资源类型
description: 包含与 Microsoft 团队会议相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8602301af0de458f07ab5a9c0af00ec8578c3a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507731"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="71c42-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="71c42-103">chatInfo resource type</span></span>

<span data-ttu-id="71c42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71c42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c42-105">包含与 Microsoft 团队会议相关的信息。</span><span class="sxs-lookup"><span data-stu-id="71c42-105">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="71c42-106">属性</span><span class="sxs-lookup"><span data-stu-id="71c42-106">Properties</span></span>

| <span data-ttu-id="71c42-107">属性</span><span class="sxs-lookup"><span data-stu-id="71c42-107">Property</span></span>            | <span data-ttu-id="71c42-108">类型</span><span class="sxs-lookup"><span data-stu-id="71c42-108">Type</span></span>    | <span data-ttu-id="71c42-109">说明</span><span class="sxs-lookup"><span data-stu-id="71c42-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="71c42-110">messageId</span><span class="sxs-lookup"><span data-stu-id="71c42-110">messageId</span></span>           | <span data-ttu-id="71c42-111">String</span><span class="sxs-lookup"><span data-stu-id="71c42-111">String</span></span>  | <span data-ttu-id="71c42-112">Microsoft 团队频道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71c42-112">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="71c42-113">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="71c42-113">replyChainMessageId</span></span> | <span data-ttu-id="71c42-114">String</span><span class="sxs-lookup"><span data-stu-id="71c42-114">String</span></span>  | <span data-ttu-id="71c42-115">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="71c42-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="71c42-116">threadId</span><span class="sxs-lookup"><span data-stu-id="71c42-116">threadId</span></span>            | <span data-ttu-id="71c42-117">String</span><span class="sxs-lookup"><span data-stu-id="71c42-117">String</span></span>  | <span data-ttu-id="71c42-118">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71c42-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71c42-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71c42-119">JSON representation</span></span>

<span data-ttu-id="71c42-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71c42-120">The following is a JSON representation of the resource.</span></span>

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
