---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a74323dc8a5e5907ea8a91553537fc8259acea6c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046585"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="4e1c0-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e1c0-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="4e1c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e1c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e1c0-105">安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="4e1c0-106">作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="4e1c0-107">方法</span><span class="sxs-lookup"><span data-stu-id="4e1c0-107">Methods</span></span>

| <span data-ttu-id="4e1c0-108">方法</span><span class="sxs-lookup"><span data-stu-id="4e1c0-108">Method</span></span>       | <span data-ttu-id="4e1c0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4e1c0-109">Return Type</span></span>  |<span data-ttu-id="4e1c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e1c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e1c0-111">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1c0-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="4e1c0-112">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1c0-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="4e1c0-113">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="4e1c0-114">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="4e1c0-114">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="4e1c0-115">无</span><span class="sxs-lookup"><span data-stu-id="4e1c0-115">None</span></span> | <span data-ttu-id="4e1c0-116">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="4e1c0-117">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="4e1c0-117">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="4e1c0-118">无</span><span class="sxs-lookup"><span data-stu-id="4e1c0-118">None</span></span> | <span data-ttu-id="4e1c0-119">从团队中删除应用) 的 (卸载。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="4e1c0-120">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1c0-120">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="4e1c0-121">无</span><span class="sxs-lookup"><span data-stu-id="4e1c0-121">None</span></span> | <span data-ttu-id="4e1c0-122">升级到团队中安装的应用程序的最新版本。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-122">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="4e1c0-123">列出为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="4e1c0-123">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="4e1c0-124">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4e1c0-124">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="4e1c0-125">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-125">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="4e1c0-126">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1c0-126">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="4e1c0-127">添加 (安装) 用户的个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-127">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="4e1c0-128">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1c0-128">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="4e1c0-129">无</span><span class="sxs-lookup"><span data-stu-id="4e1c0-129">None</span></span> | <span data-ttu-id="4e1c0-130">删除) 用户的个人作用域中的应用程序 (卸载。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-130">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="4e1c0-131">升级为用户安装的应用</span><span class="sxs-lookup"><span data-stu-id="4e1c0-131">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="4e1c0-132">无</span><span class="sxs-lookup"><span data-stu-id="4e1c0-132">None</span></span> | <span data-ttu-id="4e1c0-133">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-133">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e1c0-134">属性</span><span class="sxs-lookup"><span data-stu-id="4e1c0-134">Properties</span></span>

| <span data-ttu-id="4e1c0-135">属性</span><span class="sxs-lookup"><span data-stu-id="4e1c0-135">Property</span></span>            | <span data-ttu-id="4e1c0-136">类型</span><span class="sxs-lookup"><span data-stu-id="4e1c0-136">Type</span></span>     | <span data-ttu-id="4e1c0-137">说明</span><span class="sxs-lookup"><span data-stu-id="4e1c0-137">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="4e1c0-138">id</span><span class="sxs-lookup"><span data-stu-id="4e1c0-138">id</span></span>                  | <span data-ttu-id="4e1c0-139">string</span><span class="sxs-lookup"><span data-stu-id="4e1c0-139">string</span></span>   | <span data-ttu-id="4e1c0-140">唯一 ID (团队的 ap ID) 。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-140">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="4e1c0-141">关系</span><span class="sxs-lookup"><span data-stu-id="4e1c0-141">Relationships</span></span>

| <span data-ttu-id="4e1c0-142">关系</span><span class="sxs-lookup"><span data-stu-id="4e1c0-142">Relationship</span></span>   | <span data-ttu-id="4e1c0-143">类型</span><span class="sxs-lookup"><span data-stu-id="4e1c0-143">Type</span></span>    | <span data-ttu-id="4e1c0-144">说明</span><span class="sxs-lookup"><span data-stu-id="4e1c0-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4e1c0-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4e1c0-145">teamsApp</span></span>|[<span data-ttu-id="4e1c0-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4e1c0-146">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="4e1c0-147">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-147">The app that is installed.</span></span> |
|<span data-ttu-id="4e1c0-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4e1c0-148">teamsAppDefinition</span></span>|[<span data-ttu-id="4e1c0-149">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4e1c0-149">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="4e1c0-150">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4e1c0-150">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e1c0-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e1c0-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4e1c0-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4e1c0-152">See also</span></span>

- [<span data-ttu-id="4e1c0-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4e1c0-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="4e1c0-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="4e1c0-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="4e1c0-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4e1c0-155">teamsTab</span></span>](../resources/teamstab.md)

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


