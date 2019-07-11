---
title: synchronizationJobRestartCriteria 资源类型
description: '定义[synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md)操作的范围。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fda28a84f568b9d535a06226397375f3fa8e444a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620722"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="9a116-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a116-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a116-104">定义[synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md)操作的范围。</span><span class="sxs-lookup"><span data-stu-id="9a116-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="9a116-105">属性</span><span class="sxs-lookup"><span data-stu-id="9a116-105">Properties</span></span>
| <span data-ttu-id="9a116-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a116-106">Property</span></span>     | <span data-ttu-id="9a116-107">类型</span><span class="sxs-lookup"><span data-stu-id="9a116-107">Type</span></span>   |<span data-ttu-id="9a116-108">说明</span><span class="sxs-lookup"><span data-stu-id="9a116-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a116-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="9a116-109">resetScope</span></span>|<span data-ttu-id="9a116-110">String</span><span class="sxs-lookup"><span data-stu-id="9a116-110">String</span></span>| <span data-ttu-id="9a116-111">以下`Full`值的逗号分隔组合:、 `QuarantineState` `Watermark` `Escrows`、、。 `ConnectorDataStore`</span><span class="sxs-lookup"><span data-stu-id="9a116-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="9a116-112">如果`Full`您想要所有选项, 请使用。</span><span class="sxs-lookup"><span data-stu-id="9a116-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a116-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a116-113">JSON representation</span></span>

<span data-ttu-id="9a116-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a116-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
