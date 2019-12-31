---
title: resultInfo 资源类型
description: 包含成功和失败的特定结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43a7dba5d758f8884285e7238e4e4fab0763409f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913721"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="f171e-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f171e-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f171e-104">包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="f171e-104">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="f171e-105">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="f171e-105">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="f171e-106">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）。</span><span class="sxs-lookup"><span data-stu-id="f171e-106">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="f171e-107">属性</span><span class="sxs-lookup"><span data-stu-id="f171e-107">Properties</span></span>

| <span data-ttu-id="f171e-108">属性</span><span class="sxs-lookup"><span data-stu-id="f171e-108">Property</span></span> | <span data-ttu-id="f171e-109">类型</span><span class="sxs-lookup"><span data-stu-id="f171e-109">Type</span></span>   | <span data-ttu-id="f171e-110">说明</span><span class="sxs-lookup"><span data-stu-id="f171e-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="f171e-111">code</span><span class="sxs-lookup"><span data-stu-id="f171e-111">code</span></span>     | <span data-ttu-id="f171e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f171e-112">Int32</span></span> | <span data-ttu-id="f171e-113">结果代码。</span><span class="sxs-lookup"><span data-stu-id="f171e-113">The result code.</span></span>     |
| <span data-ttu-id="f171e-114">message</span><span class="sxs-lookup"><span data-stu-id="f171e-114">message</span></span>  | <span data-ttu-id="f171e-115">String</span><span class="sxs-lookup"><span data-stu-id="f171e-115">String</span></span> | <span data-ttu-id="f171e-116">邮件。</span><span class="sxs-lookup"><span data-stu-id="f171e-116">The message.</span></span>         |
| <span data-ttu-id="f171e-117">subcode</span><span class="sxs-lookup"><span data-stu-id="f171e-117">subcode</span></span>  | <span data-ttu-id="f171e-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f171e-118">Int32</span></span> | <span data-ttu-id="f171e-119">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="f171e-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f171e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f171e-120">JSON representation</span></span>

<span data-ttu-id="f171e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f171e-121">The following is a JSON representation of the resource.</span></span>

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
