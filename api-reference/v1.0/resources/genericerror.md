---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: b6601dc0975b12e0f21ecea9fa6e9e3063334ab1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018216"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="a0d1e-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d1e-103">genericError resource type</span></span>

<span data-ttu-id="a0d1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0d1e-105">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="a0d1e-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="a0d1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0d1e-106">Properties</span></span>

| <span data-ttu-id="a0d1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="a0d1e-107">Property</span></span> | <span data-ttu-id="a0d1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="a0d1e-108">Type</span></span> | <span data-ttu-id="a0d1e-109">描述</span><span class="sxs-lookup"><span data-stu-id="a0d1e-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a0d1e-110">message</span><span class="sxs-lookup"><span data-stu-id="a0d1e-110">message</span></span> | <span data-ttu-id="a0d1e-111">String</span><span class="sxs-lookup"><span data-stu-id="a0d1e-111">String</span></span> | <span data-ttu-id="a0d1e-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="a0d1e-112">The error message.</span></span> |
| <span data-ttu-id="a0d1e-113">code</span><span class="sxs-lookup"><span data-stu-id="a0d1e-113">code</span></span> | <span data-ttu-id="a0d1e-114">String</span><span class="sxs-lookup"><span data-stu-id="a0d1e-114">String</span></span> | <span data-ttu-id="a0d1e-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="a0d1e-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0d1e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d1e-116">JSON representation</span></span>

<span data-ttu-id="a0d1e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d1e-117">Here is a JSON representation of the resource.</span></span>

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

