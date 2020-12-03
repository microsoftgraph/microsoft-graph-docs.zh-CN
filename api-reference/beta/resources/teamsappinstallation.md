---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f5775514eb242f540bc6740d8e21620448f2d280
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563637"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="d46d1-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d46d1-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="d46d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d46d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d46d1-105">安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="d46d1-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="d46d1-106">作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="d46d1-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="d46d1-107">方法</span><span class="sxs-lookup"><span data-stu-id="d46d1-107">Methods</span></span>

| <span data-ttu-id="d46d1-108">方法</span><span class="sxs-lookup"><span data-stu-id="d46d1-108">Method</span></span>       | <span data-ttu-id="d46d1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d46d1-109">Return Type</span></span>  |<span data-ttu-id="d46d1-110">说明</span><span class="sxs-lookup"><span data-stu-id="d46d1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d46d1-111">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="d46d1-112">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d46d1-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="d46d1-113">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d46d1-114">获取团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="d46d1-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d46d1-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="d46d1-116">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="d46d1-117">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="d46d1-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="d46d1-118">无</span><span class="sxs-lookup"><span data-stu-id="d46d1-118">None</span></span> | <span data-ttu-id="d46d1-119">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="d46d1-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d46d1-120">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="d46d1-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="d46d1-121">无</span><span class="sxs-lookup"><span data-stu-id="d46d1-121">None</span></span> | <span data-ttu-id="d46d1-122">从团队中删除应用) 的 (卸载。</span><span class="sxs-lookup"><span data-stu-id="d46d1-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="d46d1-123">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="d46d1-124">无</span><span class="sxs-lookup"><span data-stu-id="d46d1-124">None</span></span> | <span data-ttu-id="d46d1-125">升级到团队中安装的应用程序的最新版本。</span><span class="sxs-lookup"><span data-stu-id="d46d1-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="d46d1-126">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="d46d1-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="d46d1-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d46d1-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="d46d1-128">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-128">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d46d1-129">为用户获取已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="d46d1-130">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d46d1-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="d46d1-131">列出在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="d46d1-132">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | | <span data-ttu-id="d46d1-133">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-133">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d46d1-134">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="d46d1-134">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="d46d1-135">无</span><span class="sxs-lookup"><span data-stu-id="d46d1-135">None</span></span> | <span data-ttu-id="d46d1-136">删除) 用户的个人作用域中的应用程序 (卸载。</span><span class="sxs-lookup"><span data-stu-id="d46d1-136">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="d46d1-137">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="d46d1-137">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="d46d1-138">无</span><span class="sxs-lookup"><span data-stu-id="d46d1-138">None</span></span> | <span data-ttu-id="d46d1-139">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-139">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="d46d1-140">属性</span><span class="sxs-lookup"><span data-stu-id="d46d1-140">Properties</span></span>

| <span data-ttu-id="d46d1-141">属性</span><span class="sxs-lookup"><span data-stu-id="d46d1-141">Property</span></span>            | <span data-ttu-id="d46d1-142">类型</span><span class="sxs-lookup"><span data-stu-id="d46d1-142">Type</span></span>     | <span data-ttu-id="d46d1-143">说明</span><span class="sxs-lookup"><span data-stu-id="d46d1-143">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d46d1-144">id</span><span class="sxs-lookup"><span data-stu-id="d46d1-144">id</span></span>                  | <span data-ttu-id="d46d1-145">string</span><span class="sxs-lookup"><span data-stu-id="d46d1-145">string</span></span>   | <span data-ttu-id="d46d1-146">唯一 ID (团队的 ap ID) 。</span><span class="sxs-lookup"><span data-stu-id="d46d1-146">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d46d1-147">关系</span><span class="sxs-lookup"><span data-stu-id="d46d1-147">Relationships</span></span>

| <span data-ttu-id="d46d1-148">关系</span><span class="sxs-lookup"><span data-stu-id="d46d1-148">Relationship</span></span>   | <span data-ttu-id="d46d1-149">类型</span><span class="sxs-lookup"><span data-stu-id="d46d1-149">Type</span></span>    | <span data-ttu-id="d46d1-150">说明</span><span class="sxs-lookup"><span data-stu-id="d46d1-150">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d46d1-151">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d46d1-151">teamsApp</span></span>|[<span data-ttu-id="d46d1-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d46d1-152">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="d46d1-153">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d46d1-153">The app that is installed.</span></span> |
|<span data-ttu-id="d46d1-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d46d1-154">teamsAppDefinition</span></span>|[<span data-ttu-id="d46d1-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d46d1-155">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="d46d1-156">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d46d1-156">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d46d1-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d46d1-157">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="d46d1-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d46d1-158">See also</span></span>

- [<span data-ttu-id="d46d1-159">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d46d1-159">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="d46d1-160">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d46d1-160">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d46d1-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d46d1-161">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="d46d1-162">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d46d1-162">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


