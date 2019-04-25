---
title: importStatusModel 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: c3fe64245d0fbce98db3ba87c3c39694e998c7e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548521"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="f5799-103">importStatusModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5799-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="f5799-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5799-104">JSON representation</span></span>

<span data-ttu-id="f5799-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5799-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f5799-106">属性</span><span class="sxs-lookup"><span data-stu-id="f5799-106">Properties</span></span>
| <span data-ttu-id="f5799-107">属性</span><span class="sxs-lookup"><span data-stu-id="f5799-107">Property</span></span>     | <span data-ttu-id="f5799-108">类型</span><span class="sxs-lookup"><span data-stu-id="f5799-108">Type</span></span>   |<span data-ttu-id="f5799-109">说明</span><span class="sxs-lookup"><span data-stu-id="f5799-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5799-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5799-110">createdDateTime</span></span>| <span data-ttu-id="f5799-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5799-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="f5799-112">id</span><span class="sxs-lookup"><span data-stu-id="f5799-112">id</span></span>|<span data-ttu-id="f5799-113">string</span><span class="sxs-lookup"><span data-stu-id="f5799-113">string</span></span>||
|<span data-ttu-id="f5799-114">status</span><span class="sxs-lookup"><span data-stu-id="f5799-114">status</span></span>|<span data-ttu-id="f5799-115">string</span><span class="sxs-lookup"><span data-stu-id="f5799-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/importstatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
