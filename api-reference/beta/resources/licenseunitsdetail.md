---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581547"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="23c01-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="23c01-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23c01-104">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="23c01-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="23c01-105">属性</span><span class="sxs-lookup"><span data-stu-id="23c01-105">Properties</span></span>
| <span data-ttu-id="23c01-106">属性</span><span class="sxs-lookup"><span data-stu-id="23c01-106">Property</span></span>     | <span data-ttu-id="23c01-107">类型</span><span class="sxs-lookup"><span data-stu-id="23c01-107">Type</span></span>   |<span data-ttu-id="23c01-108">说明</span><span class="sxs-lookup"><span data-stu-id="23c01-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="23c01-109">已启用</span><span class="sxs-lookup"><span data-stu-id="23c01-109">enabled</span></span>|<span data-ttu-id="23c01-110">Int32</span><span class="sxs-lookup"><span data-stu-id="23c01-110">Int32</span></span>| <span data-ttu-id="23c01-111">启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="23c01-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="23c01-112">已挂起</span><span class="sxs-lookup"><span data-stu-id="23c01-112">suspended</span></span>|<span data-ttu-id="23c01-113">Int32</span><span class="sxs-lookup"><span data-stu-id="23c01-113">Int32</span></span>| <span data-ttu-id="23c01-114">挂起的单位数。</span><span class="sxs-lookup"><span data-stu-id="23c01-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="23c01-115">警告</span><span class="sxs-lookup"><span data-stu-id="23c01-115">warning</span></span>|<span data-ttu-id="23c01-116">Int32</span><span class="sxs-lookup"><span data-stu-id="23c01-116">Int32</span></span>| <span data-ttu-id="23c01-117">处于警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="23c01-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="23c01-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23c01-118">JSON representation</span></span>

<span data-ttu-id="23c01-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23c01-119">Here is a JSON representation of the resource</span></span>

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
