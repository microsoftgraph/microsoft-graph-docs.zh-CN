---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 499949c5995025e9327e1f662365b0c5e43c80f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574003"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="92be8-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="92be8-103">mailTipsError resource type</span></span>

<span data-ttu-id="92be8-104">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="92be8-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="92be8-105">属性</span><span class="sxs-lookup"><span data-stu-id="92be8-105">Properties</span></span>
| <span data-ttu-id="92be8-106">属性</span><span class="sxs-lookup"><span data-stu-id="92be8-106">Property</span></span>     | <span data-ttu-id="92be8-107">类型</span><span class="sxs-lookup"><span data-stu-id="92be8-107">Type</span></span>   |<span data-ttu-id="92be8-108">描述</span><span class="sxs-lookup"><span data-stu-id="92be8-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="92be8-109">message</span><span class="sxs-lookup"><span data-stu-id="92be8-109">message</span></span> | <span data-ttu-id="92be8-110">String</span><span class="sxs-lookup"><span data-stu-id="92be8-110">String</span></span> | <span data-ttu-id="92be8-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="92be8-111">The error message.</span></span> |
| <span data-ttu-id="92be8-112">code</span><span class="sxs-lookup"><span data-stu-id="92be8-112">code</span></span> | <span data-ttu-id="92be8-113">String</span><span class="sxs-lookup"><span data-stu-id="92be8-113">String</span></span> | <span data-ttu-id="92be8-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="92be8-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92be8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92be8-115">JSON representation</span></span>

<span data-ttu-id="92be8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92be8-116">Here is a JSON representation of the resource.</span></span>

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
