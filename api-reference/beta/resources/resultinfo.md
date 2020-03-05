---
title: resultInfo 资源类型
description: 包含成功和失败的特定结果信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521080"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="4f1ea-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f1ea-103">resultInfo resource type</span></span>

<span data-ttu-id="4f1ea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4f1ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f1ea-105">包含成功和失败的特定结果信息。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-105">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="4f1ea-106">该代码指定结果是否为一般性成功或失败。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-106">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="4f1ea-107">子代码提供与成功或失败类型相关的补充信息（例如，呼叫转移成功）。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-107">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="4f1ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f1ea-108">Properties</span></span>

| <span data-ttu-id="4f1ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="4f1ea-109">Property</span></span> | <span data-ttu-id="4f1ea-110">类型</span><span class="sxs-lookup"><span data-stu-id="4f1ea-110">Type</span></span>   | <span data-ttu-id="4f1ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f1ea-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="4f1ea-112">code</span><span class="sxs-lookup"><span data-stu-id="4f1ea-112">code</span></span>     | <span data-ttu-id="4f1ea-113">Int32</span><span class="sxs-lookup"><span data-stu-id="4f1ea-113">Int32</span></span> | <span data-ttu-id="4f1ea-114">结果代码。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-114">The result code.</span></span>     |
| <span data-ttu-id="4f1ea-115">message</span><span class="sxs-lookup"><span data-stu-id="4f1ea-115">message</span></span>  | <span data-ttu-id="4f1ea-116">String</span><span class="sxs-lookup"><span data-stu-id="4f1ea-116">String</span></span> | <span data-ttu-id="4f1ea-117">邮件。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-117">The message.</span></span>         |
| <span data-ttu-id="4f1ea-118">subcode</span><span class="sxs-lookup"><span data-stu-id="4f1ea-118">subcode</span></span>  | <span data-ttu-id="4f1ea-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4f1ea-119">Int32</span></span> | <span data-ttu-id="4f1ea-120">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f1ea-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f1ea-121">JSON representation</span></span>

<span data-ttu-id="4f1ea-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f1ea-122">The following is a JSON representation of the resource.</span></span>

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
