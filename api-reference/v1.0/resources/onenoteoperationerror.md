---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
ms.openlocfilehash: 3e09bd4b4ec0a8fc36113c278ebe7cab25392ecf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008016"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="9f1f8-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f1f8-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="9f1f8-104">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="9f1f8-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f1f8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f1f8-105">JSON representation</span></span>

<span data-ttu-id="9f1f8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f1f8-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9f1f8-107">属性</span><span class="sxs-lookup"><span data-stu-id="9f1f8-107">Properties</span></span>
| <span data-ttu-id="9f1f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f1f8-108">Property</span></span>     | <span data-ttu-id="9f1f8-109">类型</span><span class="sxs-lookup"><span data-stu-id="9f1f8-109">Type</span></span>   |<span data-ttu-id="9f1f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f1f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f1f8-111">code</span><span class="sxs-lookup"><span data-stu-id="9f1f8-111">code</span></span>|<span data-ttu-id="9f1f8-112">string</span><span class="sxs-lookup"><span data-stu-id="9f1f8-112">string</span></span>|<span data-ttu-id="9f1f8-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="9f1f8-113">The error code.</span></span>|
|<span data-ttu-id="9f1f8-114">消息</span><span class="sxs-lookup"><span data-stu-id="9f1f8-114">message</span></span>|<span data-ttu-id="9f1f8-115">string</span><span class="sxs-lookup"><span data-stu-id="9f1f8-115">string</span></span>|<span data-ttu-id="9f1f8-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="9f1f8-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
