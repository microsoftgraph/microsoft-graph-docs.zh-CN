---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8159fc93744c18205e3373780c128ca37242419f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041181"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="391ff-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="391ff-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="391ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="391ff-105">失败的 OneNote 操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="391ff-105">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="391ff-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="391ff-106">JSON representation</span></span>

<span data-ttu-id="391ff-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="391ff-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="391ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="391ff-108">Properties</span></span>
| <span data-ttu-id="391ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="391ff-109">Property</span></span>     | <span data-ttu-id="391ff-110">类型</span><span class="sxs-lookup"><span data-stu-id="391ff-110">Type</span></span>   |<span data-ttu-id="391ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="391ff-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="391ff-112">code</span><span class="sxs-lookup"><span data-stu-id="391ff-112">code</span></span>|<span data-ttu-id="391ff-113">string</span><span class="sxs-lookup"><span data-stu-id="391ff-113">string</span></span>|<span data-ttu-id="391ff-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="391ff-114">The error code.</span></span>|
|<span data-ttu-id="391ff-115">message</span><span class="sxs-lookup"><span data-stu-id="391ff-115">message</span></span>|<span data-ttu-id="391ff-116">字符串</span><span class="sxs-lookup"><span data-stu-id="391ff-116">string</span></span>|<span data-ttu-id="391ff-117">错误消息。</span><span class="sxs-lookup"><span data-stu-id="391ff-117">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

