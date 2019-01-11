---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837336"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="eb4b2-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb4b2-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="eb4b2-104">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="eb4b2-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb4b2-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb4b2-105">JSON representation</span></span>

<span data-ttu-id="eb4b2-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb4b2-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="eb4b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb4b2-107">Properties</span></span>
| <span data-ttu-id="eb4b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb4b2-108">Property</span></span>     | <span data-ttu-id="eb4b2-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb4b2-109">Type</span></span>   |<span data-ttu-id="eb4b2-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb4b2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb4b2-111">code</span><span class="sxs-lookup"><span data-stu-id="eb4b2-111">code</span></span>|<span data-ttu-id="eb4b2-112">string</span><span class="sxs-lookup"><span data-stu-id="eb4b2-112">string</span></span>|<span data-ttu-id="eb4b2-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="eb4b2-113">The error code.</span></span>|
|<span data-ttu-id="eb4b2-114">消息</span><span class="sxs-lookup"><span data-stu-id="eb4b2-114">message</span></span>|<span data-ttu-id="eb4b2-115">string</span><span class="sxs-lookup"><span data-stu-id="eb4b2-115">string</span></span>|<span data-ttu-id="eb4b2-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="eb4b2-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
