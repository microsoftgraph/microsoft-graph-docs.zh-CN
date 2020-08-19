---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: d9c1245e89672fab3fa9cc22c87d677fd7ab9bf9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809523"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="e6af2-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6af2-103">genericError resource type</span></span>

<span data-ttu-id="e6af2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6af2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6af2-105">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="e6af2-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="e6af2-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6af2-106">Properties</span></span>

| <span data-ttu-id="e6af2-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6af2-107">Property</span></span> | <span data-ttu-id="e6af2-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6af2-108">Type</span></span> | <span data-ttu-id="e6af2-109">描述</span><span class="sxs-lookup"><span data-stu-id="e6af2-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e6af2-110">message</span><span class="sxs-lookup"><span data-stu-id="e6af2-110">message</span></span> | <span data-ttu-id="e6af2-111">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-111">String</span></span> | <span data-ttu-id="e6af2-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="e6af2-112">The error message.</span></span> |
| <span data-ttu-id="e6af2-113">code</span><span class="sxs-lookup"><span data-stu-id="e6af2-113">code</span></span> | <span data-ttu-id="e6af2-114">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-114">String</span></span> | <span data-ttu-id="e6af2-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="e6af2-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6af2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6af2-116">JSON representation</span></span>

<span data-ttu-id="e6af2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6af2-117">Here is a JSON representation of the resource.</span></span>

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
