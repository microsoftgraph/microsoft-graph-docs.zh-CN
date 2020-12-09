---
title: userScopeTeamsAppInstallation 资源类型
description: 代表在用户的个人作用域中安装的 teamsApp。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70ebdcb30c67d59e3a12c4a0514314015e163c17
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607019"
---
# <a name="userscopeteamsappinstallation-resource-type"></a><span data-ttu-id="1ecc8-103">userScopeTeamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ecc8-103">userScopeTeamsAppInstallation resource type</span></span>

<span data-ttu-id="1ecc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ecc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ecc8-105">代表在[用户](user.md)的个人作用域中安装的[teamsApp](teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-105">Represents a [teamsApp](teamsapp.md) installed in the personal scope of a [user](user.md).</span></span> <span data-ttu-id="1ecc8-106">作为应用程序一部分的任何 bot 都将成为应用程序添加到的用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-106">Any bots that are part of the app will become part of a user's personal scope that the app is added to.</span></span>
<span data-ttu-id="1ecc8-107">此类型继承自 [teamsAppInstallation](teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-107">This type inherits from [teamsAppInstallation](teamsappinstallation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1ecc8-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ecc8-108">Methods</span></span>

| <span data-ttu-id="1ecc8-109">方法</span><span class="sxs-lookup"><span data-stu-id="1ecc8-109">Method</span></span>       | <span data-ttu-id="1ecc8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ecc8-110">Return Type</span></span>  |<span data-ttu-id="1ecc8-111">Description</span><span class="sxs-lookup"><span data-stu-id="1ecc8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ecc8-112">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="1ecc8-112">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="1ecc8-113">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ecc8-113">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="1ecc8-114">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-114">List apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="1ecc8-115">获取已安装的用户应用程序</span><span class="sxs-lookup"><span data-stu-id="1ecc8-115">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="1ecc8-116">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1ecc8-116">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="1ecc8-117">列出在用户的个人范围内安装的指定应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-117">List the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="1ecc8-118">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="1ecc8-118">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | <span data-ttu-id="1ecc8-119">无</span><span class="sxs-lookup"><span data-stu-id="1ecc8-119">None</span></span> | <span data-ttu-id="1ecc8-120">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-120">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="1ecc8-121">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="1ecc8-121">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="1ecc8-122">无</span><span class="sxs-lookup"><span data-stu-id="1ecc8-122">None</span></span> | <span data-ttu-id="1ecc8-123">删除) 用户的个人作用域中的应用程序 (卸载。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-123">Removes (uninstalls) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="1ecc8-124">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="1ecc8-124">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="1ecc8-125">无</span><span class="sxs-lookup"><span data-stu-id="1ecc8-125">None</span></span> | <span data-ttu-id="1ecc8-126">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-126">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="1ecc8-127">在用户和应用之间获取聊天</span><span class="sxs-lookup"><span data-stu-id="1ecc8-127">Get chat between user and app</span></span>](../api/userscopeteamsappinstallation-get-chat.md) | [<span data-ttu-id="1ecc8-128">聊天</span><span class="sxs-lookup"><span data-stu-id="1ecc8-128">chat</span></span>](chat.md) | <span data-ttu-id="1ecc8-129">列出用户与应用之间的一对一聊天。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-129">Lists one-on-one chat between the user and the app.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ecc8-130">属性</span><span class="sxs-lookup"><span data-stu-id="1ecc8-130">Properties</span></span>

| <span data-ttu-id="1ecc8-131">属性</span><span class="sxs-lookup"><span data-stu-id="1ecc8-131">Property</span></span>            | <span data-ttu-id="1ecc8-132">类型</span><span class="sxs-lookup"><span data-stu-id="1ecc8-132">Type</span></span>     | <span data-ttu-id="1ecc8-133">说明</span><span class="sxs-lookup"><span data-stu-id="1ecc8-133">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1ecc8-134">id</span><span class="sxs-lookup"><span data-stu-id="1ecc8-134">id</span></span>                  | <span data-ttu-id="1ecc8-135">string</span><span class="sxs-lookup"><span data-stu-id="1ecc8-135">string</span></span>   | <span data-ttu-id="1ecc8-136">唯一 ID (团队应用程序 ID) 。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-136">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1ecc8-137">关系</span><span class="sxs-lookup"><span data-stu-id="1ecc8-137">Relationships</span></span>

| <span data-ttu-id="1ecc8-138">关系</span><span class="sxs-lookup"><span data-stu-id="1ecc8-138">Relationship</span></span>   | <span data-ttu-id="1ecc8-139">类型</span><span class="sxs-lookup"><span data-stu-id="1ecc8-139">Type</span></span>    | <span data-ttu-id="1ecc8-140">Description</span><span class="sxs-lookup"><span data-stu-id="1ecc8-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1ecc8-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecc8-141">teamsApp</span></span>|[<span data-ttu-id="1ecc8-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecc8-142">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="1ecc8-143">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-143">The app that is installed.</span></span> |
|<span data-ttu-id="1ecc8-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1ecc8-144">teamsAppDefinition</span></span>|[<span data-ttu-id="1ecc8-145">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1ecc8-145">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="1ecc8-146">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-146">The details of this version of the app.</span></span> |
|<span data-ttu-id="1ecc8-147">聊天</span><span class="sxs-lookup"><span data-stu-id="1ecc8-147">chat</span></span> |[<span data-ttu-id="1ecc8-148">聊天</span><span class="sxs-lookup"><span data-stu-id="1ecc8-148">chat</span></span>](chat.md) | <span data-ttu-id="1ecc8-149">用户和团队应用程序之间的聊天。</span><span class="sxs-lookup"><span data-stu-id="1ecc8-149">The chat between the user and Teams app.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="1ecc8-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ecc8-150">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1ecc8-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1ecc8-151">See also</span></span>

- [<span data-ttu-id="1ecc8-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1ecc8-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="1ecc8-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="1ecc8-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="1ecc8-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1ecc8-154">teamsTab</span></span>](../resources/teamstab.md)

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

