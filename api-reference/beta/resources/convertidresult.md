---
title: convertIdResult 资源类型
description: 执行由 translateExchangeIds 函数 ID 格式转换的结果。
localization_priority: Normal
ms.openlocfilehash: db28172d009ee8a8a39b7e02733d893dc20a81e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516523"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="ea98b-103">convertIdResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea98b-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea98b-104">执行由[translateExchangeIds](../api/user-translateexchangeids.md)函数 ID 格式转换的结果。</span><span class="sxs-lookup"><span data-stu-id="ea98b-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="ea98b-105">属性</span><span class="sxs-lookup"><span data-stu-id="ea98b-105">Properties</span></span>

| <span data-ttu-id="ea98b-106">属性</span><span class="sxs-lookup"><span data-stu-id="ea98b-106">Property</span></span> | <span data-ttu-id="ea98b-107">类型</span><span class="sxs-lookup"><span data-stu-id="ea98b-107">Type</span></span> | <span data-ttu-id="ea98b-108">说明</span><span class="sxs-lookup"><span data-stu-id="ea98b-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ea98b-109">SourceId</span><span class="sxs-lookup"><span data-stu-id="ea98b-109">sourceId</span></span> | <span data-ttu-id="ea98b-110">String</span><span class="sxs-lookup"><span data-stu-id="ea98b-110">String</span></span> | <span data-ttu-id="ea98b-111">已转换的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea98b-111">The identifier that was converted.</span></span> <span data-ttu-id="ea98b-112">此值是原始、 未转换标识符。</span><span class="sxs-lookup"><span data-stu-id="ea98b-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="ea98b-113">targetId</span><span class="sxs-lookup"><span data-stu-id="ea98b-113">targetId</span></span> | <span data-ttu-id="ea98b-114">String</span><span class="sxs-lookup"><span data-stu-id="ea98b-114">String</span></span> | <span data-ttu-id="ea98b-115">转换后的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea98b-115">The converted identifier.</span></span> <span data-ttu-id="ea98b-116">此值不存在，如果转换失败。</span><span class="sxs-lookup"><span data-stu-id="ea98b-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="ea98b-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="ea98b-117">errorDetails</span></span> | [<span data-ttu-id="ea98b-118">genericError</span><span class="sxs-lookup"><span data-stu-id="ea98b-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="ea98b-119">Error 对象指示转换失败的原因。</span><span class="sxs-lookup"><span data-stu-id="ea98b-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="ea98b-120">此值不存在，如果转换成功。</span><span class="sxs-lookup"><span data-stu-id="ea98b-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea98b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea98b-121">JSON representation</span></span>

<span data-ttu-id="ea98b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea98b-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/convertidresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
