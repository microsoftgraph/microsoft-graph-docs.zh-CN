---
title: genericError 资源类型
description: 通用错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 611671cc6e35fa9376bff2761719c58f0255f19d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129448"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="0c9a5-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c9a5-103">genericError resource type</span></span>

<span data-ttu-id="0c9a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c9a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c9a5-105">通用错误。</span><span class="sxs-lookup"><span data-stu-id="0c9a5-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="0c9a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c9a5-106">Properties</span></span>

| <span data-ttu-id="0c9a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c9a5-107">Property</span></span> | <span data-ttu-id="0c9a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="0c9a5-108">Type</span></span> | <span data-ttu-id="0c9a5-109">描述</span><span class="sxs-lookup"><span data-stu-id="0c9a5-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="0c9a5-110">message</span><span class="sxs-lookup"><span data-stu-id="0c9a5-110">message</span></span> | <span data-ttu-id="0c9a5-111">String</span><span class="sxs-lookup"><span data-stu-id="0c9a5-111">String</span></span> | <span data-ttu-id="0c9a5-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="0c9a5-112">The error message.</span></span> |
| <span data-ttu-id="0c9a5-113">code</span><span class="sxs-lookup"><span data-stu-id="0c9a5-113">code</span></span> | <span data-ttu-id="0c9a5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0c9a5-114">String</span></span> | <span data-ttu-id="0c9a5-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="0c9a5-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0c9a5-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c9a5-116">JSON representation</span></span>

<span data-ttu-id="0c9a5-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c9a5-117">Here is a JSON representation of the resource.</span></span>

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


