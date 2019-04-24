---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
ms.openlocfilehash: 8c2a4e995c7e1afa63b7f9daea6b61cbaf974958
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519905"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="a92b7-103">licenseUnitsDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="a92b7-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a92b7-104">**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。</span><span class="sxs-lookup"><span data-stu-id="a92b7-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="a92b7-105">属性</span><span class="sxs-lookup"><span data-stu-id="a92b7-105">Properties</span></span>
| <span data-ttu-id="a92b7-106">属性</span><span class="sxs-lookup"><span data-stu-id="a92b7-106">Property</span></span>     | <span data-ttu-id="a92b7-107">类型</span><span class="sxs-lookup"><span data-stu-id="a92b7-107">Type</span></span>   |<span data-ttu-id="a92b7-108">说明</span><span class="sxs-lookup"><span data-stu-id="a92b7-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="a92b7-109">已启用</span><span class="sxs-lookup"><span data-stu-id="a92b7-109">enabled</span></span>|<span data-ttu-id="a92b7-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a92b7-110">Int32</span></span>| <span data-ttu-id="a92b7-111">启用的单位数。</span><span class="sxs-lookup"><span data-stu-id="a92b7-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="a92b7-112">已挂起</span><span class="sxs-lookup"><span data-stu-id="a92b7-112">suspended</span></span>|<span data-ttu-id="a92b7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a92b7-113">Int32</span></span>| <span data-ttu-id="a92b7-114">挂起的单位数。</span><span class="sxs-lookup"><span data-stu-id="a92b7-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="a92b7-115">警告</span><span class="sxs-lookup"><span data-stu-id="a92b7-115">warning</span></span>|<span data-ttu-id="a92b7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a92b7-116">Int32</span></span>| <span data-ttu-id="a92b7-117">处于警告状态的单位数。</span><span class="sxs-lookup"><span data-stu-id="a92b7-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a92b7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a92b7-118">JSON representation</span></span>

<span data-ttu-id="a92b7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a92b7-119">Here is a JSON representation of the resource</span></span>

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
