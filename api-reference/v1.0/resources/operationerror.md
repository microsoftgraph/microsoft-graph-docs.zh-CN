---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462604"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="ad70e-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad70e-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad70e-104">描述[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="ad70e-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="ad70e-105">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="ad70e-105">operationError Properties</span></span>
| <span data-ttu-id="ad70e-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad70e-106">Property</span></span>     | <span data-ttu-id="ad70e-107">类型</span><span class="sxs-lookup"><span data-stu-id="ad70e-107">Type</span></span>   |<span data-ttu-id="ad70e-108">说明</span><span class="sxs-lookup"><span data-stu-id="ad70e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad70e-109">code</span><span class="sxs-lookup"><span data-stu-id="ad70e-109">code</span></span>|<span data-ttu-id="ad70e-110">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="ad70e-110">string (readonly)</span></span>|<span data-ttu-id="ad70e-111">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="ad70e-111">Operation error code.</span></span>|
|<span data-ttu-id="ad70e-112">message</span><span class="sxs-lookup"><span data-stu-id="ad70e-112">message</span></span>|<span data-ttu-id="ad70e-113">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="ad70e-113">string (readonly)</span></span>|<span data-ttu-id="ad70e-114">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="ad70e-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad70e-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad70e-115">JSON representation</span></span>

<span data-ttu-id="ad70e-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad70e-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
