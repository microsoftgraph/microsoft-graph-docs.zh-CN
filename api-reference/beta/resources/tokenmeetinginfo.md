---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8e115887e67f19375ca8b96a216af98c80e0b312
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513366"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="0fb7f-103">tokenMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fb7f-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb7f-104">TokenMeetingInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="0fb7f-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="0fb7f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0fb7f-105">Properties</span></span>

| <span data-ttu-id="0fb7f-106">属性</span><span class="sxs-lookup"><span data-stu-id="0fb7f-106">Property</span></span>                     | <span data-ttu-id="0fb7f-107">类型</span><span class="sxs-lookup"><span data-stu-id="0fb7f-107">Type</span></span>    | <span data-ttu-id="0fb7f-108">说明</span><span class="sxs-lookup"><span data-stu-id="0fb7f-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="0fb7f-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="0fb7f-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="0fb7f-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb7f-110">Boolean</span></span> | <span data-ttu-id="0fb7f-111">指示是否一旦离开对话的主机，也可以继续对话。</span><span class="sxs-lookup"><span data-stu-id="0fb7f-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="0fb7f-112">token</span><span class="sxs-lookup"><span data-stu-id="0fb7f-112">token</span></span>                        | <span data-ttu-id="0fb7f-113">String</span><span class="sxs-lookup"><span data-stu-id="0fb7f-113">String</span></span>  | <span data-ttu-id="0fb7f-114">要加入/激活会议的标记。</span><span class="sxs-lookup"><span data-stu-id="0fb7f-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="0fb7f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fb7f-115">JSON representation</span></span>

<span data-ttu-id="0fb7f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fb7f-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="0fb7f-117">示例</span><span class="sxs-lookup"><span data-stu-id="0fb7f-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tokenmeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
