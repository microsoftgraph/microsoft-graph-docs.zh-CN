---
title: commsNotifications 资源类型
description: 通信服务器用于在一个批处理中发送多个通知的通知列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8a6be0d41a95f75130796e1073750c3e90d65a9a
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006710"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="84a3f-103">commsNotifications 资源类型</span><span class="sxs-lookup"><span data-stu-id="84a3f-103">commsNotifications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84a3f-104">通信服务器用于在一个批处理中发送多个通知的通知列表。</span><span class="sxs-lookup"><span data-stu-id="84a3f-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="84a3f-105">属性</span><span class="sxs-lookup"><span data-stu-id="84a3f-105">Properties</span></span>

| <span data-ttu-id="84a3f-106">属性</span><span class="sxs-lookup"><span data-stu-id="84a3f-106">Property</span></span>       | <span data-ttu-id="84a3f-107">类型</span><span class="sxs-lookup"><span data-stu-id="84a3f-107">Type</span></span>                                                 | <span data-ttu-id="84a3f-108">说明</span><span class="sxs-lookup"><span data-stu-id="84a3f-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="84a3f-109">值</span><span class="sxs-lookup"><span data-stu-id="84a3f-109">value</span></span>          | <span data-ttu-id="84a3f-110">[commsNotification](commsnotification.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a3f-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="84a3f-111">资源中的更改通知。</span><span class="sxs-lookup"><span data-stu-id="84a3f-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84a3f-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84a3f-112">JSON representation</span></span>

<span data-ttu-id="84a3f-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84a3f-113">The following is a JSON representation of the resource.</span></span>

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
