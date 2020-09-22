---
title: workbookOperationError 资源类型
description: 表示失败的工作簿操作中的错误。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce65847d6ddbb0a8db0c1277e38753ecab7080e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015139"
---
# <a name="workbookoperationerror-resource-type"></a><span data-ttu-id="a9fe8-103">workbookOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9fe8-103">workbookOperationError resource type</span></span>

<span data-ttu-id="a9fe8-104">表示失败的工作簿操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="a9fe8-104">Represents an error from a failed workbook operation.</span></span>

## <a name="properties"></a><span data-ttu-id="a9fe8-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9fe8-105">Properties</span></span>

| <span data-ttu-id="a9fe8-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9fe8-106">Property</span></span>     | <span data-ttu-id="a9fe8-107">类型</span><span class="sxs-lookup"><span data-stu-id="a9fe8-107">Type</span></span>        | <span data-ttu-id="a9fe8-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9fe8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9fe8-109">code</span><span class="sxs-lookup"><span data-stu-id="a9fe8-109">code</span></span>|<span data-ttu-id="a9fe8-110">String</span><span class="sxs-lookup"><span data-stu-id="a9fe8-110">String</span></span>| <span data-ttu-id="a9fe8-111">错误代码。</span><span class="sxs-lookup"><span data-stu-id="a9fe8-111">The error code.</span></span>|
|<span data-ttu-id="a9fe8-112">message</span><span class="sxs-lookup"><span data-stu-id="a9fe8-112">message</span></span>|<span data-ttu-id="a9fe8-113">String</span><span class="sxs-lookup"><span data-stu-id="a9fe8-113">String</span></span>| <span data-ttu-id="a9fe8-114">错误消息。</span><span class="sxs-lookup"><span data-stu-id="a9fe8-114">The error message.</span></span>|
|<span data-ttu-id="a9fe8-115">innererror</span><span class="sxs-lookup"><span data-stu-id="a9fe8-115">innererror</span></span>|<span data-ttu-id="a9fe8-116">error object</span><span class="sxs-lookup"><span data-stu-id="a9fe8-116">error object</span></span>| <span data-ttu-id="a9fe8-p101">可选。可能比顶级错误更具体的其他错误对象。</span><span class="sxs-lookup"><span data-stu-id="a9fe8-p101">Optional. Additional error objects that may be more specific than the top level error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9fe8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9fe8-119">JSON representation</span></span>

<span data-ttu-id="a9fe8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9fe8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

