---
title: teamMemberSettings 资源类型
description: 例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3854481e89f04fa727b77c6b4f8699c62a16d739
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978246"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="d68bd-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d68bd-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="d68bd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d68bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d68bd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d68bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d68bd-106">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加[团队](team.md)中。</span><span class="sxs-lookup"><span data-stu-id="d68bd-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d68bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="d68bd-107">Properties</span></span>
| <span data-ttu-id="d68bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="d68bd-108">Property</span></span>     | <span data-ttu-id="d68bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="d68bd-109">Type</span></span>   |<span data-ttu-id="d68bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="d68bd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d68bd-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="d68bd-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="d68bd-112">布尔</span><span class="sxs-lookup"><span data-stu-id="d68bd-112">Boolean</span></span>|<span data-ttu-id="d68bd-113">如果设置为 true，则成员可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="d68bd-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="d68bd-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="d68bd-114">allowDeleteChannels</span></span>|<span data-ttu-id="d68bd-115">布尔</span><span class="sxs-lookup"><span data-stu-id="d68bd-115">Boolean</span></span>|<span data-ttu-id="d68bd-116">如果设置为 true，则成员可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="d68bd-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="d68bd-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="d68bd-117">allowAddRemoveApps</span></span>|<span data-ttu-id="d68bd-118">布尔</span><span class="sxs-lookup"><span data-stu-id="d68bd-118">Boolean</span></span>|<span data-ttu-id="d68bd-119">如果设置为 true，则成员可以添加和删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="d68bd-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="d68bd-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="d68bd-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="d68bd-121">布尔</span><span class="sxs-lookup"><span data-stu-id="d68bd-121">Boolean</span></span>|<span data-ttu-id="d68bd-122">如果设置为 true，则成员可以添加、 更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="d68bd-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="d68bd-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="d68bd-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="d68bd-124">布尔</span><span class="sxs-lookup"><span data-stu-id="d68bd-124">Boolean</span></span>|<span data-ttu-id="d68bd-125">如果设置为 true，则成员可以添加、 更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="d68bd-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d68bd-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d68bd-126">JSON representation</span></span>

<span data-ttu-id="d68bd-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d68bd-127">The following is a JSON representation of the resource.</span></span>

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
