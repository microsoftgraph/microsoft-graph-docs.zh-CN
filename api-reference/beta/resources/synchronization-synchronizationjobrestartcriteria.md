---
title: synchronizationJobRestartCriteria 资源类型
description: 定义[synchronizationJob： restart](../api/synchronization_synchronizationjob_restart.md)操作的范围。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c8992104493e7f59b1ddc74c7128dda50b2bfd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520063"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="0cb57-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="0cb57-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="0cb57-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0cb57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb57-105">定义[synchronizationJob： restart](../api/synchronization-synchronizationjob-restart.md)操作的范围。</span><span class="sxs-lookup"><span data-stu-id="0cb57-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="0cb57-106">属性</span><span class="sxs-lookup"><span data-stu-id="0cb57-106">Properties</span></span>
| <span data-ttu-id="0cb57-107">属性</span><span class="sxs-lookup"><span data-stu-id="0cb57-107">Property</span></span>     | <span data-ttu-id="0cb57-108">类型</span><span class="sxs-lookup"><span data-stu-id="0cb57-108">Type</span></span>   |<span data-ttu-id="0cb57-109">说明</span><span class="sxs-lookup"><span data-stu-id="0cb57-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cb57-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="0cb57-110">resetScope</span></span>|<span data-ttu-id="0cb57-111">String</span><span class="sxs-lookup"><span data-stu-id="0cb57-111">String</span></span>| <span data-ttu-id="0cb57-112">以下`Full`值的逗号分隔组合：、 `QuarantineState` `Watermark` `Escrows`、、。 `ConnectorDataStore`</span><span class="sxs-lookup"><span data-stu-id="0cb57-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="0cb57-113">如果`Full`您想要所有选项，请使用。</span><span class="sxs-lookup"><span data-stu-id="0cb57-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cb57-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0cb57-114">JSON representation</span></span>

<span data-ttu-id="0cb57-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cb57-115">The following is a JSON representation of the resource.</span></span>

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
