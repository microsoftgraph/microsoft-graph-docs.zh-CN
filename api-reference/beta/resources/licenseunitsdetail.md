---
title: licenseUnitsDetail 资源类型
description: subscribedSku 实体的 prepaidUnits 属性为 licenseUnitsDetail 类型。
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511315"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="567c6-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="567c6-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="567c6-104">[subscribedSku](subscribedsku.md) 实体的 **prepaidUnits** 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="567c6-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="567c6-105">属性</span><span class="sxs-lookup"><span data-stu-id="567c6-105">Properties</span></span>
| <span data-ttu-id="567c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="567c6-106">Property</span></span>     | <span data-ttu-id="567c6-107">类型</span><span class="sxs-lookup"><span data-stu-id="567c6-107">Type</span></span>   |<span data-ttu-id="567c6-108">说明</span><span class="sxs-lookup"><span data-stu-id="567c6-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="567c6-109">已启用</span><span class="sxs-lookup"><span data-stu-id="567c6-109">enabled</span></span>|<span data-ttu-id="567c6-110">Int32</span><span class="sxs-lookup"><span data-stu-id="567c6-110">Int32</span></span>| <span data-ttu-id="567c6-111">已启用的单元数。</span><span class="sxs-lookup"><span data-stu-id="567c6-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="567c6-112">suspended</span><span class="sxs-lookup"><span data-stu-id="567c6-112">suspended</span></span>|<span data-ttu-id="567c6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="567c6-113">Int32</span></span>| <span data-ttu-id="567c6-114">已挂起的单元数。</span><span class="sxs-lookup"><span data-stu-id="567c6-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="567c6-115">warning</span><span class="sxs-lookup"><span data-stu-id="567c6-115">warning</span></span>|<span data-ttu-id="567c6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="567c6-116">Int32</span></span>| <span data-ttu-id="567c6-117">处于警告状态的单元数。</span><span class="sxs-lookup"><span data-stu-id="567c6-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="567c6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="567c6-118">JSON representation</span></span>

<span data-ttu-id="567c6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="567c6-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
