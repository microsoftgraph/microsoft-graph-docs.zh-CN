---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4df97a37cf1f2dc086af8905f6ec168a7ac458b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533542"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="390f9-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="390f9-103">teamGuestSettings resource type</span></span>

<span data-ttu-id="390f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="390f9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="390f9-105">用于配置来宾是否可以在[团队](team.md)中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="390f9-105">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="390f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="390f9-106">Properties</span></span>
| <span data-ttu-id="390f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="390f9-107">Property</span></span>     | <span data-ttu-id="390f9-108">类型</span><span class="sxs-lookup"><span data-stu-id="390f9-108">Type</span></span>   |<span data-ttu-id="390f9-109">说明</span><span class="sxs-lookup"><span data-stu-id="390f9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="390f9-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="390f9-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="390f9-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="390f9-111">Boolean</span></span>|<span data-ttu-id="390f9-112">如果设置为 true，则来宾可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="390f9-112">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="390f9-113">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="390f9-113">allowDeleteChannels</span></span>|<span data-ttu-id="390f9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="390f9-114">Boolean</span></span>|<span data-ttu-id="390f9-115">如果设置为 true，则来宾可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="390f9-115">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="390f9-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="390f9-116">JSON representation</span></span>

<span data-ttu-id="390f9-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="390f9-117">The following is a JSON representation of the resource.</span></span>

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
