---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dfa463ce47b9724d18f6f13b53ef46a1cb493f4a
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060456"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="5173c-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5173c-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="5173c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5173c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5173c-105">设置配置成员是否可以在团队中执行某些操作，例如，创建频道和添加[机器人](team.md)。</span><span class="sxs-lookup"><span data-stu-id="5173c-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5173c-106">属性</span><span class="sxs-lookup"><span data-stu-id="5173c-106">Properties</span></span>
| <span data-ttu-id="5173c-107">属性</span><span class="sxs-lookup"><span data-stu-id="5173c-107">Property</span></span>     | <span data-ttu-id="5173c-108">类型</span><span class="sxs-lookup"><span data-stu-id="5173c-108">Type</span></span>   |<span data-ttu-id="5173c-109">说明</span><span class="sxs-lookup"><span data-stu-id="5173c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5173c-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="5173c-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="5173c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-111">Boolean</span></span>|<span data-ttu-id="5173c-112">如果设置为 true，成员可以添加和更新任何频道。</span><span class="sxs-lookup"><span data-stu-id="5173c-112">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="5173c-113">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="5173c-113">allowCreatePrivateChannels</span></span>|<span data-ttu-id="5173c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-114">Boolean</span></span>|<span data-ttu-id="5173c-115">如果设置为 true，成员可以添加和更新私人频道。</span><span class="sxs-lookup"><span data-stu-id="5173c-115">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="5173c-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="5173c-116">allowDeleteChannels</span></span>|<span data-ttu-id="5173c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-117">Boolean</span></span>|<span data-ttu-id="5173c-118">如果设置为 true，成员可以删除频道。</span><span class="sxs-lookup"><span data-stu-id="5173c-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="5173c-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="5173c-119">allowAddRemoveApps</span></span>|<span data-ttu-id="5173c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-120">Boolean</span></span>|<span data-ttu-id="5173c-121">如果设置为 true，成员可以添加和删除应用。</span><span class="sxs-lookup"><span data-stu-id="5173c-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="5173c-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="5173c-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="5173c-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-123">Boolean</span></span>|<span data-ttu-id="5173c-124">如果设置为 true，成员可以添加、更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="5173c-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="5173c-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="5173c-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="5173c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="5173c-126">Boolean</span></span>|<span data-ttu-id="5173c-127">如果设置为 true，成员可以添加、更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="5173c-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5173c-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5173c-128">JSON representation</span></span>

<span data-ttu-id="5173c-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5173c-129">The following is a JSON representation of the resource.</span></span>

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


