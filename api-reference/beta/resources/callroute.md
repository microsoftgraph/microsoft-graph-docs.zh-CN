---
title: callRoute 资源类型
description: callRoute 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543829"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="cdbc2-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="cdbc2-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdbc2-104">callRoute 类型。</span><span class="sxs-lookup"><span data-stu-id="cdbc2-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="cdbc2-105">属性</span><span class="sxs-lookup"><span data-stu-id="cdbc2-105">Properties</span></span>

| <span data-ttu-id="cdbc2-106">属性</span><span class="sxs-lookup"><span data-stu-id="cdbc2-106">Property</span></span>            | <span data-ttu-id="cdbc2-107">类型</span><span class="sxs-lookup"><span data-stu-id="cdbc2-107">Type</span></span>                          | <span data-ttu-id="cdbc2-108">说明</span><span class="sxs-lookup"><span data-stu-id="cdbc2-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="cdbc2-109">终稿</span><span class="sxs-lookup"><span data-stu-id="cdbc2-109">final</span></span>               | [<span data-ttu-id="cdbc2-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="cdbc2-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="cdbc2-111">在呼叫中解析为的标识。</span><span class="sxs-lookup"><span data-stu-id="cdbc2-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="cdbc2-112">源语言</span><span class="sxs-lookup"><span data-stu-id="cdbc2-112">original</span></span>            | [<span data-ttu-id="cdbc2-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="cdbc2-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="cdbc2-114">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="cdbc2-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="cdbc2-115">routingType</span><span class="sxs-lookup"><span data-stu-id="cdbc2-115">routingType</span></span>         | <span data-ttu-id="cdbc2-116">String</span><span class="sxs-lookup"><span data-stu-id="cdbc2-116">String</span></span>                        | <span data-ttu-id="cdbc2-117">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="cdbc2-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cdbc2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cdbc2-118">JSON representation</span></span>

<span data-ttu-id="cdbc2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdbc2-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
