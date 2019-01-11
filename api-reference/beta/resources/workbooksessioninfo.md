---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860961"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="836fa-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="836fa-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="836fa-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="836fa-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="836fa-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="836fa-105">JSON representation</span></span>

<span data-ttu-id="836fa-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="836fa-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="836fa-107">属性</span><span class="sxs-lookup"><span data-stu-id="836fa-107">Properties</span></span>

| <span data-ttu-id="836fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="836fa-108">Property</span></span> | <span data-ttu-id="836fa-109">类型</span><span class="sxs-lookup"><span data-stu-id="836fa-109">Type</span></span>  | <span data-ttu-id="836fa-110">说明</span><span class="sxs-lookup"><span data-stu-id="836fa-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="836fa-111">ID</span><span class="sxs-lookup"><span data-stu-id="836fa-111">id</span></span>  | <span data-ttu-id="836fa-112">string</span><span class="sxs-lookup"><span data-stu-id="836fa-112">string</span></span> | <span data-ttu-id="836fa-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="836fa-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="836fa-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="836fa-114">persistChanges</span></span> | <span data-ttu-id="836fa-115">string</span><span class="sxs-lookup"><span data-stu-id="836fa-115">string</span></span> |  <span data-ttu-id="836fa-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="836fa-116">`true` for persistent session.</span></span> <span data-ttu-id="836fa-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="836fa-117">`false` for non-persistent session (view mode)</span></span> |

