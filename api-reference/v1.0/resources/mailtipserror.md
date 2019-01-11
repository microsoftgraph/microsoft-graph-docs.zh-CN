---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: a4916bc34d7c76dc6c6592ee03e64b20a6485190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892091"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="69a48-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="69a48-103">mailTipsError resource type</span></span>

<span data-ttu-id="69a48-104">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="69a48-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="69a48-105">属性</span><span class="sxs-lookup"><span data-stu-id="69a48-105">Properties</span></span>
| <span data-ttu-id="69a48-106">属性</span><span class="sxs-lookup"><span data-stu-id="69a48-106">Property</span></span>     | <span data-ttu-id="69a48-107">类型</span><span class="sxs-lookup"><span data-stu-id="69a48-107">Type</span></span>   |<span data-ttu-id="69a48-108">Description</span><span class="sxs-lookup"><span data-stu-id="69a48-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="69a48-109">message</span><span class="sxs-lookup"><span data-stu-id="69a48-109">message</span></span> | <span data-ttu-id="69a48-110">字符串</span><span class="sxs-lookup"><span data-stu-id="69a48-110">String</span></span> | <span data-ttu-id="69a48-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="69a48-111">The error message.</span></span> |
| <span data-ttu-id="69a48-112">code</span><span class="sxs-lookup"><span data-stu-id="69a48-112">code</span></span> | <span data-ttu-id="69a48-113">字符串</span><span class="sxs-lookup"><span data-stu-id="69a48-113">String</span></span> | <span data-ttu-id="69a48-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="69a48-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69a48-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69a48-115">JSON representation</span></span>

<span data-ttu-id="69a48-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69a48-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
