---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3291f70e8cc18ee532f636feb1de9e8bb5751e02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462597"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="dad00-103">onenoteOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="dad00-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dad00-104">失败的 OneNote 操作中的错误。</span><span class="sxs-lookup"><span data-stu-id="dad00-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dad00-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dad00-105">JSON representation</span></span>

<span data-ttu-id="dad00-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dad00-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="dad00-107">属性</span><span class="sxs-lookup"><span data-stu-id="dad00-107">Properties</span></span>
| <span data-ttu-id="dad00-108">属性</span><span class="sxs-lookup"><span data-stu-id="dad00-108">Property</span></span>     | <span data-ttu-id="dad00-109">类型</span><span class="sxs-lookup"><span data-stu-id="dad00-109">Type</span></span>   |<span data-ttu-id="dad00-110">说明</span><span class="sxs-lookup"><span data-stu-id="dad00-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad00-111">code</span><span class="sxs-lookup"><span data-stu-id="dad00-111">code</span></span>|<span data-ttu-id="dad00-112">string</span><span class="sxs-lookup"><span data-stu-id="dad00-112">string</span></span>|<span data-ttu-id="dad00-113">错误代码。</span><span class="sxs-lookup"><span data-stu-id="dad00-113">The error code.</span></span>|
|<span data-ttu-id="dad00-114">message</span><span class="sxs-lookup"><span data-stu-id="dad00-114">message</span></span>|<span data-ttu-id="dad00-115">字符串</span><span class="sxs-lookup"><span data-stu-id="dad00-115">string</span></span>|<span data-ttu-id="dad00-116">错误消息。</span><span class="sxs-lookup"><span data-stu-id="dad00-116">The error message.</span></span>|

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
