---
title: operationError 资源类型
description: 介绍 teamsAsyncOperation 中的错误。
ms.openlocfilehash: 0207f490328d377fedab72d2a5300baaf3645150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043652"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="69724-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="69724-103">operationError resource type</span></span>

> <span data-ttu-id="69724-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69724-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69724-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69724-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69724-106">介绍[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="69724-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="69724-107">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="69724-107">operationError Properties</span></span>
| <span data-ttu-id="69724-108">属性</span><span class="sxs-lookup"><span data-stu-id="69724-108">Property</span></span>     | <span data-ttu-id="69724-109">类型</span><span class="sxs-lookup"><span data-stu-id="69724-109">Type</span></span>   |<span data-ttu-id="69724-110">说明</span><span class="sxs-lookup"><span data-stu-id="69724-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69724-111">code</span><span class="sxs-lookup"><span data-stu-id="69724-111">code</span></span>|<span data-ttu-id="69724-112">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="69724-112">string (readonly)</span></span>|<span data-ttu-id="69724-113">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="69724-113">Operation error code.</span></span>|
|<span data-ttu-id="69724-114">message</span><span class="sxs-lookup"><span data-stu-id="69724-114">message</span></span>|<span data-ttu-id="69724-115">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="69724-115">string (readonly)</span></span>|<span data-ttu-id="69724-116">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="69724-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69724-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69724-117">JSON representation</span></span>

<span data-ttu-id="69724-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69724-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
