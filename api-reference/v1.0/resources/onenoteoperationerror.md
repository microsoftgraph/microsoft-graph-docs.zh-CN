---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3291f70e8cc18ee532f636feb1de9e8bb5751e02
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932460"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="69970-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="69970-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="69970-104">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="69970-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69970-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69970-105">JSON representation</span></span>

<span data-ttu-id="69970-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69970-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="69970-107">属性</span><span class="sxs-lookup"><span data-stu-id="69970-107">Properties</span></span>
| <span data-ttu-id="69970-108">属性</span><span class="sxs-lookup"><span data-stu-id="69970-108">Property</span></span>     | <span data-ttu-id="69970-109">类型</span><span class="sxs-lookup"><span data-stu-id="69970-109">Type</span></span>   |<span data-ttu-id="69970-110">说明</span><span class="sxs-lookup"><span data-stu-id="69970-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69970-111">code</span><span class="sxs-lookup"><span data-stu-id="69970-111">code</span></span>|<span data-ttu-id="69970-112">string</span><span class="sxs-lookup"><span data-stu-id="69970-112">string</span></span>|<span data-ttu-id="69970-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="69970-113">The error code.</span></span>|
|<span data-ttu-id="69970-114">消息</span><span class="sxs-lookup"><span data-stu-id="69970-114">message</span></span>|<span data-ttu-id="69970-115">string</span><span class="sxs-lookup"><span data-stu-id="69970-115">string</span></span>|<span data-ttu-id="69970-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="69970-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
