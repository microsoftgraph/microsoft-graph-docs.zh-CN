---
title: teamMemberSettings 资源类型
description: 例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6ffd1dba4a0aafb1364a6d3f1ee673e2381c7178
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954251"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="deed1-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="deed1-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="deed1-104">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加[团队](team.md)中。</span><span class="sxs-lookup"><span data-stu-id="deed1-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="deed1-105">属性</span><span class="sxs-lookup"><span data-stu-id="deed1-105">Properties</span></span>
| <span data-ttu-id="deed1-106">属性</span><span class="sxs-lookup"><span data-stu-id="deed1-106">Property</span></span>     | <span data-ttu-id="deed1-107">类型</span><span class="sxs-lookup"><span data-stu-id="deed1-107">Type</span></span>   |<span data-ttu-id="deed1-108">说明</span><span class="sxs-lookup"><span data-stu-id="deed1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deed1-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="deed1-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="deed1-110">布尔</span><span class="sxs-lookup"><span data-stu-id="deed1-110">Boolean</span></span>|<span data-ttu-id="deed1-111">如果设置为 true，则成员可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="deed1-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="deed1-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="deed1-112">allowDeleteChannels</span></span>|<span data-ttu-id="deed1-113">布尔</span><span class="sxs-lookup"><span data-stu-id="deed1-113">Boolean</span></span>|<span data-ttu-id="deed1-114">如果设置为 true，则成员可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="deed1-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="deed1-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="deed1-115">allowAddRemoveApps</span></span>|<span data-ttu-id="deed1-116">布尔</span><span class="sxs-lookup"><span data-stu-id="deed1-116">Boolean</span></span>|<span data-ttu-id="deed1-117">如果设置为 true，则成员可以添加和删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="deed1-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="deed1-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="deed1-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="deed1-119">布尔</span><span class="sxs-lookup"><span data-stu-id="deed1-119">Boolean</span></span>|<span data-ttu-id="deed1-120">如果设置为 true，则成员可以添加、 更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="deed1-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="deed1-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="deed1-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="deed1-122">布尔</span><span class="sxs-lookup"><span data-stu-id="deed1-122">Boolean</span></span>|<span data-ttu-id="deed1-123">如果设置为 true，则成员可以添加、 更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="deed1-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="deed1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deed1-124">JSON representation</span></span>

<span data-ttu-id="deed1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deed1-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
