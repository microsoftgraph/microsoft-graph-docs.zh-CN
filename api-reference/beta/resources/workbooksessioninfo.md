---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642217"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="af396-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="af396-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="af396-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="af396-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="af396-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af396-105">JSON representation</span></span>

<span data-ttu-id="af396-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af396-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="af396-107">属性</span><span class="sxs-lookup"><span data-stu-id="af396-107">Properties</span></span>

| <span data-ttu-id="af396-108">属性</span><span class="sxs-lookup"><span data-stu-id="af396-108">Property</span></span> | <span data-ttu-id="af396-109">类型</span><span class="sxs-lookup"><span data-stu-id="af396-109">Type</span></span>  | <span data-ttu-id="af396-110">说明</span><span class="sxs-lookup"><span data-stu-id="af396-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="af396-111">id</span><span class="sxs-lookup"><span data-stu-id="af396-111">id</span></span>  | <span data-ttu-id="af396-112">string</span><span class="sxs-lookup"><span data-stu-id="af396-112">string</span></span> | <span data-ttu-id="af396-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="af396-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="af396-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="af396-114">persistChanges</span></span> | <span data-ttu-id="af396-115">string</span><span class="sxs-lookup"><span data-stu-id="af396-115">string</span></span> |  <span data-ttu-id="af396-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="af396-116">`true` for persistent session.</span></span> <span data-ttu-id="af396-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="af396-117">`false` for non-persistent session (view mode)</span></span> |

