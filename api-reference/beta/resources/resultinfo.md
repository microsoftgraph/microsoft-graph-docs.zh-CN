---
title: resultInfo 资源类型
description: ResultInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521080"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="ce4e4-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce4e4-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce4e4-104">ResultInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="ce4e4-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="ce4e4-105">属性</span><span class="sxs-lookup"><span data-stu-id="ce4e4-105">Properties</span></span>

| <span data-ttu-id="ce4e4-106">属性</span><span class="sxs-lookup"><span data-stu-id="ce4e4-106">Property</span></span> | <span data-ttu-id="ce4e4-107">类型</span><span class="sxs-lookup"><span data-stu-id="ce4e4-107">Type</span></span>   | <span data-ttu-id="ce4e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="ce4e4-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="ce4e4-109">code</span><span class="sxs-lookup"><span data-stu-id="ce4e4-109">code</span></span>     | <span data-ttu-id="ce4e4-110">String</span><span class="sxs-lookup"><span data-stu-id="ce4e4-110">String</span></span> | <span data-ttu-id="ce4e4-111">结果代码。</span><span class="sxs-lookup"><span data-stu-id="ce4e4-111">The result code.</span></span>     |
| <span data-ttu-id="ce4e4-112">message</span><span class="sxs-lookup"><span data-stu-id="ce4e4-112">message</span></span>  | <span data-ttu-id="ce4e4-113">String</span><span class="sxs-lookup"><span data-stu-id="ce4e4-113">String</span></span> | <span data-ttu-id="ce4e4-114">消息。</span><span class="sxs-lookup"><span data-stu-id="ce4e4-114">The message.</span></span>         |
| <span data-ttu-id="ce4e4-115">subCode</span><span class="sxs-lookup"><span data-stu-id="ce4e4-115">subCode</span></span>  | <span data-ttu-id="ce4e4-116">String</span><span class="sxs-lookup"><span data-stu-id="ce4e4-116">String</span></span> | <span data-ttu-id="ce4e4-117">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="ce4e4-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce4e4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce4e4-118">JSON representation</span></span>

<span data-ttu-id="ce4e4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce4e4-119">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="ce4e4-120">示例错误结果</span><span class="sxs-lookup"><span data-stu-id="ce4e4-120">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="ce4e4-121">示例通用的成功结果</span><span class="sxs-lookup"><span data-stu-id="ce4e4-121">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="ce4e4-122">示例记录成功结果</span><span class="sxs-lookup"><span data-stu-id="ce4e4-122">Example Record Success result</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/resultinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
