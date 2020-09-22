---
title: workbookSessionInfo 资源类型
description: 提供有关工作簿会话的信息。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d5b75d3062b087848f804c0f89726c67783c540
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015104"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="d567f-103">workbookSessionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d567f-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="d567f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d567f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d567f-105">提供有关工作簿会话的信息。</span><span class="sxs-lookup"><span data-stu-id="d567f-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d567f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d567f-106">JSON representation</span></span>

<span data-ttu-id="d567f-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d567f-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d567f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d567f-108">Properties</span></span>

| <span data-ttu-id="d567f-109">属性</span><span class="sxs-lookup"><span data-stu-id="d567f-109">Property</span></span> | <span data-ttu-id="d567f-110">类型</span><span class="sxs-lookup"><span data-stu-id="d567f-110">Type</span></span>  | <span data-ttu-id="d567f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d567f-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="d567f-112">id</span><span class="sxs-lookup"><span data-stu-id="d567f-112">id</span></span>  | <span data-ttu-id="d567f-113">string</span><span class="sxs-lookup"><span data-stu-id="d567f-113">string</span></span> | <span data-ttu-id="d567f-114">工作簿会话 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d567f-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="d567f-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="d567f-115">persistChanges</span></span> | <span data-ttu-id="d567f-116">boolean</span><span class="sxs-lookup"><span data-stu-id="d567f-116">boolean</span></span> |  <span data-ttu-id="d567f-117">对于持续会话，值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="d567f-117">`true` for persistent session.</span></span> <span data-ttu-id="d567f-118">对于非持续会话（视图模式），值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="d567f-118">`false` for non-persistent session (view mode)</span></span> |


