---
title: teamMemberSettings 资源类型
description: 例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加团队中。
localization_priority: Normal
ms.openlocfilehash: 7b63bce5bc298f7d9599d8c6146d7962d319c79f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826066"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="5e636-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e636-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="5e636-104">例如，要配置的成员可以执行某些操作时，是否设置创建通道，并将自动程序，添加[团队](team.md)中。</span><span class="sxs-lookup"><span data-stu-id="5e636-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e636-105">属性</span><span class="sxs-lookup"><span data-stu-id="5e636-105">Properties</span></span>
| <span data-ttu-id="5e636-106">属性</span><span class="sxs-lookup"><span data-stu-id="5e636-106">Property</span></span>     | <span data-ttu-id="5e636-107">类型</span><span class="sxs-lookup"><span data-stu-id="5e636-107">Type</span></span>   |<span data-ttu-id="5e636-108">Description</span><span class="sxs-lookup"><span data-stu-id="5e636-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e636-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="5e636-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="5e636-110">布尔</span><span class="sxs-lookup"><span data-stu-id="5e636-110">Boolean</span></span>|<span data-ttu-id="5e636-111">如果设置为 true，则成员可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="5e636-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="5e636-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="5e636-112">allowDeleteChannels</span></span>|<span data-ttu-id="5e636-113">布尔</span><span class="sxs-lookup"><span data-stu-id="5e636-113">Boolean</span></span>|<span data-ttu-id="5e636-114">如果设置为 true，则成员可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="5e636-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="5e636-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="5e636-115">allowAddRemoveApps</span></span>|<span data-ttu-id="5e636-116">布尔</span><span class="sxs-lookup"><span data-stu-id="5e636-116">Boolean</span></span>|<span data-ttu-id="5e636-117">如果设置为 true，则成员可以添加和删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="5e636-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="5e636-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="5e636-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="5e636-119">布尔</span><span class="sxs-lookup"><span data-stu-id="5e636-119">Boolean</span></span>|<span data-ttu-id="5e636-120">如果设置为 true，则成员可以添加、 更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="5e636-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="5e636-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="5e636-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="5e636-122">布尔</span><span class="sxs-lookup"><span data-stu-id="5e636-122">Boolean</span></span>|<span data-ttu-id="5e636-123">如果设置为 true，则成员可以添加、 更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="5e636-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e636-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e636-124">JSON representation</span></span>

<span data-ttu-id="5e636-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e636-125">The following is a JSON representation of the resource.</span></span>

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
