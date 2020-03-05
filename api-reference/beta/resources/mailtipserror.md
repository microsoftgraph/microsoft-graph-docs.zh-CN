---
title: mailTipsError 资源类型
description: 操作过程中发生的错误。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5ffb76a1dd8d047170ff50231858b1a94fd244ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522804"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="acdda-103">mailTipsError 资源类型</span><span class="sxs-lookup"><span data-stu-id="acdda-103">mailTipsError resource type</span></span>

<span data-ttu-id="acdda-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="acdda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acdda-105">操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="acdda-105">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="acdda-106">属性</span><span class="sxs-lookup"><span data-stu-id="acdda-106">Properties</span></span>
| <span data-ttu-id="acdda-107">属性</span><span class="sxs-lookup"><span data-stu-id="acdda-107">Property</span></span>     | <span data-ttu-id="acdda-108">类型</span><span class="sxs-lookup"><span data-stu-id="acdda-108">Type</span></span>   |<span data-ttu-id="acdda-109">描述</span><span class="sxs-lookup"><span data-stu-id="acdda-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="acdda-110">message</span><span class="sxs-lookup"><span data-stu-id="acdda-110">message</span></span> | <span data-ttu-id="acdda-111">String</span><span class="sxs-lookup"><span data-stu-id="acdda-111">String</span></span> | <span data-ttu-id="acdda-112">错误消息。</span><span class="sxs-lookup"><span data-stu-id="acdda-112">The error message.</span></span> |
| <span data-ttu-id="acdda-113">code</span><span class="sxs-lookup"><span data-stu-id="acdda-113">code</span></span> | <span data-ttu-id="acdda-114">String</span><span class="sxs-lookup"><span data-stu-id="acdda-114">String</span></span> | <span data-ttu-id="acdda-115">错误代码。</span><span class="sxs-lookup"><span data-stu-id="acdda-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="acdda-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acdda-116">JSON representation</span></span>

<span data-ttu-id="acdda-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acdda-117">Here is a JSON representation of the resource.</span></span>

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
