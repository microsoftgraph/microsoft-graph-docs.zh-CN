---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: ee4f6a09f3baec827d5ec2627edb7de89a878945
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973937"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="5fa92-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fa92-103">genericError resource type</span></span>

<span data-ttu-id="5fa92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fa92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fa92-105">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="5fa92-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="5fa92-106">属性</span><span class="sxs-lookup"><span data-stu-id="5fa92-106">Properties</span></span>

| <span data-ttu-id="5fa92-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fa92-107">Property</span></span> | <span data-ttu-id="5fa92-108">类型</span><span class="sxs-lookup"><span data-stu-id="5fa92-108">Type</span></span> | <span data-ttu-id="5fa92-109">描述</span><span class="sxs-lookup"><span data-stu-id="5fa92-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5fa92-110">message</span><span class="sxs-lookup"><span data-stu-id="5fa92-110">message</span></span> | <span data-ttu-id="5fa92-111">String</span><span class="sxs-lookup"><span data-stu-id="5fa92-111">String</span></span> | <span data-ttu-id="5fa92-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="5fa92-112">The error message.</span></span> |
| <span data-ttu-id="5fa92-113">code</span><span class="sxs-lookup"><span data-stu-id="5fa92-113">code</span></span> | <span data-ttu-id="5fa92-114">String</span><span class="sxs-lookup"><span data-stu-id="5fa92-114">String</span></span> | <span data-ttu-id="5fa92-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="5fa92-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5fa92-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fa92-116">JSON representation</span></span>

<span data-ttu-id="5fa92-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fa92-117">Here is a JSON representation of the resource.</span></span>

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


