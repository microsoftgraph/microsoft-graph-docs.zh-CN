---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 499949c5995025e9327e1f662365b0c5e43c80f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934203"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="24add-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="24add-103">mailTipsError resource type</span></span>

<span data-ttu-id="24add-104">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="24add-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="24add-105">属性</span><span class="sxs-lookup"><span data-stu-id="24add-105">Properties</span></span>
| <span data-ttu-id="24add-106">属性</span><span class="sxs-lookup"><span data-stu-id="24add-106">Property</span></span>     | <span data-ttu-id="24add-107">类型</span><span class="sxs-lookup"><span data-stu-id="24add-107">Type</span></span>   |<span data-ttu-id="24add-108">说明</span><span class="sxs-lookup"><span data-stu-id="24add-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="24add-109">message</span><span class="sxs-lookup"><span data-stu-id="24add-109">message</span></span> | <span data-ttu-id="24add-110">字符串</span><span class="sxs-lookup"><span data-stu-id="24add-110">String</span></span> | <span data-ttu-id="24add-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="24add-111">The error message.</span></span> |
| <span data-ttu-id="24add-112">code</span><span class="sxs-lookup"><span data-stu-id="24add-112">code</span></span> | <span data-ttu-id="24add-113">字符串</span><span class="sxs-lookup"><span data-stu-id="24add-113">String</span></span> | <span data-ttu-id="24add-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="24add-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24add-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24add-115">JSON representation</span></span>

<span data-ttu-id="24add-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24add-116">Here is a JSON representation of the resource.</span></span>

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
