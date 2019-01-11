---
title: resultInfo 资源类型
description: ResultInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ca814fd5c44f0f811099faed53354d08ce8befdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855277"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="c55ef-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c55ef-103">resultInfo resource type</span></span>

> <span data-ttu-id="c55ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c55ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c55ef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c55ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c55ef-106">ResultInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="c55ef-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="c55ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="c55ef-107">Properties</span></span>

| <span data-ttu-id="c55ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="c55ef-108">Property</span></span> | <span data-ttu-id="c55ef-109">类型</span><span class="sxs-lookup"><span data-stu-id="c55ef-109">Type</span></span>   | <span data-ttu-id="c55ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="c55ef-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="c55ef-111">code</span><span class="sxs-lookup"><span data-stu-id="c55ef-111">code</span></span>     | <span data-ttu-id="c55ef-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c55ef-112">String</span></span> | <span data-ttu-id="c55ef-113">结果代码。</span><span class="sxs-lookup"><span data-stu-id="c55ef-113">The result code.</span></span>     |
| <span data-ttu-id="c55ef-114">message</span><span class="sxs-lookup"><span data-stu-id="c55ef-114">message</span></span>  | <span data-ttu-id="c55ef-115">字符串</span><span class="sxs-lookup"><span data-stu-id="c55ef-115">String</span></span> | <span data-ttu-id="c55ef-116">消息。</span><span class="sxs-lookup"><span data-stu-id="c55ef-116">The message.</span></span>         |
| <span data-ttu-id="c55ef-117">subCode</span><span class="sxs-lookup"><span data-stu-id="c55ef-117">subCode</span></span>  | <span data-ttu-id="c55ef-118">字符串</span><span class="sxs-lookup"><span data-stu-id="c55ef-118">String</span></span> | <span data-ttu-id="c55ef-119">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="c55ef-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c55ef-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c55ef-120">JSON representation</span></span>

<span data-ttu-id="c55ef-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c55ef-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="c55ef-122">示例错误结果</span><span class="sxs-lookup"><span data-stu-id="c55ef-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="c55ef-123">示例通用的成功结果</span><span class="sxs-lookup"><span data-stu-id="c55ef-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="c55ef-124">示例记录成功结果</span><span class="sxs-lookup"><span data-stu-id="c55ef-124">Example Record Success result</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
