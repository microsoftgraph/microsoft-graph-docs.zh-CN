---
title: userScopeTeamsAppInstallation 资源类型
description: 代表在用户的个人作用域中安装的 teamsApp。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 30df2c14f8723dedd25fb7c4e5b2a00481338dc3
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606858"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="e131d-103">userScopeTeamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e131d-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="e131d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e131d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e131d-105">代表在[用户](user.md)的个人作用域中安装的[teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="e131d-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="e131d-106">作为应用程序一部分的任何 bot 都将成为应用程序添加到的用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="e131d-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="e131d-107">此类型继承自 [teamsAppInstallation](teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="e131d-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e131d-108">`id` **TeamsAppInstallation** 资源的值与 `id` 关联的 **teamsApp** 资源的值不同。</span><span class="sxs-lookup"><span data-stu-id="e131d-108">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="e131d-109">方法</span><span class="sxs-lookup"><span data-stu-id="e131d-109">Methods</span></span>

| <span data-ttu-id="e131d-110">方法</span><span class="sxs-lookup"><span data-stu-id="e131d-110">Method</span></span>       | <span data-ttu-id="e131d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e131d-111">Return Type</span></span>  |<span data-ttu-id="e131d-112">Description</span><span class="sxs-lookup"><span data-stu-id="e131d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e131d-113">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="e131d-113">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="e131d-114">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e131d-114">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="e131d-115">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-115">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="e131d-116">为用户获取已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="e131d-116">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="e131d-117">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e131d-117">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="e131d-118">列出在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-118">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="e131d-119">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="e131d-119">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | <span data-ttu-id="e131d-120">无</span><span class="sxs-lookup"><span data-stu-id="e131d-120">None</span></span> | <span data-ttu-id="e131d-121">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-121">Add (install) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="e131d-122">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="e131d-122">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="e131d-123">无</span><span class="sxs-lookup"><span data-stu-id="e131d-123">None</span></span> | <span data-ttu-id="e131d-124">删除 (卸载) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-124">Remove (uninstall) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="e131d-125">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="e131d-125">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="e131d-126">无</span><span class="sxs-lookup"><span data-stu-id="e131d-126">None</span></span> | <span data-ttu-id="e131d-127">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-127">Upgrade to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e131d-128">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="e131d-128">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="e131d-129">聊天</span><span class="sxs-lookup"><span data-stu-id="e131d-129">chat</span></span>](chat.md) | <span data-ttu-id="e131d-130">在用户和应用程序之间列出一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="e131d-130">List one-on-one chats between a user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="e131d-131">属性</span><span class="sxs-lookup"><span data-stu-id="e131d-131">Properties</span></span>

| <span data-ttu-id="e131d-132">属性</span><span class="sxs-lookup"><span data-stu-id="e131d-132">Property</span></span>            | <span data-ttu-id="e131d-133">类型</span><span class="sxs-lookup"><span data-stu-id="e131d-133">Type</span></span>     | <span data-ttu-id="e131d-134">说明</span><span class="sxs-lookup"><span data-stu-id="e131d-134">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e131d-135">id</span><span class="sxs-lookup"><span data-stu-id="e131d-135">id</span></span>                  | <span data-ttu-id="e131d-136">string</span><span class="sxs-lookup"><span data-stu-id="e131d-136">string</span></span>   | <span data-ttu-id="e131d-137">唯一 ID (团队应用程序 ID) 。</span><span class="sxs-lookup"><span data-stu-id="e131d-137">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e131d-138">关系</span><span class="sxs-lookup"><span data-stu-id="e131d-138">Relationships</span></span>

| <span data-ttu-id="e131d-139">关系</span><span class="sxs-lookup"><span data-stu-id="e131d-139">Relationship</span></span>   | <span data-ttu-id="e131d-140">类型</span><span class="sxs-lookup"><span data-stu-id="e131d-140">Type</span></span>    | <span data-ttu-id="e131d-141">Description</span><span class="sxs-lookup"><span data-stu-id="e131d-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e131d-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e131d-142">teamsApp</span></span>|[<span data-ttu-id="e131d-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e131d-143">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="e131d-144">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e131d-144">The app that is installed.</span></span> |
|<span data-ttu-id="e131d-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e131d-145">teamsAppDefinition</span></span>|[<span data-ttu-id="e131d-146">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e131d-146">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="e131d-147">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e131d-147">The details of this version of the app.</span></span> |
|<span data-ttu-id="e131d-148">聊天</span><span class="sxs-lookup"><span data-stu-id="e131d-148">chat</span></span> |[<span data-ttu-id="e131d-149">聊天</span><span class="sxs-lookup"><span data-stu-id="e131d-149">chat</span></span>](chat.md) | <span data-ttu-id="e131d-150">用户和团队应用程序之间的聊天。</span><span class="sxs-lookup"><span data-stu-id="e131d-150">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="e131d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e131d-151">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userScopeTeamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="e131d-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e131d-152">See also</span></span>

- [<span data-ttu-id="e131d-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e131d-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e131d-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e131d-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e131d-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e131d-155">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userScopeTeamsAppInstallation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

