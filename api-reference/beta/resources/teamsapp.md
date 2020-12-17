---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb7c75f144f2056e610e45f86b44a19d9211f306
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706120"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="ccf0f-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccf0f-103">teamsApp resource type</span></span>

<span data-ttu-id="ccf0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccf0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccf0f-105">代表[Microsoft Teams](teams-api-overview.md) 应用目录中的一个应用.</span><span class="sxs-lookup"><span data-stu-id="ccf0f-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="ccf0f-106">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/team-post-installedapps.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="ccf0f-107">方法</span><span class="sxs-lookup"><span data-stu-id="ccf0f-107">Methods</span></span>

| <span data-ttu-id="ccf0f-108">方法</span><span class="sxs-lookup"><span data-stu-id="ccf0f-108">Method</span></span>       | <span data-ttu-id="ccf0f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ccf0f-109">Return Type</span></span>  |<span data-ttu-id="ccf0f-110">说明</span><span class="sxs-lookup"><span data-stu-id="ccf0f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ccf0f-111">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="ccf0f-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="ccf0f-112">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccf0f-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="ccf0f-113">列出 Microsoft Teams 应用目录中的所有应用。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="ccf0f-114">将应用程序上载到目录</span><span class="sxs-lookup"><span data-stu-id="ccf0f-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="ccf0f-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ccf0f-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ccf0f-116">将应用上载到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="ccf0f-117">更新目录中的应用</span><span class="sxs-lookup"><span data-stu-id="ccf0f-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="ccf0f-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ccf0f-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ccf0f-119">更新组织的应用程序目录中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="ccf0f-120">从目录删除应用程序</span><span class="sxs-lookup"><span data-stu-id="ccf0f-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="ccf0f-121">无</span><span class="sxs-lookup"><span data-stu-id="ccf0f-121">None</span></span> | <span data-ttu-id="ccf0f-122">从组织的应用程序目录中删除应用。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-122">Remove an app from your organization's app catalog.</span></span>|
|[<span data-ttu-id="ccf0f-123">获取与目录中的应用程序关联的机器人</span><span class="sxs-lookup"><span data-stu-id="ccf0f-123">Get bot associated with app in catalog</span></span>](../api/teamworkbot-get.md) | [<span data-ttu-id="ccf0f-124">teamworkbot</span><span class="sxs-lookup"><span data-stu-id="ccf0f-124">teamworkbot</span></span>](teamworkbot.md) | <span data-ttu-id="ccf0f-125">获取与 Teams 应用关联的机器人。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-125">Get the bot associated with the Teams app.</span></span>|

## <a name="properties"></a><span data-ttu-id="ccf0f-126">属性</span><span class="sxs-lookup"><span data-stu-id="ccf0f-126">Properties</span></span>

| <span data-ttu-id="ccf0f-127">属性</span><span class="sxs-lookup"><span data-stu-id="ccf0f-127">Property</span></span>            | <span data-ttu-id="ccf0f-128">类型</span><span class="sxs-lookup"><span data-stu-id="ccf0f-128">Type</span></span>     | <span data-ttu-id="ccf0f-129">说明</span><span class="sxs-lookup"><span data-stu-id="ccf0f-129">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ccf0f-130">id</span><span class="sxs-lookup"><span data-stu-id="ccf0f-130">id</span></span>                  | <span data-ttu-id="ccf0f-131">string</span><span class="sxs-lookup"><span data-stu-id="ccf0f-131">string</span></span>   | <span data-ttu-id="ccf0f-132">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-132">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="ccf0f-133">externalId</span><span class="sxs-lookup"><span data-stu-id="ccf0f-133">externalId</span></span>          | <span data-ttu-id="ccf0f-134">string</span><span class="sxs-lookup"><span data-stu-id="ccf0f-134">string</span></span>   | <span data-ttu-id="ccf0f-135">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-135">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="ccf0f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ccf0f-136">displayName</span></span>                | <span data-ttu-id="ccf0f-137">string</span><span class="sxs-lookup"><span data-stu-id="ccf0f-137">string</span></span>   | <span data-ttu-id="ccf0f-138">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-138">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="ccf0f-139">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="ccf0f-139">distributionMethod</span></span>  | <span data-ttu-id="ccf0f-140">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="ccf0f-140">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="ccf0f-141">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-141">The method of distribution for the app.</span></span> <span data-ttu-id="ccf0f-142">只读。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-142">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="ccf0f-143">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="ccf0f-143">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="ccf0f-144">成员</span><span class="sxs-lookup"><span data-stu-id="ccf0f-144">Member</span></span>|<span data-ttu-id="ccf0f-145">值</span><span class="sxs-lookup"><span data-stu-id="ccf0f-145">Value</span></span>|<span data-ttu-id="ccf0f-146">说明</span><span class="sxs-lookup"><span data-stu-id="ccf0f-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf0f-147">商店</span><span class="sxs-lookup"><span data-stu-id="ccf0f-147">store</span></span>|<span data-ttu-id="ccf0f-148">0</span><span class="sxs-lookup"><span data-stu-id="ccf0f-148">0</span></span>| <span data-ttu-id="ccf0f-149">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-149">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="ccf0f-150">组织</span><span class="sxs-lookup"><span data-stu-id="ccf0f-150">organization</span></span>|<span data-ttu-id="ccf0f-151">1</span><span class="sxs-lookup"><span data-stu-id="ccf0f-151">1</span></span>|<span data-ttu-id="ccf0f-152">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-152">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="ccf0f-153">旁加载</span><span class="sxs-lookup"><span data-stu-id="ccf0f-153">sideloaded</span></span>|<span data-ttu-id="ccf0f-154">2</span><span class="sxs-lookup"><span data-stu-id="ccf0f-154">2</span></span>|<span data-ttu-id="ccf0f-155">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-155">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf0f-156">关系</span><span class="sxs-lookup"><span data-stu-id="ccf0f-156">Relationships</span></span>

| <span data-ttu-id="ccf0f-157">关系</span><span class="sxs-lookup"><span data-stu-id="ccf0f-157">Relationship</span></span> | <span data-ttu-id="ccf0f-158">类型</span><span class="sxs-lookup"><span data-stu-id="ccf0f-158">Type</span></span>   | <span data-ttu-id="ccf0f-159">说明</span><span class="sxs-lookup"><span data-stu-id="ccf0f-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ccf0f-160">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="ccf0f-160">appDefinitions</span></span>|<span data-ttu-id="ccf0f-161">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccf0f-161">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="ccf0f-162">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ccf0f-162">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccf0f-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccf0f-163">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "string",
  "distributionMethod": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="ccf0f-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ccf0f-164">See also</span></span>

- [<span data-ttu-id="ccf0f-165">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ccf0f-165">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ccf0f-166">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ccf0f-166">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="ccf0f-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ccf0f-167">teamsTab</span></span>](../resources/teamstab.md)

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



