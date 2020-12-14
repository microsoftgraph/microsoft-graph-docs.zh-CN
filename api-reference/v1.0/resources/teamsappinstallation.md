---
title: teamsAppInstallation 资源类型
description: 表示安装在团队中的 teamsApp 或用户的个人作用域。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da55c4cf7b20558258493c69c46e2b26107f4aed
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660070"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="35909-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="35909-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="35909-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35909-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35909-105">表示 [安装在团队](teamsapp.md) 中的 [teamsApp](team.md) 或用户的个人 [作用域](user.md)。</span><span class="sxs-lookup"><span data-stu-id="35909-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="35909-106">作为应用一部分的任何机器人都将成为应用添加到的任何团队或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="35909-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="35909-107">**teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。</span><span class="sxs-lookup"><span data-stu-id="35909-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="35909-108">方法</span><span class="sxs-lookup"><span data-stu-id="35909-108">Methods</span></span>

| <span data-ttu-id="35909-109">方法</span><span class="sxs-lookup"><span data-stu-id="35909-109">Method</span></span>       | <span data-ttu-id="35909-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="35909-110">Return Type</span></span>  |<span data-ttu-id="35909-111">说明</span><span class="sxs-lookup"><span data-stu-id="35909-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35909-112">列出在团队中安装的应用</span><span class="sxs-lookup"><span data-stu-id="35909-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="35909-113">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35909-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="35909-114">列出在团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="35909-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="35909-115">在团队中安装应用</span><span class="sxs-lookup"><span data-stu-id="35909-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="35909-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35909-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="35909-117">获取在团队中安装的指定应用。</span><span class="sxs-lookup"><span data-stu-id="35909-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="35909-118">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="35909-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="35909-119">无</span><span class="sxs-lookup"><span data-stu-id="35909-119">None</span></span> | <span data-ttu-id="35909-120">添加 (将) 安装到团队。</span><span class="sxs-lookup"><span data-stu-id="35909-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="35909-121">升级团队中安装的应用</span><span class="sxs-lookup"><span data-stu-id="35909-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="35909-122">无</span><span class="sxs-lookup"><span data-stu-id="35909-122">None</span></span> | <span data-ttu-id="35909-123">将团队中安装的应用升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="35909-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="35909-124">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="35909-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="35909-125">无</span><span class="sxs-lookup"><span data-stu-id="35909-125">None</span></span> | <span data-ttu-id="35909-126">从 (中删除) 卸载应用。</span><span class="sxs-lookup"><span data-stu-id="35909-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="35909-127">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="35909-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="35909-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35909-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="35909-129">列出在用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="35909-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="35909-130">为用户安装应用</span><span class="sxs-lookup"><span data-stu-id="35909-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="35909-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35909-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="35909-132">获取在用户的个人范围内安装的指定应用。</span><span class="sxs-lookup"><span data-stu-id="35909-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="35909-133">为用户添加应用</span><span class="sxs-lookup"><span data-stu-id="35909-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="35909-134">添加 (在) 范围内安装应用。</span><span class="sxs-lookup"><span data-stu-id="35909-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="35909-135">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="35909-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="35909-136">无</span><span class="sxs-lookup"><span data-stu-id="35909-136">None</span></span> | <span data-ttu-id="35909-137">将用户个人范围内安装的应用升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="35909-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="35909-138">为用户删除应用</span><span class="sxs-lookup"><span data-stu-id="35909-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="35909-139">无</span><span class="sxs-lookup"><span data-stu-id="35909-139">None</span></span> | <span data-ttu-id="35909-140">删除 (用户) 范围内卸载应用。</span><span class="sxs-lookup"><span data-stu-id="35909-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|


## <a name="properties"></a><span data-ttu-id="35909-141">属性</span><span class="sxs-lookup"><span data-stu-id="35909-141">Properties</span></span>

| <span data-ttu-id="35909-142">属性</span><span class="sxs-lookup"><span data-stu-id="35909-142">Property</span></span>            | <span data-ttu-id="35909-143">类型</span><span class="sxs-lookup"><span data-stu-id="35909-143">Type</span></span>     | <span data-ttu-id="35909-144">说明</span><span class="sxs-lookup"><span data-stu-id="35909-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="35909-145">id</span><span class="sxs-lookup"><span data-stu-id="35909-145">id</span></span>                  | <span data-ttu-id="35909-146">string</span><span class="sxs-lookup"><span data-stu-id="35909-146">string</span></span>   | <span data-ttu-id="35909-147">唯一 ID (不是 Teams 应用 ID) 。</span><span class="sxs-lookup"><span data-stu-id="35909-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="35909-148">关系</span><span class="sxs-lookup"><span data-stu-id="35909-148">Relationships</span></span>

| <span data-ttu-id="35909-149">关系</span><span class="sxs-lookup"><span data-stu-id="35909-149">Relationship</span></span>   | <span data-ttu-id="35909-150">类型</span><span class="sxs-lookup"><span data-stu-id="35909-150">Type</span></span>    | <span data-ttu-id="35909-151">说明</span><span class="sxs-lookup"><span data-stu-id="35909-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="35909-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35909-152">teamsApp</span></span>|[<span data-ttu-id="35909-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35909-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="35909-154">安装的应用。</span><span class="sxs-lookup"><span data-stu-id="35909-154">The app that is installed.</span></span> |
|<span data-ttu-id="35909-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35909-155">teamsAppDefinition</span></span>|[<span data-ttu-id="35909-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35909-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="35909-157">此版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="35909-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="35909-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35909-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="35909-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="35909-159">See also</span></span>

- [<span data-ttu-id="35909-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35909-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="35909-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="35909-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="35909-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35909-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="35909-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="35909-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

