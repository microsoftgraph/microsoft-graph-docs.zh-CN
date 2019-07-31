---
title: teamGuestSettings 资源类型
description: 用于配置来宾是否可以在团队中创建、更新或删除频道的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d6e10ccde127e2318ad9c2f3015f5d911574513
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964555"
---
# <a name="teamguestsettings-resource-type"></a><span data-ttu-id="44c7c-103">teamGuestSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="44c7c-103">teamGuestSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44c7c-104">用于配置来宾是否可以在[团队](team.md)中创建、更新或删除频道的设置。</span><span class="sxs-lookup"><span data-stu-id="44c7c-104">Settings to configure whether guests can create, update, or delete channels in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="44c7c-105">属性</span><span class="sxs-lookup"><span data-stu-id="44c7c-105">Properties</span></span>
| <span data-ttu-id="44c7c-106">属性</span><span class="sxs-lookup"><span data-stu-id="44c7c-106">Property</span></span>     | <span data-ttu-id="44c7c-107">类型</span><span class="sxs-lookup"><span data-stu-id="44c7c-107">Type</span></span>   |<span data-ttu-id="44c7c-108">说明</span><span class="sxs-lookup"><span data-stu-id="44c7c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44c7c-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="44c7c-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="44c7c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="44c7c-110">Boolean</span></span>|<span data-ttu-id="44c7c-111">如果设置为 true, 则来宾可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="44c7c-111">If set to true, guests can add and update channels.</span></span>|
|<span data-ttu-id="44c7c-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="44c7c-112">allowDeleteChannels</span></span>|<span data-ttu-id="44c7c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="44c7c-113">Boolean</span></span>|<span data-ttu-id="44c7c-114">如果设置为 true, 则来宾可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="44c7c-114">If set to true, guests can delete channels.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44c7c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44c7c-115">JSON representation</span></span>

<span data-ttu-id="44c7c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44c7c-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
