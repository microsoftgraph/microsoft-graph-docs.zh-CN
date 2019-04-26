---
title: teamsAppInstallation 资源类型
description: '在团队中安装的 teamsApp。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d8770a21b11c9ba1042c9a0f59d9405dce96f9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345800"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="b1255-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1255-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1255-104">在[团队](team.md)中安装的[teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="b1255-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="b1255-105">作为应用程序的一部分的任何 bot 都将成为向其添加应用程序的任何团队的一部分。</span><span class="sxs-lookup"><span data-stu-id="b1255-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="b1255-106">方法</span><span class="sxs-lookup"><span data-stu-id="b1255-106">Methods</span></span>

| <span data-ttu-id="b1255-107">方法</span><span class="sxs-lookup"><span data-stu-id="b1255-107">Method</span></span>       | <span data-ttu-id="b1255-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1255-108">Return Type</span></span>  |<span data-ttu-id="b1255-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1255-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1255-110">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="b1255-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="b1255-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1255-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="b1255-112">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b1255-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="b1255-113">添加应用程序</span><span class="sxs-lookup"><span data-stu-id="b1255-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="b1255-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1255-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="b1255-115">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="b1255-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="b1255-116">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="b1255-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="b1255-117">无</span><span class="sxs-lookup"><span data-stu-id="b1255-117">None</span></span> | <span data-ttu-id="b1255-118">从团队中删除 (卸载) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="b1255-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="b1255-119">升级应用程序</span><span class="sxs-lookup"><span data-stu-id="b1255-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="b1255-120">无</span><span class="sxs-lookup"><span data-stu-id="b1255-120">None</span></span> | <span data-ttu-id="b1255-121">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b1255-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1255-122">属性</span><span class="sxs-lookup"><span data-stu-id="b1255-122">Properties</span></span>

| <span data-ttu-id="b1255-123">属性</span><span class="sxs-lookup"><span data-stu-id="b1255-123">Property</span></span>            | <span data-ttu-id="b1255-124">类型</span><span class="sxs-lookup"><span data-stu-id="b1255-124">Type</span></span>     | <span data-ttu-id="b1255-125">说明</span><span class="sxs-lookup"><span data-stu-id="b1255-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b1255-126">id</span><span class="sxs-lookup"><span data-stu-id="b1255-126">id</span></span>                  | <span data-ttu-id="b1255-127">string</span><span class="sxs-lookup"><span data-stu-id="b1255-127">string</span></span>   | <span data-ttu-id="b1255-128">唯一 id (而不是团队 appid)。</span><span class="sxs-lookup"><span data-stu-id="b1255-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="b1255-129">关系</span><span class="sxs-lookup"><span data-stu-id="b1255-129">Relationships</span></span>

| <span data-ttu-id="b1255-130">关系</span><span class="sxs-lookup"><span data-stu-id="b1255-130">Relationship</span></span>   | <span data-ttu-id="b1255-131">类型</span><span class="sxs-lookup"><span data-stu-id="b1255-131">Type</span></span>    | <span data-ttu-id="b1255-132">说明</span><span class="sxs-lookup"><span data-stu-id="b1255-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b1255-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1255-133">teamsApp</span></span>|[<span data-ttu-id="b1255-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1255-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="b1255-135">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b1255-135">The app that is installed.</span></span> |
|<span data-ttu-id="b1255-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1255-136">teamsAppDefinition</span></span>|[<span data-ttu-id="b1255-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1255-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="b1255-138">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1255-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1255-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1255-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="b1255-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b1255-140">See also</span></span>

- [<span data-ttu-id="b1255-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1255-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="b1255-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1255-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="b1255-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b1255-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

