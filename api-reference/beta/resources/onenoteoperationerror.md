---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 78e0ab763f27d17cf926795459b4e4a25cdf8e71
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522054"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="a555a-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="a555a-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a555a-104">失败的 OneNote 操作中的错误</span><span class="sxs-lookup"><span data-stu-id="a555a-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a555a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a555a-105">JSON representation</span></span>

<span data-ttu-id="a555a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a555a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a555a-107">属性</span><span class="sxs-lookup"><span data-stu-id="a555a-107">Properties</span></span>
| <span data-ttu-id="a555a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a555a-108">Property</span></span>     | <span data-ttu-id="a555a-109">类型</span><span class="sxs-lookup"><span data-stu-id="a555a-109">Type</span></span>   |<span data-ttu-id="a555a-110">说明</span><span class="sxs-lookup"><span data-stu-id="a555a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a555a-111">code</span><span class="sxs-lookup"><span data-stu-id="a555a-111">code</span></span>|<span data-ttu-id="a555a-112">string</span><span class="sxs-lookup"><span data-stu-id="a555a-112">string</span></span>|<span data-ttu-id="a555a-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="a555a-113">The error code.</span></span>|
|<span data-ttu-id="a555a-114">消息</span><span class="sxs-lookup"><span data-stu-id="a555a-114">message</span></span>|<span data-ttu-id="a555a-115">string</span><span class="sxs-lookup"><span data-stu-id="a555a-115">string</span></span>|<span data-ttu-id="a555a-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="a555a-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
