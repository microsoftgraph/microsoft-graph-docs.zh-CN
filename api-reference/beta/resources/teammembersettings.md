---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 33f1930096ff63968db39e06ddec26c53ae8bcc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341720"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="5bd86-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bd86-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd86-104">用于配置成员是否可以在[团队](team.md)中执行某些操作 (例如, 创建频道和添加 bot) 的设置。</span><span class="sxs-lookup"><span data-stu-id="5bd86-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5bd86-105">属性</span><span class="sxs-lookup"><span data-stu-id="5bd86-105">Properties</span></span>
| <span data-ttu-id="5bd86-106">属性</span><span class="sxs-lookup"><span data-stu-id="5bd86-106">Property</span></span>     | <span data-ttu-id="5bd86-107">类型</span><span class="sxs-lookup"><span data-stu-id="5bd86-107">Type</span></span>   |<span data-ttu-id="5bd86-108">说明</span><span class="sxs-lookup"><span data-stu-id="5bd86-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd86-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="5bd86-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="5bd86-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd86-110">Boolean</span></span>|<span data-ttu-id="5bd86-111">如果设置为 true, 则成员可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="5bd86-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="5bd86-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="5bd86-112">allowDeleteChannels</span></span>|<span data-ttu-id="5bd86-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd86-113">Boolean</span></span>|<span data-ttu-id="5bd86-114">如果设置为 true, 则成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="5bd86-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="5bd86-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="5bd86-115">allowAddRemoveApps</span></span>|<span data-ttu-id="5bd86-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd86-116">Boolean</span></span>|<span data-ttu-id="5bd86-117">如果设置为 true, 则成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="5bd86-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="5bd86-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="5bd86-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="5bd86-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd86-119">Boolean</span></span>|<span data-ttu-id="5bd86-120">如果设置为 true, 则成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="5bd86-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="5bd86-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="5bd86-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="5bd86-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd86-122">Boolean</span></span>|<span data-ttu-id="5bd86-123">如果设置为 true, 则成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="5bd86-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bd86-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bd86-124">JSON representation</span></span>

<span data-ttu-id="5bd86-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bd86-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
