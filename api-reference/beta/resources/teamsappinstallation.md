---
title: teamsAppInstallation 资源类型
description: '安装在团队、聊天或用户个人作用域中的 teamsApp。 '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66cf31f21a105934181aee5e506cc2215f9ce7a9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663904"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="ef690-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef690-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="ef690-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef690-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef690-105">[TeamsApp](teamsapp.md)安装在团队[、](team.md)[聊天](chat.md)或用户的个人[作用域中](user.md)。</span><span class="sxs-lookup"><span data-stu-id="ef690-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="ef690-106">作为应用一部分的任何机器人都将成为应用添加到的任何团队、聊天或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="ef690-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="ef690-107">**teamsAppInstallation** 资源的 `id` 与关联 **teamsApp** 资源的 `id` 具有不同的值。</span><span class="sxs-lookup"><span data-stu-id="ef690-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="ef690-108">方法</span><span class="sxs-lookup"><span data-stu-id="ef690-108">Methods</span></span>

| <span data-ttu-id="ef690-109">方法</span><span class="sxs-lookup"><span data-stu-id="ef690-109">Method</span></span>       | <span data-ttu-id="ef690-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ef690-110">Return Type</span></span>  |<span data-ttu-id="ef690-111">说明</span><span class="sxs-lookup"><span data-stu-id="ef690-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef690-112">列出在团队中安装的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="ef690-113">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef690-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ef690-114">列出在团队中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="ef690-115">在团队中安装应用</span><span class="sxs-lookup"><span data-stu-id="ef690-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="ef690-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ef690-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="ef690-117">获取在团队中安装的指定应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="ef690-118">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="ef690-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="ef690-119">无</span><span class="sxs-lookup"><span data-stu-id="ef690-119">None</span></span> | <span data-ttu-id="ef690-120">添加 (将) 安装到团队。</span><span class="sxs-lookup"><span data-stu-id="ef690-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="ef690-121">升级团队中安装的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="ef690-122">无</span><span class="sxs-lookup"><span data-stu-id="ef690-122">None</span></span> | <span data-ttu-id="ef690-123">将团队中安装的应用升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="ef690-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="ef690-124">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="ef690-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="ef690-125">无</span><span class="sxs-lookup"><span data-stu-id="ef690-125">None</span></span> | <span data-ttu-id="ef690-126">从 (中删除) 卸载应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="ef690-127">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="ef690-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef690-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="ef690-129">列出在用户的个人范围内安装的应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ef690-130">为用户安装应用</span><span class="sxs-lookup"><span data-stu-id="ef690-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="ef690-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ef690-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="ef690-132">获取在用户的个人范围内安装的指定应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="ef690-133">为用户添加应用</span><span class="sxs-lookup"><span data-stu-id="ef690-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="ef690-134">添加 (在) 范围内安装应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ef690-135">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="ef690-136">无</span><span class="sxs-lookup"><span data-stu-id="ef690-136">None</span></span> | <span data-ttu-id="ef690-137">将用户个人范围内安装的应用升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="ef690-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="ef690-138">为用户删除应用</span><span class="sxs-lookup"><span data-stu-id="ef690-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="ef690-139">无</span><span class="sxs-lookup"><span data-stu-id="ef690-139">None</span></span> | <span data-ttu-id="ef690-140">删除 (用户) 范围内应用的卸载权限。</span><span class="sxs-lookup"><span data-stu-id="ef690-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="ef690-141">列出聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="ef690-142">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef690-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ef690-143">列出聊天中安装的应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="ef690-144">在聊天中安装应用</span><span class="sxs-lookup"><span data-stu-id="ef690-144">Get app installed in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="ef690-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ef690-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="ef690-146">获取在聊天中安装的指定应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="ef690-147">在聊天中添加应用</span><span class="sxs-lookup"><span data-stu-id="ef690-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="ef690-148">添加 (将) 安装到聊天中。</span><span class="sxs-lookup"><span data-stu-id="ef690-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="ef690-149">升级聊天中的应用</span><span class="sxs-lookup"><span data-stu-id="ef690-149">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="ef690-150">无</span><span class="sxs-lookup"><span data-stu-id="ef690-150">None</span></span> | <span data-ttu-id="ef690-151">将聊天中安装的应用升级到最新版本。</span><span class="sxs-lookup"><span data-stu-id="ef690-151">Upgrade the app installed in a chat to the latest version.</span></span>|
|[<span data-ttu-id="ef690-152">从聊天中删除应用</span><span class="sxs-lookup"><span data-stu-id="ef690-152">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="ef690-153">无</span><span class="sxs-lookup"><span data-stu-id="ef690-153">None</span></span> | <span data-ttu-id="ef690-154">从 (卸载) 应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-154">Remove (uninstall) app from a chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="ef690-155">属性</span><span class="sxs-lookup"><span data-stu-id="ef690-155">Properties</span></span>

| <span data-ttu-id="ef690-156">属性</span><span class="sxs-lookup"><span data-stu-id="ef690-156">Property</span></span>            | <span data-ttu-id="ef690-157">类型</span><span class="sxs-lookup"><span data-stu-id="ef690-157">Type</span></span>     | <span data-ttu-id="ef690-158">说明</span><span class="sxs-lookup"><span data-stu-id="ef690-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ef690-159">id</span><span class="sxs-lookup"><span data-stu-id="ef690-159">id</span></span>                  | <span data-ttu-id="ef690-160">string</span><span class="sxs-lookup"><span data-stu-id="ef690-160">string</span></span>   | <span data-ttu-id="ef690-161">唯一 ID (不是团队的 ap ID) 。</span><span class="sxs-lookup"><span data-stu-id="ef690-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef690-162">关系</span><span class="sxs-lookup"><span data-stu-id="ef690-162">Relationships</span></span>

| <span data-ttu-id="ef690-163">关系</span><span class="sxs-lookup"><span data-stu-id="ef690-163">Relationship</span></span>   | <span data-ttu-id="ef690-164">类型</span><span class="sxs-lookup"><span data-stu-id="ef690-164">Type</span></span>    | <span data-ttu-id="ef690-165">说明</span><span class="sxs-lookup"><span data-stu-id="ef690-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ef690-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ef690-166">teamsApp</span></span>|[<span data-ttu-id="ef690-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ef690-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="ef690-168">安装的应用。</span><span class="sxs-lookup"><span data-stu-id="ef690-168">The app that is installed.</span></span> |
|<span data-ttu-id="ef690-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ef690-169">teamsAppDefinition</span></span>|[<span data-ttu-id="ef690-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ef690-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="ef690-171">此版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ef690-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef690-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef690-172">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ef690-173">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ef690-173">See also</span></span>

- [<span data-ttu-id="ef690-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ef690-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ef690-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ef690-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="ef690-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ef690-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="ef690-177">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ef690-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


