---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3035574b92dfa703b926a81163efbb7f6eff764b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345774"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="14fb9-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="14fb9-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14fb9-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="14fb9-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="14fb9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14fb9-105">JSON representation</span></span>

<span data-ttu-id="14fb9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14fb9-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="14fb9-107">属性</span><span class="sxs-lookup"><span data-stu-id="14fb9-107">Properties</span></span>

| <span data-ttu-id="14fb9-108">属性</span><span class="sxs-lookup"><span data-stu-id="14fb9-108">Property</span></span> | <span data-ttu-id="14fb9-109">类型</span><span class="sxs-lookup"><span data-stu-id="14fb9-109">Type</span></span>  | <span data-ttu-id="14fb9-110">说明</span><span class="sxs-lookup"><span data-stu-id="14fb9-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="14fb9-111">id</span><span class="sxs-lookup"><span data-stu-id="14fb9-111">id</span></span>  | <span data-ttu-id="14fb9-112">string</span><span class="sxs-lookup"><span data-stu-id="14fb9-112">string</span></span> | <span data-ttu-id="14fb9-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="14fb9-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="14fb9-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="14fb9-114">persistChanges</span></span> | <span data-ttu-id="14fb9-115">string</span><span class="sxs-lookup"><span data-stu-id="14fb9-115">string</span></span> |  <span data-ttu-id="14fb9-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="14fb9-116">`true` for persistent session.</span></span> <span data-ttu-id="14fb9-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="14fb9-117">`false` for non-persistent session (view mode)</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
