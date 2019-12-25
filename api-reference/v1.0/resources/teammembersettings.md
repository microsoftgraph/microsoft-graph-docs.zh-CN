---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c1485bbc43588b8144cbe1cc7cb189f9b8c9fdc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863776"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="e5892-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5892-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="e5892-104">用于配置成员是否可以在[团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。</span><span class="sxs-lookup"><span data-stu-id="e5892-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e5892-105">属性</span><span class="sxs-lookup"><span data-stu-id="e5892-105">Properties</span></span>
| <span data-ttu-id="e5892-106">属性</span><span class="sxs-lookup"><span data-stu-id="e5892-106">Property</span></span>     | <span data-ttu-id="e5892-107">类型</span><span class="sxs-lookup"><span data-stu-id="e5892-107">Type</span></span>   |<span data-ttu-id="e5892-108">说明</span><span class="sxs-lookup"><span data-stu-id="e5892-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5892-109">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="e5892-109">allowCreatePrivateChannels</span></span>|<span data-ttu-id="e5892-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-110">Boolean</span></span>|<span data-ttu-id="e5892-111">如果设置为 true，则成员可以添加和更新专用通道。</span><span class="sxs-lookup"><span data-stu-id="e5892-111">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="e5892-112">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="e5892-112">allowCreateUpdateChannels</span></span>|<span data-ttu-id="e5892-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-113">Boolean</span></span>|<span data-ttu-id="e5892-114">如果设置为 true，则成员可以添加和更新频道。</span><span class="sxs-lookup"><span data-stu-id="e5892-114">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="e5892-115">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="e5892-115">allowDeleteChannels</span></span>|<span data-ttu-id="e5892-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-116">Boolean</span></span>|<span data-ttu-id="e5892-117">如果设置为 true，则成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="e5892-117">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="e5892-118">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="e5892-118">allowAddRemoveApps</span></span>|<span data-ttu-id="e5892-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-119">Boolean</span></span>|<span data-ttu-id="e5892-120">如果设置为 true，则成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="e5892-120">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="e5892-121">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="e5892-121">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="e5892-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-122">Boolean</span></span>|<span data-ttu-id="e5892-123">如果设置为 true，则成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="e5892-123">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="e5892-124">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="e5892-124">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="e5892-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5892-125">Boolean</span></span>|<span data-ttu-id="e5892-126">如果设置为 true，则成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="e5892-126">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5892-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5892-127">JSON representation</span></span>

<span data-ttu-id="e5892-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5892-128">The following is a JSON representation of the resource.</span></span>

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
