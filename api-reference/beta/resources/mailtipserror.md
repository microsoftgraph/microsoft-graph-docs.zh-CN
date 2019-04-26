---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bcf56c3f5f090fd2f14f3556442e5c19ece9c6cf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342679"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="e335f-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="e335f-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e335f-104">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="e335f-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="e335f-105">属性</span><span class="sxs-lookup"><span data-stu-id="e335f-105">Properties</span></span>
| <span data-ttu-id="e335f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e335f-106">Property</span></span>     | <span data-ttu-id="e335f-107">类型</span><span class="sxs-lookup"><span data-stu-id="e335f-107">Type</span></span>   |<span data-ttu-id="e335f-108">描述</span><span class="sxs-lookup"><span data-stu-id="e335f-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="e335f-109">message</span><span class="sxs-lookup"><span data-stu-id="e335f-109">message</span></span> | <span data-ttu-id="e335f-110">String</span><span class="sxs-lookup"><span data-stu-id="e335f-110">String</span></span> | <span data-ttu-id="e335f-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="e335f-111">The error message.</span></span> |
| <span data-ttu-id="e335f-112">code</span><span class="sxs-lookup"><span data-stu-id="e335f-112">code</span></span> | <span data-ttu-id="e335f-113">String</span><span class="sxs-lookup"><span data-stu-id="e335f-113">String</span></span> | <span data-ttu-id="e335f-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="e335f-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e335f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e335f-115">JSON representation</span></span>

<span data-ttu-id="e335f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e335f-116">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
