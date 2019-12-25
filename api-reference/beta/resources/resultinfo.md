---
title: resultInfo 资源类型
description: 包含成功和失败的特定结果信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb59cb63ff7c50ba14b972991d54806eabc4f54
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866628"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="f0c94-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0c94-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c94-104">包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="f0c94-104">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="f0c94-105">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="f0c94-105">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="f0c94-106">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）。</span><span class="sxs-lookup"><span data-stu-id="f0c94-106">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="f0c94-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0c94-107">Properties</span></span>

| <span data-ttu-id="f0c94-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0c94-108">Property</span></span> | <span data-ttu-id="f0c94-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0c94-109">Type</span></span>   | <span data-ttu-id="f0c94-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0c94-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="f0c94-111">code</span><span class="sxs-lookup"><span data-stu-id="f0c94-111">code</span></span>     | <span data-ttu-id="f0c94-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f0c94-112">Int32</span></span> | <span data-ttu-id="f0c94-113">结果代码。</span><span class="sxs-lookup"><span data-stu-id="f0c94-113">The result code.</span></span>     |
| <span data-ttu-id="f0c94-114">message</span><span class="sxs-lookup"><span data-stu-id="f0c94-114">message</span></span>  | <span data-ttu-id="f0c94-115">String</span><span class="sxs-lookup"><span data-stu-id="f0c94-115">String</span></span> | <span data-ttu-id="f0c94-116">邮件。</span><span class="sxs-lookup"><span data-stu-id="f0c94-116">The message.</span></span>         |
| <span data-ttu-id="f0c94-117">subcode</span><span class="sxs-lookup"><span data-stu-id="f0c94-117">subcode</span></span>  | <span data-ttu-id="f0c94-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f0c94-118">Int32</span></span> | <span data-ttu-id="f0c94-119">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="f0c94-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0c94-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0c94-120">JSON representation</span></span>

<span data-ttu-id="f0c94-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0c94-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
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
