---
title: resultInfo 资源类型
description: resultInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562991"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="09911-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="09911-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09911-104">resultInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="09911-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="09911-105">属性</span><span class="sxs-lookup"><span data-stu-id="09911-105">Properties</span></span>

| <span data-ttu-id="09911-106">属性</span><span class="sxs-lookup"><span data-stu-id="09911-106">Property</span></span> | <span data-ttu-id="09911-107">类型</span><span class="sxs-lookup"><span data-stu-id="09911-107">Type</span></span>   | <span data-ttu-id="09911-108">说明</span><span class="sxs-lookup"><span data-stu-id="09911-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="09911-109">code</span><span class="sxs-lookup"><span data-stu-id="09911-109">code</span></span>     | <span data-ttu-id="09911-110">String</span><span class="sxs-lookup"><span data-stu-id="09911-110">String</span></span> | <span data-ttu-id="09911-111">结果代码。</span><span class="sxs-lookup"><span data-stu-id="09911-111">The result code.</span></span>     |
| <span data-ttu-id="09911-112">message</span><span class="sxs-lookup"><span data-stu-id="09911-112">message</span></span>  | <span data-ttu-id="09911-113">String</span><span class="sxs-lookup"><span data-stu-id="09911-113">String</span></span> | <span data-ttu-id="09911-114">邮件。</span><span class="sxs-lookup"><span data-stu-id="09911-114">The message.</span></span>         |
| <span data-ttu-id="09911-115">subCode</span><span class="sxs-lookup"><span data-stu-id="09911-115">subCode</span></span>  | <span data-ttu-id="09911-116">String</span><span class="sxs-lookup"><span data-stu-id="09911-116">String</span></span> | <span data-ttu-id="09911-117">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="09911-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09911-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09911-118">JSON representation</span></span>

<span data-ttu-id="09911-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09911-119">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="09911-120">示例错误结果</span><span class="sxs-lookup"><span data-stu-id="09911-120">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="09911-121">示例一般成功结果</span><span class="sxs-lookup"><span data-stu-id="09911-121">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="09911-122">记录成功结果的示例</span><span class="sxs-lookup"><span data-stu-id="09911-122">Example Record Success result</span></span>

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
