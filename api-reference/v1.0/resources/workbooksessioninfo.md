---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2e6b925e7cc1790b1c6d4f08bab02fa92f19936
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033332"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="e387b-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e387b-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="e387b-104">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="e387b-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e387b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e387b-105">JSON representation</span></span>

<span data-ttu-id="e387b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e387b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e387b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e387b-107">Properties</span></span>

| <span data-ttu-id="e387b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e387b-108">Property</span></span> | <span data-ttu-id="e387b-109">类型</span><span class="sxs-lookup"><span data-stu-id="e387b-109">Type</span></span>  | <span data-ttu-id="e387b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e387b-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="e387b-111">id</span><span class="sxs-lookup"><span data-stu-id="e387b-111">id</span></span>  | <span data-ttu-id="e387b-112">string</span><span class="sxs-lookup"><span data-stu-id="e387b-112">string</span></span> | <span data-ttu-id="e387b-113">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="e387b-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="e387b-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="e387b-114">persistChanges</span></span> | <span data-ttu-id="e387b-115">boolean</span><span class="sxs-lookup"><span data-stu-id="e387b-115">boolean</span></span> |  <span data-ttu-id="e387b-116">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e387b-116">`true` for persistent session.</span></span> <span data-ttu-id="e387b-117">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e387b-117">`false` for non-persistent session (view mode)</span></span> |

