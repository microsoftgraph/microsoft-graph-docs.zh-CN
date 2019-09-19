---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bddfdaba2456f44a0cea2688109abbf152af291f
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036429"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="e1311-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1311-103">genericError resource type</span></span>

<span data-ttu-id="e1311-104">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="e1311-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="e1311-105">属性</span><span class="sxs-lookup"><span data-stu-id="e1311-105">Properties</span></span>

| <span data-ttu-id="e1311-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1311-106">Property</span></span> | <span data-ttu-id="e1311-107">类型</span><span class="sxs-lookup"><span data-stu-id="e1311-107">Type</span></span> | <span data-ttu-id="e1311-108">描述</span><span class="sxs-lookup"><span data-stu-id="e1311-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e1311-109">message</span><span class="sxs-lookup"><span data-stu-id="e1311-109">message</span></span> | <span data-ttu-id="e1311-110">String</span><span class="sxs-lookup"><span data-stu-id="e1311-110">String</span></span> | <span data-ttu-id="e1311-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="e1311-111">The error message.</span></span> |
| <span data-ttu-id="e1311-112">code</span><span class="sxs-lookup"><span data-stu-id="e1311-112">code</span></span> | <span data-ttu-id="e1311-113">String</span><span class="sxs-lookup"><span data-stu-id="e1311-113">String</span></span> | <span data-ttu-id="e1311-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="e1311-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e1311-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1311-115">JSON representation</span></span>

<span data-ttu-id="e1311-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1311-116">Here is a JSON representation of the resource.</span></span>

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
