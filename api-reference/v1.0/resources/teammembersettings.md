---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d75ae8d97d3d2c95cc1779e38346efeea3026f23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533533"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="91ef0-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="91ef0-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="91ef0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ef0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="91ef0-105">用于配置成员是否可以在[团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。</span><span class="sxs-lookup"><span data-stu-id="91ef0-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="91ef0-106">属性</span><span class="sxs-lookup"><span data-stu-id="91ef0-106">Properties</span></span>
| <span data-ttu-id="91ef0-107">属性</span><span class="sxs-lookup"><span data-stu-id="91ef0-107">Property</span></span>     | <span data-ttu-id="91ef0-108">类型</span><span class="sxs-lookup"><span data-stu-id="91ef0-108">Type</span></span>   |<span data-ttu-id="91ef0-109">说明</span><span class="sxs-lookup"><span data-stu-id="91ef0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91ef0-110">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="91ef0-110">allowCreatePrivateChannels</span></span>|<span data-ttu-id="91ef0-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-111">Boolean</span></span>|<span data-ttu-id="91ef0-112">如果设置为 true，则成员可以添加和更新专用通道。</span><span class="sxs-lookup"><span data-stu-id="91ef0-112">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="91ef0-113">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="91ef0-113">allowCreateUpdateChannels</span></span>|<span data-ttu-id="91ef0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-114">Boolean</span></span>|<span data-ttu-id="91ef0-115">如果设置为 true，则成员可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="91ef0-115">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="91ef0-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="91ef0-116">allowDeleteChannels</span></span>|<span data-ttu-id="91ef0-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-117">Boolean</span></span>|<span data-ttu-id="91ef0-118">如果设置为 true，则成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="91ef0-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="91ef0-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="91ef0-119">allowAddRemoveApps</span></span>|<span data-ttu-id="91ef0-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-120">Boolean</span></span>|<span data-ttu-id="91ef0-121">如果设置为 true，则成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="91ef0-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="91ef0-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="91ef0-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="91ef0-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-123">Boolean</span></span>|<span data-ttu-id="91ef0-124">如果设置为 true，则成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="91ef0-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="91ef0-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="91ef0-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="91ef0-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ef0-126">Boolean</span></span>|<span data-ttu-id="91ef0-127">如果设置为 true，则成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="91ef0-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91ef0-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91ef0-128">JSON representation</span></span>

<span data-ttu-id="91ef0-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91ef0-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreatePrivateChannels": true,
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
