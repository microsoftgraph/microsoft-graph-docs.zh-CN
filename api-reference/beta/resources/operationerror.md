---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: 2419d4230e5618f601a5d8fe0743ec9ef807cf00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809320"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="13270-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="13270-103">operationError resource type</span></span>

<span data-ttu-id="13270-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13270-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13270-105">描述 [teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="13270-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="13270-106">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="13270-106">operationError Properties</span></span>
| <span data-ttu-id="13270-107">属性</span><span class="sxs-lookup"><span data-stu-id="13270-107">Property</span></span>     | <span data-ttu-id="13270-108">类型</span><span class="sxs-lookup"><span data-stu-id="13270-108">Type</span></span>   |<span data-ttu-id="13270-109">说明</span><span class="sxs-lookup"><span data-stu-id="13270-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13270-110">code</span><span class="sxs-lookup"><span data-stu-id="13270-110">code</span></span>|<span data-ttu-id="13270-111">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="13270-111">string (readonly)</span></span>|<span data-ttu-id="13270-112">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="13270-112">Operation error code.</span></span>|
|<span data-ttu-id="13270-113">message</span><span class="sxs-lookup"><span data-stu-id="13270-113">message</span></span>|<span data-ttu-id="13270-114">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="13270-114">string (readonly)</span></span>|<span data-ttu-id="13270-115">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="13270-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13270-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13270-116">JSON representation</span></span>

<span data-ttu-id="13270-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13270-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
