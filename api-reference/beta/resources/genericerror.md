---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 701a3b7ed0d7bad6e33f8ba41e77ec7340a57146
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973523"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="825fb-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="825fb-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="825fb-104">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="825fb-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="825fb-105">属性</span><span class="sxs-lookup"><span data-stu-id="825fb-105">Properties</span></span>

| <span data-ttu-id="825fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="825fb-106">Property</span></span> | <span data-ttu-id="825fb-107">类型</span><span class="sxs-lookup"><span data-stu-id="825fb-107">Type</span></span> | <span data-ttu-id="825fb-108">描述</span><span class="sxs-lookup"><span data-stu-id="825fb-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="825fb-109">message</span><span class="sxs-lookup"><span data-stu-id="825fb-109">message</span></span> | <span data-ttu-id="825fb-110">String</span><span class="sxs-lookup"><span data-stu-id="825fb-110">String</span></span> | <span data-ttu-id="825fb-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="825fb-111">The error message.</span></span> |
| <span data-ttu-id="825fb-112">code</span><span class="sxs-lookup"><span data-stu-id="825fb-112">code</span></span> | <span data-ttu-id="825fb-113">String</span><span class="sxs-lookup"><span data-stu-id="825fb-113">String</span></span> | <span data-ttu-id="825fb-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="825fb-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="825fb-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="825fb-115">JSON representation</span></span>

<span data-ttu-id="825fb-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="825fb-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
