---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7c5cc116567b0ee2db1b2dd5e28c4749d7c6772c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033864"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="ee0d7-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee0d7-103">teamGuestSettings resource type</span></span>



<span data-ttu-id="ee0d7-104">用于配置来宾是否可以在[团队](team.md)中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="ee0d7-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee0d7-105">属性</span><span class="sxs-lookup"><span data-stu-id="ee0d7-105">Properties</span></span>
| <span data-ttu-id="ee0d7-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee0d7-106">Property</span></span>     | <span data-ttu-id="ee0d7-107">类型</span><span class="sxs-lookup"><span data-stu-id="ee0d7-107">Type</span></span>   |<span data-ttu-id="ee0d7-108">说明</span><span class="sxs-lookup"><span data-stu-id="ee0d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee0d7-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ee0d7-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ee0d7-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee0d7-110">Boolean</span></span>|<span data-ttu-id="ee0d7-111">如果设置为 true, 则来宾可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="ee0d7-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="ee0d7-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ee0d7-112">allowDeleteChannels</span></span>|<span data-ttu-id="ee0d7-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee0d7-113">Boolean</span></span>|<span data-ttu-id="ee0d7-114">如果设置为 true, 则来宾可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="ee0d7-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee0d7-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee0d7-115">JSON representation</span></span>

<span data-ttu-id="ee0d7-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee0d7-116">The following is a JSON representation of the resource.</span></span>

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
