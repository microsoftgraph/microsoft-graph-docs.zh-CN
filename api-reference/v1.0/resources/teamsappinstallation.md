---
title: teamsAppInstallation 资源类型
description: 代表在团队中安装的 teamsApp 或用户的个人作用域。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c872d41ebc09978d9dc54ac01d82cb33258541d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607033"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="856c7-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="856c7-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="856c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="856c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="856c7-105">代表在[团队](team.md)中安装的[teamsApp](teamsapp.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="856c7-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="856c7-106">作为应用程序一部分的任何 bot 都将成为应用程序添加到的任何团队或用户的个人作用域的一部分。</span><span class="sxs-lookup"><span data-stu-id="856c7-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="856c7-107">`id` **TeamsAppInstallation** 资源的值与 `id` 关联的 **teamsApp** 资源的值不同。</span><span class="sxs-lookup"><span data-stu-id="856c7-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="856c7-108">方法</span><span class="sxs-lookup"><span data-stu-id="856c7-108">Methods</span></span>

| <span data-ttu-id="856c7-109">方法</span><span class="sxs-lookup"><span data-stu-id="856c7-109">Method</span></span>       | <span data-ttu-id="856c7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="856c7-110">Return Type</span></span>  |<span data-ttu-id="856c7-111">Description</span><span class="sxs-lookup"><span data-stu-id="856c7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="856c7-112">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="856c7-113">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="856c7-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="856c7-114">列出团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="856c7-115">获取团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="856c7-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="856c7-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="856c7-117">获取团队中安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="856c7-118">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="856c7-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="856c7-119">无</span><span class="sxs-lookup"><span data-stu-id="856c7-119">None</span></span> | <span data-ttu-id="856c7-120">向团队添加 (安装) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="856c7-121">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="856c7-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="856c7-122">无</span><span class="sxs-lookup"><span data-stu-id="856c7-122">None</span></span> | <span data-ttu-id="856c7-123">删除 (从团队中的应用) 卸载。</span><span class="sxs-lookup"><span data-stu-id="856c7-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="856c7-124">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="856c7-125">无</span><span class="sxs-lookup"><span data-stu-id="856c7-125">None</span></span> | <span data-ttu-id="856c7-126">将团队中安装的应用程序升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="856c7-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="856c7-127">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="856c7-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="856c7-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="856c7-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="856c7-129">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="856c7-130">获取已安装的用户应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="856c7-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="856c7-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="856c7-132">获取在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="856c7-133">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="856c7-134">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="856c7-135">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="856c7-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="856c7-136">无</span><span class="sxs-lookup"><span data-stu-id="856c7-136">None</span></span> | <span data-ttu-id="856c7-137">删除 (卸载) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="856c7-138">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="856c7-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="856c7-139">无</span><span class="sxs-lookup"><span data-stu-id="856c7-139">None</span></span> | <span data-ttu-id="856c7-140">将用户的个人范围内安装的应用程序升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="856c7-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|


## <a name="properties"></a><span data-ttu-id="856c7-141">属性</span><span class="sxs-lookup"><span data-stu-id="856c7-141">Properties</span></span>

| <span data-ttu-id="856c7-142">属性</span><span class="sxs-lookup"><span data-stu-id="856c7-142">Property</span></span>            | <span data-ttu-id="856c7-143">类型</span><span class="sxs-lookup"><span data-stu-id="856c7-143">Type</span></span>     | <span data-ttu-id="856c7-144">说明</span><span class="sxs-lookup"><span data-stu-id="856c7-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="856c7-145">id</span><span class="sxs-lookup"><span data-stu-id="856c7-145">id</span></span>                  | <span data-ttu-id="856c7-146">string</span><span class="sxs-lookup"><span data-stu-id="856c7-146">string</span></span>   | <span data-ttu-id="856c7-147">唯一 ID (团队应用程序 ID) 。</span><span class="sxs-lookup"><span data-stu-id="856c7-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="856c7-148">关系</span><span class="sxs-lookup"><span data-stu-id="856c7-148">Relationships</span></span>

| <span data-ttu-id="856c7-149">关系</span><span class="sxs-lookup"><span data-stu-id="856c7-149">Relationship</span></span>   | <span data-ttu-id="856c7-150">类型</span><span class="sxs-lookup"><span data-stu-id="856c7-150">Type</span></span>    | <span data-ttu-id="856c7-151">Description</span><span class="sxs-lookup"><span data-stu-id="856c7-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="856c7-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="856c7-152">teamsApp</span></span>|[<span data-ttu-id="856c7-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="856c7-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="856c7-154">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="856c7-154">The app that is installed.</span></span> |
|<span data-ttu-id="856c7-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="856c7-155">teamsAppDefinition</span></span>|[<span data-ttu-id="856c7-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="856c7-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="856c7-157">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="856c7-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="856c7-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="856c7-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="856c7-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="856c7-159">See also</span></span>

- [<span data-ttu-id="856c7-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="856c7-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="856c7-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="856c7-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="856c7-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="856c7-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="856c7-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="856c7-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

