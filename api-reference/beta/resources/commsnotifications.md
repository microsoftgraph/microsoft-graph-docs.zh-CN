---
title: commsNotifications 资源类型
description: 通信服务器用于在一个批处理中发送多个通知的通知列表。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 750c0d0a19e4ec8bbf99a95235573d67d87701ed
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033949"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="41ed8-103">commsNotifications 资源类型</span><span class="sxs-lookup"><span data-stu-id="41ed8-103">commsNotifications resource type</span></span>

<span data-ttu-id="41ed8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41ed8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41ed8-105">通信服务器用于在一个批处理中发送多个通知的通知列表。</span><span class="sxs-lookup"><span data-stu-id="41ed8-105">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="41ed8-106">属性</span><span class="sxs-lookup"><span data-stu-id="41ed8-106">Properties</span></span>

| <span data-ttu-id="41ed8-107">属性</span><span class="sxs-lookup"><span data-stu-id="41ed8-107">Property</span></span>       | <span data-ttu-id="41ed8-108">类型</span><span class="sxs-lookup"><span data-stu-id="41ed8-108">Type</span></span>                                                 | <span data-ttu-id="41ed8-109">说明</span><span class="sxs-lookup"><span data-stu-id="41ed8-109">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="41ed8-110">值</span><span class="sxs-lookup"><span data-stu-id="41ed8-110">value</span></span>          | <span data-ttu-id="41ed8-111">[commsNotification](commsnotification.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41ed8-111">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="41ed8-112">资源中的更改通知。</span><span class="sxs-lookup"><span data-stu-id="41ed8-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41ed8-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41ed8-113">JSON representation</span></span>

<span data-ttu-id="41ed8-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41ed8-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


