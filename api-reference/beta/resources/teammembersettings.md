---
title: teamMemberSettings 资源类型
description: 用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522642"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="7ce45-103">teamMemberSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ce45-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ce45-104">用于配置成员是否可以在团队中执行某些操作（例如，创建频道和添加机器人）的设置。</span><span class="sxs-lookup"><span data-stu-id="7ce45-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ce45-105">属性</span><span class="sxs-lookup"><span data-stu-id="7ce45-105">Properties</span></span>
| <span data-ttu-id="7ce45-106">属性</span><span class="sxs-lookup"><span data-stu-id="7ce45-106">Property</span></span>     | <span data-ttu-id="7ce45-107">类型</span><span class="sxs-lookup"><span data-stu-id="7ce45-107">Type</span></span>   |<span data-ttu-id="7ce45-108">说明</span><span class="sxs-lookup"><span data-stu-id="7ce45-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ce45-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="7ce45-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="7ce45-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce45-110">Boolean</span></span>|<span data-ttu-id="7ce45-111">如果设置为 true，则成员可以添加和更新通道。</span><span class="sxs-lookup"><span data-stu-id="7ce45-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="7ce45-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="7ce45-112">allowDeleteChannels</span></span>|<span data-ttu-id="7ce45-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce45-113">Boolean</span></span>|<span data-ttu-id="7ce45-114">如果设置为 true，则成员可以删除通道。</span><span class="sxs-lookup"><span data-stu-id="7ce45-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="7ce45-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="7ce45-115">allowAddRemoveApps</span></span>|<span data-ttu-id="7ce45-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce45-116">Boolean</span></span>|<span data-ttu-id="7ce45-117">如果设置为 true，则成员可以添加和删除应用程序。</span><span class="sxs-lookup"><span data-stu-id="7ce45-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="7ce45-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="7ce45-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="7ce45-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce45-119">Boolean</span></span>|<span data-ttu-id="7ce45-120">如果设置为 true，则成员可以添加、 更新和删除选项卡。</span><span class="sxs-lookup"><span data-stu-id="7ce45-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="7ce45-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="7ce45-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="7ce45-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce45-122">Boolean</span></span>|<span data-ttu-id="7ce45-123">如果设置为 true，则成员可以添加、 更新和删除连接器。</span><span class="sxs-lookup"><span data-stu-id="7ce45-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ce45-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ce45-124">JSON representation</span></span>

<span data-ttu-id="7ce45-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ce45-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teammembersettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
