---
title: resultInfo 资源类型
description: ResultInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: acc01a17420390343c3eb1f866761d54d5c81c79
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006548"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="47c62-103">resultInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="47c62-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47c62-104">ResultInfo 类型。</span><span class="sxs-lookup"><span data-stu-id="47c62-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="47c62-105">属性</span><span class="sxs-lookup"><span data-stu-id="47c62-105">Properties</span></span>

| <span data-ttu-id="47c62-106">属性</span><span class="sxs-lookup"><span data-stu-id="47c62-106">Property</span></span> | <span data-ttu-id="47c62-107">类型</span><span class="sxs-lookup"><span data-stu-id="47c62-107">Type</span></span>   | <span data-ttu-id="47c62-108">说明</span><span class="sxs-lookup"><span data-stu-id="47c62-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="47c62-109">code</span><span class="sxs-lookup"><span data-stu-id="47c62-109">code</span></span>     | <span data-ttu-id="47c62-110">Int32</span><span class="sxs-lookup"><span data-stu-id="47c62-110">Int32</span></span> | <span data-ttu-id="47c62-111">结果代码。</span><span class="sxs-lookup"><span data-stu-id="47c62-111">The result code.</span></span>     |
| <span data-ttu-id="47c62-112">message</span><span class="sxs-lookup"><span data-stu-id="47c62-112">message</span></span>  | <span data-ttu-id="47c62-113">String</span><span class="sxs-lookup"><span data-stu-id="47c62-113">String</span></span> | <span data-ttu-id="47c62-114">邮件。</span><span class="sxs-lookup"><span data-stu-id="47c62-114">The message.</span></span>         |
| <span data-ttu-id="47c62-115">subcode</span><span class="sxs-lookup"><span data-stu-id="47c62-115">subcode</span></span>  | <span data-ttu-id="47c62-116">Int32</span><span class="sxs-lookup"><span data-stu-id="47c62-116">Int32</span></span> | <span data-ttu-id="47c62-117">结果子代码。</span><span class="sxs-lookup"><span data-stu-id="47c62-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47c62-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47c62-118">JSON representation</span></span>

<span data-ttu-id="47c62-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47c62-119">The following is a JSON representation of the resource.</span></span>

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
