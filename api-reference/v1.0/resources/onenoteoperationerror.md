---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 95eda3299b62a1ebe49b2520206265cc14c3ac57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035768"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="0c02f-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c02f-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="0c02f-104">失败的 OneNote 操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="0c02f-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c02f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c02f-105">JSON representation</span></span>

<span data-ttu-id="0c02f-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c02f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0c02f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c02f-107">Properties</span></span>
| <span data-ttu-id="0c02f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c02f-108">Property</span></span>     | <span data-ttu-id="0c02f-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c02f-109">Type</span></span>   |<span data-ttu-id="0c02f-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c02f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c02f-111">code</span><span class="sxs-lookup"><span data-stu-id="0c02f-111">code</span></span>|<span data-ttu-id="0c02f-112">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-112">string</span></span>|<span data-ttu-id="0c02f-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="0c02f-113">The error code.</span></span>|
|<span data-ttu-id="0c02f-114">message</span><span class="sxs-lookup"><span data-stu-id="0c02f-114">message</span></span>|<span data-ttu-id="0c02f-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0c02f-115">string</span></span>|<span data-ttu-id="0c02f-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="0c02f-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
