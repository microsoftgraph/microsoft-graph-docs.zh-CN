---
title: teamsAppInstallation 资源类型
description: 代表在团队中安装的 teamsApp 或用户的个人作用域。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0d15f65273504b3b7577c875fec69c5a212a8c76
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563749"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="a8b3e-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8b3e-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="a8b3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8b3e-105">代表在[团队](team.md)中安装的[teamsApp](teamsapp.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="a8b3e-106">作为应用程序一部分的任何 bot 都将成为应用程序添加到的任何团队或用户的个人作用域的一部分。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="a8b3e-107">方法</span><span class="sxs-lookup"><span data-stu-id="a8b3e-107">Methods</span></span>

| <span data-ttu-id="a8b3e-108">方法</span><span class="sxs-lookup"><span data-stu-id="a8b3e-108">Method</span></span>       | <span data-ttu-id="a8b3e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8b3e-109">Return Type</span></span>  |<span data-ttu-id="a8b3e-110">说明</span><span class="sxs-lookup"><span data-stu-id="a8b3e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8b3e-111">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="a8b3e-112">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8b3e-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="a8b3e-113">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="a8b3e-114">获取团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="a8b3e-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8b3e-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="a8b3e-116">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="a8b3e-117">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="a8b3e-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) | <span data-ttu-id="a8b3e-118">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-118">None</span></span> | <span data-ttu-id="a8b3e-119">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="a8b3e-120">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="a8b3e-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="a8b3e-121">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-121">None</span></span> | <span data-ttu-id="a8b3e-122">从团队中删除应用) 的 (卸载。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="a8b3e-123">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="a8b3e-124">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-124">None</span></span> | <span data-ttu-id="a8b3e-125">升级到团队中安装的应用程序的最新版本。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="a8b3e-126">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="a8b3e-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="a8b3e-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8b3e-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="a8b3e-128">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-128">Lists apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="a8b3e-129">为用户获取已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="a8b3e-130">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8b3e-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="a8b3e-131">列出在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="a8b3e-132">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | <span data-ttu-id="a8b3e-133">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-133">None</span></span> | <span data-ttu-id="a8b3e-134">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-134">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="a8b3e-135">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8b3e-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="a8b3e-136">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-136">None</span></span> | <span data-ttu-id="a8b3e-137">从用户的个人作用域) 应用中删除 (卸载。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-137">Removes (uninstalls) an app from the personal scope of a user.</span></span> |
|[<span data-ttu-id="a8b3e-138">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="a8b3e-138">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="a8b3e-139">无</span><span class="sxs-lookup"><span data-stu-id="a8b3e-139">None</span></span> | <span data-ttu-id="a8b3e-140">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-140">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8b3e-141">属性</span><span class="sxs-lookup"><span data-stu-id="a8b3e-141">Properties</span></span>

| <span data-ttu-id="a8b3e-142">属性</span><span class="sxs-lookup"><span data-stu-id="a8b3e-142">Property</span></span>            | <span data-ttu-id="a8b3e-143">类型</span><span class="sxs-lookup"><span data-stu-id="a8b3e-143">Type</span></span>     | <span data-ttu-id="a8b3e-144">说明</span><span class="sxs-lookup"><span data-stu-id="a8b3e-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a8b3e-145">id</span><span class="sxs-lookup"><span data-stu-id="a8b3e-145">id</span></span>                  | <span data-ttu-id="a8b3e-146">string</span><span class="sxs-lookup"><span data-stu-id="a8b3e-146">string</span></span>   | <span data-ttu-id="a8b3e-147">唯一 ID (不是团队的 appID) 。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-147">A unique ID (not the Teams appID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a8b3e-148">关系</span><span class="sxs-lookup"><span data-stu-id="a8b3e-148">Relationships</span></span>

| <span data-ttu-id="a8b3e-149">关系</span><span class="sxs-lookup"><span data-stu-id="a8b3e-149">Relationship</span></span>   | <span data-ttu-id="a8b3e-150">类型</span><span class="sxs-lookup"><span data-stu-id="a8b3e-150">Type</span></span>    | <span data-ttu-id="a8b3e-151">说明</span><span class="sxs-lookup"><span data-stu-id="a8b3e-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8b3e-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8b3e-152">teamsApp</span></span>|[<span data-ttu-id="a8b3e-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8b3e-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="a8b3e-154">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-154">The app that is installed.</span></span> |
|<span data-ttu-id="a8b3e-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8b3e-155">teamsAppDefinition</span></span>|[<span data-ttu-id="a8b3e-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8b3e-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="a8b3e-157">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a8b3e-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a8b3e-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8b3e-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a8b3e-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a8b3e-159">See also</span></span>

- [<span data-ttu-id="a8b3e-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8b3e-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a8b3e-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8b3e-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a8b3e-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8b3e-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="a8b3e-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8b3e-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

