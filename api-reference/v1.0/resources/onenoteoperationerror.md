---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: Jewan-microsoft
ms.openlocfilehash: e31d47f9351a050eef134cde2f6a6a8bbdf526d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320690"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="d0f96-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0f96-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="d0f96-104">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="d0f96-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0f96-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0f96-105">JSON representation</span></span>

<span data-ttu-id="d0f96-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0f96-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d0f96-107">属性</span><span class="sxs-lookup"><span data-stu-id="d0f96-107">Properties</span></span>
| <span data-ttu-id="d0f96-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0f96-108">Property</span></span>     | <span data-ttu-id="d0f96-109">类型</span><span class="sxs-lookup"><span data-stu-id="d0f96-109">Type</span></span>   |<span data-ttu-id="d0f96-110">说明</span><span class="sxs-lookup"><span data-stu-id="d0f96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0f96-111">code</span><span class="sxs-lookup"><span data-stu-id="d0f96-111">code</span></span>|<span data-ttu-id="d0f96-112">string</span><span class="sxs-lookup"><span data-stu-id="d0f96-112">string</span></span>|<span data-ttu-id="d0f96-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="d0f96-113">The error code.</span></span>|
|<span data-ttu-id="d0f96-114">消息</span><span class="sxs-lookup"><span data-stu-id="d0f96-114">message</span></span>|<span data-ttu-id="d0f96-115">string</span><span class="sxs-lookup"><span data-stu-id="d0f96-115">string</span></span>|<span data-ttu-id="d0f96-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="d0f96-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
