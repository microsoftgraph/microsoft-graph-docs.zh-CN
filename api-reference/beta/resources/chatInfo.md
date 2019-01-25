---
title: chatInfo 资源类型
description: 有关 Microsoft 团队中的邮件的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507661"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="5042e-103">chatInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5042e-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5042e-104">有关 Microsoft 团队中的邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="5042e-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="5042e-105">属性</span><span class="sxs-lookup"><span data-stu-id="5042e-105">Properties</span></span>

| <span data-ttu-id="5042e-106">属性</span><span class="sxs-lookup"><span data-stu-id="5042e-106">Property</span></span>            | <span data-ttu-id="5042e-107">类型</span><span class="sxs-lookup"><span data-stu-id="5042e-107">Type</span></span>    | <span data-ttu-id="5042e-108">说明</span><span class="sxs-lookup"><span data-stu-id="5042e-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="5042e-109">MessageId</span><span class="sxs-lookup"><span data-stu-id="5042e-109">messageId</span></span>           | <span data-ttu-id="5042e-110">String</span><span class="sxs-lookup"><span data-stu-id="5042e-110">String</span></span>  | <span data-ttu-id="5042e-111">Microsoft 团队通道中的邮件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5042e-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="5042e-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="5042e-112">replyChainMessageId</span></span> | <span data-ttu-id="5042e-113">String</span><span class="sxs-lookup"><span data-stu-id="5042e-113">String</span></span>  | <span data-ttu-id="5042e-114">答复邮件的 ID。</span><span class="sxs-lookup"><span data-stu-id="5042e-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="5042e-115">threadId</span><span class="sxs-lookup"><span data-stu-id="5042e-115">threadId</span></span>            | <span data-ttu-id="5042e-116">String</span><span class="sxs-lookup"><span data-stu-id="5042e-116">String</span></span>  | <span data-ttu-id="5042e-117">Microsoft 团队中的线程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5042e-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5042e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5042e-118">JSON representation</span></span>

<span data-ttu-id="5042e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5042e-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatInfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
