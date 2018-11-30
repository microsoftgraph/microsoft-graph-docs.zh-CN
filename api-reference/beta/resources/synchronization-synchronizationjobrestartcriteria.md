---
title: synchronizationJobRestartCriteria 资源类型
description: 定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。
ms.openlocfilehash: edf5cf258750df72dda2c9754d3543e07fc32e39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041881"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="9f293-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f293-103">synchronizationJobRestartCriteria resource type</span></span>

> <span data-ttu-id="9f293-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f293-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f293-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f293-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f293-106">定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。</span><span class="sxs-lookup"><span data-stu-id="9f293-106">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="9f293-107">属性</span><span class="sxs-lookup"><span data-stu-id="9f293-107">Properties</span></span>
| <span data-ttu-id="9f293-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f293-108">Property</span></span>     | <span data-ttu-id="9f293-109">类型</span><span class="sxs-lookup"><span data-stu-id="9f293-109">Type</span></span>   |<span data-ttu-id="9f293-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f293-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f293-111">resetScope</span><span class="sxs-lookup"><span data-stu-id="9f293-111">resetScope</span></span>|<span data-ttu-id="9f293-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9f293-112">String</span></span>| <span data-ttu-id="9f293-113">以逗号分隔的下列值的组合： `Full`， `QuarantineState`， `Watermark`， `Escrows`， `ConnectorDataStore`。</span><span class="sxs-lookup"><span data-stu-id="9f293-113">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="9f293-114">使用`Full`如果希望所有选项。</span><span class="sxs-lookup"><span data-stu-id="9f293-114">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f293-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f293-115">JSON representation</span></span>

<span data-ttu-id="9f293-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f293-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->