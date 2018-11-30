---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
ms.openlocfilehash: 8604207844ade4e0c10981f30d03b33eacf4a0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009187"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="d35df-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="d35df-103">mailTipsError resource type</span></span>

<span data-ttu-id="d35df-104">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="d35df-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="d35df-105">属性</span><span class="sxs-lookup"><span data-stu-id="d35df-105">Properties</span></span>
| <span data-ttu-id="d35df-106">属性</span><span class="sxs-lookup"><span data-stu-id="d35df-106">Property</span></span>     | <span data-ttu-id="d35df-107">类型</span><span class="sxs-lookup"><span data-stu-id="d35df-107">Type</span></span>   |<span data-ttu-id="d35df-108">说明</span><span class="sxs-lookup"><span data-stu-id="d35df-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d35df-109">message</span><span class="sxs-lookup"><span data-stu-id="d35df-109">message</span></span> | <span data-ttu-id="d35df-110">字符串</span><span class="sxs-lookup"><span data-stu-id="d35df-110">String</span></span> | <span data-ttu-id="d35df-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="d35df-111">The error message.</span></span> |
| <span data-ttu-id="d35df-112">code</span><span class="sxs-lookup"><span data-stu-id="d35df-112">code</span></span> | <span data-ttu-id="d35df-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d35df-113">String</span></span> | <span data-ttu-id="d35df-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="d35df-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d35df-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d35df-115">JSON representation</span></span>

<span data-ttu-id="d35df-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d35df-116">Here is a JSON representation of the resource.</span></span>

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