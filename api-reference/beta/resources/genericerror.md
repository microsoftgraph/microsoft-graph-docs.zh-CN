---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4c68fa52046ccb48645aab1fbf2de4a772665328
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497641"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="8994c-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="8994c-103">genericError resource type</span></span>

<span data-ttu-id="8994c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8994c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8994c-105">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="8994c-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="8994c-106">属性</span><span class="sxs-lookup"><span data-stu-id="8994c-106">Properties</span></span>

| <span data-ttu-id="8994c-107">属性</span><span class="sxs-lookup"><span data-stu-id="8994c-107">Property</span></span> | <span data-ttu-id="8994c-108">类型</span><span class="sxs-lookup"><span data-stu-id="8994c-108">Type</span></span> | <span data-ttu-id="8994c-109">描述</span><span class="sxs-lookup"><span data-stu-id="8994c-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8994c-110">message</span><span class="sxs-lookup"><span data-stu-id="8994c-110">message</span></span> | <span data-ttu-id="8994c-111">String</span><span class="sxs-lookup"><span data-stu-id="8994c-111">String</span></span> | <span data-ttu-id="8994c-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="8994c-112">The error message.</span></span> |
| <span data-ttu-id="8994c-113">code</span><span class="sxs-lookup"><span data-stu-id="8994c-113">code</span></span> | <span data-ttu-id="8994c-114">String</span><span class="sxs-lookup"><span data-stu-id="8994c-114">String</span></span> | <span data-ttu-id="8994c-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="8994c-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8994c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8994c-116">JSON representation</span></span>

<span data-ttu-id="8994c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8994c-117">Here is a JSON representation of the resource.</span></span>

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
