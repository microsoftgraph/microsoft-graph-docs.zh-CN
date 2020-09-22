---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d3c716937c7a10091a663ea614d3a63c91ab4b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046634"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="b741b-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b741b-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="b741b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b741b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b741b-105">用于配置成员是否可以在 [团队](team.md)中执行某些操作（例如，创建频道和添加 bot）的设置。</span><span class="sxs-lookup"><span data-stu-id="b741b-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b741b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b741b-106">Properties</span></span>
| <span data-ttu-id="b741b-107">属性</span><span class="sxs-lookup"><span data-stu-id="b741b-107">Property</span></span>     | <span data-ttu-id="b741b-108">类型</span><span class="sxs-lookup"><span data-stu-id="b741b-108">Type</span></span>   |<span data-ttu-id="b741b-109">说明</span><span class="sxs-lookup"><span data-stu-id="b741b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b741b-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="b741b-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="b741b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-111">Boolean</span></span>|<span data-ttu-id="b741b-112">如果设置为 true，则成员可以添加和更新任何频道。</span><span class="sxs-lookup"><span data-stu-id="b741b-112">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="b741b-113">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="b741b-113">allowCreatePrivateChannels</span></span>|<span data-ttu-id="b741b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-114">Boolean</span></span>|<span data-ttu-id="b741b-115">如果设置为 true，则成员可以添加和更新专用通道。</span><span class="sxs-lookup"><span data-stu-id="b741b-115">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="b741b-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="b741b-116">allowDeleteChannels</span></span>|<span data-ttu-id="b741b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-117">Boolean</span></span>|<span data-ttu-id="b741b-118">如果设置为 true，则成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="b741b-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="b741b-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="b741b-119">allowAddRemoveApps</span></span>|<span data-ttu-id="b741b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-120">Boolean</span></span>|<span data-ttu-id="b741b-121">如果设置为 true，则成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="b741b-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="b741b-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="b741b-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="b741b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-123">Boolean</span></span>|<span data-ttu-id="b741b-124">如果设置为 true，则成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="b741b-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="b741b-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="b741b-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="b741b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b741b-126">Boolean</span></span>|<span data-ttu-id="b741b-127">如果设置为 true，则成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="b741b-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b741b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b741b-128">JSON representation</span></span>

<span data-ttu-id="b741b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b741b-129">The following is a JSON representation of the resource.</span></span>

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


