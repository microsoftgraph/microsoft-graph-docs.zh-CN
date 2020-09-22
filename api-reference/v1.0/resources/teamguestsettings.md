---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1d56c6a09c866a8d023466b57be1468d8f771269
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093999"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="68c7a-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="68c7a-103">teamGuestSettings resource type</span></span>

<span data-ttu-id="68c7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68c7a-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="68c7a-105">用于配置来宾是否可以在 [团队](team.md)中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="68c7a-105">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="68c7a-106">属性</span><span class="sxs-lookup"><span data-stu-id="68c7a-106">Properties</span></span>
| <span data-ttu-id="68c7a-107">属性</span><span class="sxs-lookup"><span data-stu-id="68c7a-107">Property</span></span>     | <span data-ttu-id="68c7a-108">类型</span><span class="sxs-lookup"><span data-stu-id="68c7a-108">Type</span></span>   |<span data-ttu-id="68c7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="68c7a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68c7a-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="68c7a-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="68c7a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="68c7a-111">Boolean</span></span>|<span data-ttu-id="68c7a-112">如果设置为 true，则来宾可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="68c7a-112">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="68c7a-113">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="68c7a-113">allowDeleteChannels</span></span>|<span data-ttu-id="68c7a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="68c7a-114">Boolean</span></span>|<span data-ttu-id="68c7a-115">如果设置为 true，则来宾可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="68c7a-115">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68c7a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68c7a-116">JSON representation</span></span>

<span data-ttu-id="68c7a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68c7a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

