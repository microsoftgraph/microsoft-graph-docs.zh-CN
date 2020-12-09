---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b34450f29ccb1fb02cf1751c78f312c71fdefc9
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606951"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="1966d-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1966d-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="1966d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1966d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1966d-105">安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="1966d-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="1966d-106">作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="1966d-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="1966d-107">`id` **TeamsAppInstallation** 资源的值与 `id` 关联的 **teamsApp** 资源的值不同。</span><span class="sxs-lookup"><span data-stu-id="1966d-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="1966d-108">方法</span><span class="sxs-lookup"><span data-stu-id="1966d-108">Methods</span></span>

| <span data-ttu-id="1966d-109">方法</span><span class="sxs-lookup"><span data-stu-id="1966d-109">Method</span></span>       | <span data-ttu-id="1966d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1966d-110">Return Type</span></span>  |<span data-ttu-id="1966d-111">Description</span><span class="sxs-lookup"><span data-stu-id="1966d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1966d-112">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="1966d-113">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1966d-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="1966d-114">列出团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="1966d-115">获取团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="1966d-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1966d-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="1966d-117">获取团队中安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="1966d-118">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="1966d-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="1966d-119">无</span><span class="sxs-lookup"><span data-stu-id="1966d-119">None</span></span> | <span data-ttu-id="1966d-120">向团队添加 (安装) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="1966d-121">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="1966d-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="1966d-122">无</span><span class="sxs-lookup"><span data-stu-id="1966d-122">None</span></span> | <span data-ttu-id="1966d-123">删除 (从团队中的应用) 卸载。</span><span class="sxs-lookup"><span data-stu-id="1966d-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="1966d-124">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="1966d-125">无</span><span class="sxs-lookup"><span data-stu-id="1966d-125">None</span></span> | <span data-ttu-id="1966d-126">将团队中安装的应用程序升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="1966d-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="1966d-127">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="1966d-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="1966d-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1966d-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="1966d-129">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="1966d-130">获取已安装的用户应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="1966d-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1966d-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="1966d-132">获取在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="1966d-133">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="1966d-134">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="1966d-135">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="1966d-136">无</span><span class="sxs-lookup"><span data-stu-id="1966d-136">None</span></span> | <span data-ttu-id="1966d-137">删除 (卸载) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="1966d-138">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="1966d-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="1966d-139">无</span><span class="sxs-lookup"><span data-stu-id="1966d-139">None</span></span> | <span data-ttu-id="1966d-140">将用户的个人范围内安装的应用程序升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="1966d-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="1966d-141">列出聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="1966d-142">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1966d-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="1966d-143">列出聊天中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="1966d-144">获取聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-144">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="1966d-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1966d-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="1966d-146">获取聊天中安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="1966d-147">在聊天中添加应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="1966d-148">将 (安装) 应用程序添加到聊天。</span><span class="sxs-lookup"><span data-stu-id="1966d-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="1966d-149">从聊天中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-149">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="1966d-150">无</span><span class="sxs-lookup"><span data-stu-id="1966d-150">None</span></span> | <span data-ttu-id="1966d-151">从聊天中删除 (卸载) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-151">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="1966d-152">升级聊天中的应用程序</span><span class="sxs-lookup"><span data-stu-id="1966d-152">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="1966d-153">无</span><span class="sxs-lookup"><span data-stu-id="1966d-153">None</span></span> | <span data-ttu-id="1966d-154">将聊天中安装的应用程序升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="1966d-154">Upgrade the app installed in a chat to the latest version.</span></span>|

## <a name="properties"></a><span data-ttu-id="1966d-155">属性</span><span class="sxs-lookup"><span data-stu-id="1966d-155">Properties</span></span>

| <span data-ttu-id="1966d-156">属性</span><span class="sxs-lookup"><span data-stu-id="1966d-156">Property</span></span>            | <span data-ttu-id="1966d-157">类型</span><span class="sxs-lookup"><span data-stu-id="1966d-157">Type</span></span>     | <span data-ttu-id="1966d-158">说明</span><span class="sxs-lookup"><span data-stu-id="1966d-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1966d-159">id</span><span class="sxs-lookup"><span data-stu-id="1966d-159">id</span></span>                  | <span data-ttu-id="1966d-160">string</span><span class="sxs-lookup"><span data-stu-id="1966d-160">string</span></span>   | <span data-ttu-id="1966d-161">唯一 ID (团队的 ap ID) 。</span><span class="sxs-lookup"><span data-stu-id="1966d-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1966d-162">关系</span><span class="sxs-lookup"><span data-stu-id="1966d-162">Relationships</span></span>

| <span data-ttu-id="1966d-163">关系</span><span class="sxs-lookup"><span data-stu-id="1966d-163">Relationship</span></span>   | <span data-ttu-id="1966d-164">类型</span><span class="sxs-lookup"><span data-stu-id="1966d-164">Type</span></span>    | <span data-ttu-id="1966d-165">Description</span><span class="sxs-lookup"><span data-stu-id="1966d-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1966d-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1966d-166">teamsApp</span></span>|[<span data-ttu-id="1966d-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1966d-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="1966d-168">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1966d-168">The app that is installed.</span></span> |
|<span data-ttu-id="1966d-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1966d-169">teamsAppDefinition</span></span>|[<span data-ttu-id="1966d-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1966d-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="1966d-171">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1966d-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1966d-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1966d-172">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1966d-173">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1966d-173">See also</span></span>

- [<span data-ttu-id="1966d-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1966d-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1966d-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1966d-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="1966d-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1966d-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="1966d-177">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1966d-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


