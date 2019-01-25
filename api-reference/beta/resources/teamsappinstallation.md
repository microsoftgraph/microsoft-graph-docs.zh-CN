---
title: teamsAppInstallation 资源类型
description: '团队中安装 teamsApp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512834"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="fca43-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fca43-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca43-104">安装在[工作组](team.md) [teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="fca43-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="fca43-105">应用程序一部分的任何 bot 将成为应用程序添加到任何工作组的一部分。</span><span class="sxs-lookup"><span data-stu-id="fca43-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="fca43-106">方法</span><span class="sxs-lookup"><span data-stu-id="fca43-106">Methods</span></span>

| <span data-ttu-id="fca43-107">方法</span><span class="sxs-lookup"><span data-stu-id="fca43-107">Method</span></span>       | <span data-ttu-id="fca43-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="fca43-108">Return Type</span></span>  |<span data-ttu-id="fca43-109">说明</span><span class="sxs-lookup"><span data-stu-id="fca43-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fca43-110">列表应用程序</span><span class="sxs-lookup"><span data-stu-id="fca43-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="fca43-111">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="fca43-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="fca43-112">列出了安装团队中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fca43-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="fca43-113">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="fca43-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="fca43-114">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="fca43-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="fca43-115">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="fca43-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="fca43-116">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="fca43-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="fca43-117">无</span><span class="sxs-lookup"><span data-stu-id="fca43-117">None</span></span> | <span data-ttu-id="fca43-118">删除 （卸载） 从团队应用程序。</span><span class="sxs-lookup"><span data-stu-id="fca43-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="fca43-119">升级的应用程序</span><span class="sxs-lookup"><span data-stu-id="fca43-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="fca43-120">无</span><span class="sxs-lookup"><span data-stu-id="fca43-120">None</span></span> | <span data-ttu-id="fca43-121">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fca43-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="fca43-122">属性</span><span class="sxs-lookup"><span data-stu-id="fca43-122">Properties</span></span>

| <span data-ttu-id="fca43-123">属性</span><span class="sxs-lookup"><span data-stu-id="fca43-123">Property</span></span>            | <span data-ttu-id="fca43-124">类型</span><span class="sxs-lookup"><span data-stu-id="fca43-124">Type</span></span>     | <span data-ttu-id="fca43-125">说明</span><span class="sxs-lookup"><span data-stu-id="fca43-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="fca43-126">id</span><span class="sxs-lookup"><span data-stu-id="fca43-126">id</span></span>                  | <span data-ttu-id="fca43-127">string</span><span class="sxs-lookup"><span data-stu-id="fca43-127">string</span></span>   | <span data-ttu-id="fca43-128">唯一的 id (不团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="fca43-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="fca43-129">关系</span><span class="sxs-lookup"><span data-stu-id="fca43-129">Relationships</span></span>

| <span data-ttu-id="fca43-130">关系</span><span class="sxs-lookup"><span data-stu-id="fca43-130">Relationship</span></span>   | <span data-ttu-id="fca43-131">类型</span><span class="sxs-lookup"><span data-stu-id="fca43-131">Type</span></span>    | <span data-ttu-id="fca43-132">说明</span><span class="sxs-lookup"><span data-stu-id="fca43-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fca43-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="fca43-133">teamsApp</span></span>|[<span data-ttu-id="fca43-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="fca43-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="fca43-135">安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="fca43-135">The app that is installed.</span></span> |
|<span data-ttu-id="fca43-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="fca43-136">teamsAppDefinition</span></span>|[<span data-ttu-id="fca43-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="fca43-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="fca43-138">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fca43-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fca43-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fca43-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="fca43-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fca43-140">See also</span></span>

- [<span data-ttu-id="fca43-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="fca43-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="fca43-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="fca43-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="fca43-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="fca43-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

