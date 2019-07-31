---
title: resultInfo 资源类型
description: ResultInfo 类型。
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1e5f6a523a8aca4454cd3355e2a0287fef9fc90d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965367"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="259b6-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="259b6-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="259b6-104">ResultInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="259b6-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="259b6-105">属性</span><span class="sxs-lookup"><span data-stu-id="259b6-105">Properties</span></span>

| <span data-ttu-id="259b6-106">属性</span><span class="sxs-lookup"><span data-stu-id="259b6-106">Property</span></span> | <span data-ttu-id="259b6-107">类型</span><span class="sxs-lookup"><span data-stu-id="259b6-107">Type</span></span>   | <span data-ttu-id="259b6-108">说明</span><span class="sxs-lookup"><span data-stu-id="259b6-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="259b6-109">code</span><span class="sxs-lookup"><span data-stu-id="259b6-109">code</span></span>     | <span data-ttu-id="259b6-110">String</span><span class="sxs-lookup"><span data-stu-id="259b6-110">String</span></span> | <span data-ttu-id="259b6-111">结果代码。</span><span class="sxs-lookup"><span data-stu-id="259b6-111">The result code.</span></span>     |
| <span data-ttu-id="259b6-112">message</span><span class="sxs-lookup"><span data-stu-id="259b6-112">message</span></span>  | <span data-ttu-id="259b6-113">String</span><span class="sxs-lookup"><span data-stu-id="259b6-113">String</span></span> | <span data-ttu-id="259b6-114">邮件。</span><span class="sxs-lookup"><span data-stu-id="259b6-114">The message.</span></span>         |
| <span data-ttu-id="259b6-115">subCode</span><span class="sxs-lookup"><span data-stu-id="259b6-115">subCode</span></span>  | <span data-ttu-id="259b6-116">String</span><span class="sxs-lookup"><span data-stu-id="259b6-116">String</span></span> | <span data-ttu-id="259b6-117">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="259b6-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="259b6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="259b6-118">JSON representation</span></span>

<span data-ttu-id="259b6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="259b6-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="259b6-120">示例错误结果</span><span class="sxs-lookup"><span data-stu-id="259b6-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="259b6-121">示例一般成功结果</span><span class="sxs-lookup"><span data-stu-id="259b6-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="259b6-122">记录成功结果的示例</span><span class="sxs-lookup"><span data-stu-id="259b6-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
