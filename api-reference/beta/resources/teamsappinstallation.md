---
title: teamsAppInstallation 资源类型
description: '安装在团队中的 teamsApp、聊天或用户的个人作用域。 '
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e1246616b7a3d76c6170a02286a2cde2a15d3a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908507"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="48237-103">teamsAppInstallation 资源类型</span><span class="sxs-lookup"><span data-stu-id="48237-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48237-104">安装在[团队](team.md)中的[teamsApp](teamsapp.md) 、[聊天](chat.md)或[用户](user.md)的个人作用域。</span><span class="sxs-lookup"><span data-stu-id="48237-104">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="48237-105">作为应用程序一部分的任何 bot 都将成为向其添加应用程序的任何团队、聊天或用户个人范围的一部分。</span><span class="sxs-lookup"><span data-stu-id="48237-105">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="48237-106">方法</span><span class="sxs-lookup"><span data-stu-id="48237-106">Methods</span></span>

| <span data-ttu-id="48237-107">方法</span><span class="sxs-lookup"><span data-stu-id="48237-107">Method</span></span>       | <span data-ttu-id="48237-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="48237-108">Return Type</span></span>  |<span data-ttu-id="48237-109">说明</span><span class="sxs-lookup"><span data-stu-id="48237-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48237-110">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-110">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="48237-111">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48237-111">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="48237-112">列出在团队中安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="48237-113">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="48237-113">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="48237-114">无</span><span class="sxs-lookup"><span data-stu-id="48237-114">None</span></span> | <span data-ttu-id="48237-115">将应用添加（安装）到团队。</span><span class="sxs-lookup"><span data-stu-id="48237-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="48237-116">从团队中删除应用</span><span class="sxs-lookup"><span data-stu-id="48237-116">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="48237-117">无</span><span class="sxs-lookup"><span data-stu-id="48237-117">None</span></span> | <span data-ttu-id="48237-118">从团队中删除 (卸载) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="48237-119">升级在团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-119">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="48237-120">无</span><span class="sxs-lookup"><span data-stu-id="48237-120">None</span></span> | <span data-ttu-id="48237-121">升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-121">Upgrades to the latest version of the app.</span></span>|
|[<span data-ttu-id="48237-122">列出为用户安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-122">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="48237-123">[teamsAppInstallation](teamsappinstallation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48237-123">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="48237-124">列出在用户的个人范围内安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-124">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="48237-125">为用户添加应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-125">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="48237-126">在用户的个人作用域中添加 (安装) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-126">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="48237-127">删除用户的应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-127">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="48237-128">无</span><span class="sxs-lookup"><span data-stu-id="48237-128">None</span></span> | <span data-ttu-id="48237-129">删除 (卸载) 用户个人作用域中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-129">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="48237-130">为用户安装的升级应用程序</span><span class="sxs-lookup"><span data-stu-id="48237-130">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="48237-131">无</span><span class="sxs-lookup"><span data-stu-id="48237-131">None</span></span> | <span data-ttu-id="48237-132">升级到在用户的个人范围内安装的最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-132">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="48237-133">属性</span><span class="sxs-lookup"><span data-stu-id="48237-133">Properties</span></span>

| <span data-ttu-id="48237-134">属性</span><span class="sxs-lookup"><span data-stu-id="48237-134">Property</span></span>            | <span data-ttu-id="48237-135">类型</span><span class="sxs-lookup"><span data-stu-id="48237-135">Type</span></span>     | <span data-ttu-id="48237-136">说明</span><span class="sxs-lookup"><span data-stu-id="48237-136">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="48237-137">id</span><span class="sxs-lookup"><span data-stu-id="48237-137">id</span></span>                  | <span data-ttu-id="48237-138">string</span><span class="sxs-lookup"><span data-stu-id="48237-138">string</span></span>   | <span data-ttu-id="48237-139">唯一的 ID (而不是团队的 ap ID)。</span><span class="sxs-lookup"><span data-stu-id="48237-139">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="48237-140">关系</span><span class="sxs-lookup"><span data-stu-id="48237-140">Relationships</span></span>

| <span data-ttu-id="48237-141">关系</span><span class="sxs-lookup"><span data-stu-id="48237-141">Relationship</span></span>   | <span data-ttu-id="48237-142">类型</span><span class="sxs-lookup"><span data-stu-id="48237-142">Type</span></span>    | <span data-ttu-id="48237-143">说明</span><span class="sxs-lookup"><span data-stu-id="48237-143">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="48237-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48237-144">teamsApp</span></span>|[<span data-ttu-id="48237-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48237-145">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="48237-146">已安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="48237-146">The app that is installed.</span></span> |
|<span data-ttu-id="48237-147">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="48237-147">teamsAppDefinition</span></span>|[<span data-ttu-id="48237-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="48237-148">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="48237-149">此版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="48237-149">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48237-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48237-150">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="48237-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="48237-151">See also</span></span>

- [<span data-ttu-id="48237-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="48237-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="48237-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="48237-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="48237-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="48237-154">teamsTab</span></span>](../resources/teamstab.md)

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
