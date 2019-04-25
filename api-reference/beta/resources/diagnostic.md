---
title: 诊断资源类型
description: 有关 OneNote 操作的错误或警告的信息。
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535212"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="5e25d-103">诊断资源类型</span><span class="sxs-lookup"><span data-stu-id="5e25d-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e25d-104">有关 OneNote 操作的错误或警告的信息。</span><span class="sxs-lookup"><span data-stu-id="5e25d-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e25d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e25d-105">JSON representation</span></span>

<span data-ttu-id="5e25d-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e25d-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5e25d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5e25d-107">Properties</span></span>
| <span data-ttu-id="5e25d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e25d-108">Property</span></span>     | <span data-ttu-id="5e25d-109">类型</span><span class="sxs-lookup"><span data-stu-id="5e25d-109">Type</span></span>   |<span data-ttu-id="5e25d-110">描述</span><span class="sxs-lookup"><span data-stu-id="5e25d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e25d-111">message</span><span class="sxs-lookup"><span data-stu-id="5e25d-111">message</span></span>|<span data-ttu-id="5e25d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="5e25d-112">String</span></span>|<span data-ttu-id="5e25d-113">描述触发错误或警告的条件的消息。</span><span class="sxs-lookup"><span data-stu-id="5e25d-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="5e25d-114">url</span><span class="sxs-lookup"><span data-stu-id="5e25d-114">url</span></span>|<span data-ttu-id="5e25d-115">String</span><span class="sxs-lookup"><span data-stu-id="5e25d-115">String</span></span>|<span data-ttu-id="5e25d-116">有关此问题的文档的链接。</span><span class="sxs-lookup"><span data-stu-id="5e25d-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
