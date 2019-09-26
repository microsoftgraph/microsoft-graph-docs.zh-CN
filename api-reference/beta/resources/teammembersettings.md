---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8967eb083ad2bd413277c42b688c2d0c48d8244b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196257"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="863e6-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="863e6-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863e6-104">用于配置成员是否可以在[团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。</span><span class="sxs-lookup"><span data-stu-id="863e6-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="863e6-105">属性</span><span class="sxs-lookup"><span data-stu-id="863e6-105">Properties</span></span>
| <span data-ttu-id="863e6-106">属性</span><span class="sxs-lookup"><span data-stu-id="863e6-106">Property</span></span>     | <span data-ttu-id="863e6-107">类型</span><span class="sxs-lookup"><span data-stu-id="863e6-107">Type</span></span>   |<span data-ttu-id="863e6-108">说明</span><span class="sxs-lookup"><span data-stu-id="863e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="863e6-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="863e6-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="863e6-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-110">Boolean</span></span>|<span data-ttu-id="863e6-111">如果设置为 true，则成员可以添加和更新任何频道。</span><span class="sxs-lookup"><span data-stu-id="863e6-111">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="863e6-112">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="863e6-112">allowCreatePrivateChannels</span></span>|<span data-ttu-id="863e6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-113">Boolean</span></span>|<span data-ttu-id="863e6-114">如果设置为 true，则成员可以添加和更新专用通道。</span><span class="sxs-lookup"><span data-stu-id="863e6-114">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="863e6-115">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="863e6-115">allowDeleteChannels</span></span>|<span data-ttu-id="863e6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-116">Boolean</span></span>|<span data-ttu-id="863e6-117">如果设置为 true，则成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="863e6-117">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="863e6-118">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="863e6-118">allowAddRemoveApps</span></span>|<span data-ttu-id="863e6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-119">Boolean</span></span>|<span data-ttu-id="863e6-120">如果设置为 true，则成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="863e6-120">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="863e6-121">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="863e6-121">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="863e6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-122">Boolean</span></span>|<span data-ttu-id="863e6-123">如果设置为 true，则成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="863e6-123">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="863e6-124">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="863e6-124">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="863e6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="863e6-125">Boolean</span></span>|<span data-ttu-id="863e6-126">如果设置为 true，则成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="863e6-126">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="863e6-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="863e6-127">JSON representation</span></span>

<span data-ttu-id="863e6-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="863e6-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
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
