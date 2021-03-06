---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2ffa5b3f5562e83d1e1e1ef64629e39a1da41cd4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472858"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="865da-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="865da-103">teamsApp resource type</span></span>

<span data-ttu-id="865da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="865da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="865da-105">代表[Microsoft Teams](teams-api-overview.md) 应用目录中的一个应用.</span><span class="sxs-lookup"><span data-stu-id="865da-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="865da-106">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/team-post-installedapps.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="865da-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="865da-107">方法</span><span class="sxs-lookup"><span data-stu-id="865da-107">Methods</span></span>

| <span data-ttu-id="865da-108">方法</span><span class="sxs-lookup"><span data-stu-id="865da-108">Method</span></span>       | <span data-ttu-id="865da-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="865da-109">Return Type</span></span>  |<span data-ttu-id="865da-110">说明</span><span class="sxs-lookup"><span data-stu-id="865da-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="865da-111">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="865da-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="865da-112">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="865da-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="865da-113">列出 Microsoft Teams 应用目录中的所有应用。</span><span class="sxs-lookup"><span data-stu-id="865da-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="865da-114">上传应用到目录</span><span class="sxs-lookup"><span data-stu-id="865da-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="865da-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="865da-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="865da-116">将应用上传到组织的应用目录。</span><span class="sxs-lookup"><span data-stu-id="865da-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="865da-117">更新目录中的应用</span><span class="sxs-lookup"><span data-stu-id="865da-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="865da-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="865da-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="865da-119">更新组织应用目录中的应用。</span><span class="sxs-lookup"><span data-stu-id="865da-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="865da-120">从目录中删除应用</span><span class="sxs-lookup"><span data-stu-id="865da-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="865da-121">无</span><span class="sxs-lookup"><span data-stu-id="865da-121">None</span></span> | <span data-ttu-id="865da-122">从组织应用目录中删除应用。</span><span class="sxs-lookup"><span data-stu-id="865da-122">Remove an app from your organization's app catalog.</span></span>|
|[<span data-ttu-id="865da-123">获取与目录中的应用程序相关联的自动程序</span><span class="sxs-lookup"><span data-stu-id="865da-123">Get bot associated with app in catalog</span></span>](../api/teamworkbot-get.md) | [<span data-ttu-id="865da-124">团队合作</span><span class="sxs-lookup"><span data-stu-id="865da-124">teamworkbot</span></span>](teamworkbot.md) | <span data-ttu-id="865da-125">获取与 Teams 应用关联的自动程序。</span><span class="sxs-lookup"><span data-stu-id="865da-125">Get the bot associated with the Teams app.</span></span>|

## <a name="properties"></a><span data-ttu-id="865da-126">属性</span><span class="sxs-lookup"><span data-stu-id="865da-126">Properties</span></span>

| <span data-ttu-id="865da-127">属性</span><span class="sxs-lookup"><span data-stu-id="865da-127">Property</span></span>            | <span data-ttu-id="865da-128">类型</span><span class="sxs-lookup"><span data-stu-id="865da-128">Type</span></span>     | <span data-ttu-id="865da-129">说明</span><span class="sxs-lookup"><span data-stu-id="865da-129">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="865da-130">id</span><span class="sxs-lookup"><span data-stu-id="865da-130">id</span></span>                  | <span data-ttu-id="865da-131">string</span><span class="sxs-lookup"><span data-stu-id="865da-131">string</span></span>   | <span data-ttu-id="865da-132">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="865da-132">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="865da-133">externalId</span><span class="sxs-lookup"><span data-stu-id="865da-133">externalId</span></span>          | <span data-ttu-id="865da-134">string</span><span class="sxs-lookup"><span data-stu-id="865da-134">string</span></span>   | <span data-ttu-id="865da-135">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="865da-135">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="865da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="865da-136">displayName</span></span>                | <span data-ttu-id="865da-137">string</span><span class="sxs-lookup"><span data-stu-id="865da-137">string</span></span>   | <span data-ttu-id="865da-138">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="865da-138">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="865da-139">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="865da-139">distributionMethod</span></span>  | <span data-ttu-id="865da-140">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="865da-140">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="865da-141">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="865da-141">The method of distribution for the app.</span></span> <span data-ttu-id="865da-142">只读。</span><span class="sxs-lookup"><span data-stu-id="865da-142">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="865da-143">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="865da-143">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="865da-144">成员</span><span class="sxs-lookup"><span data-stu-id="865da-144">Member</span></span>|<span data-ttu-id="865da-145">值</span><span class="sxs-lookup"><span data-stu-id="865da-145">Value</span></span>|<span data-ttu-id="865da-146">说明</span><span class="sxs-lookup"><span data-stu-id="865da-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="865da-147">商店</span><span class="sxs-lookup"><span data-stu-id="865da-147">store</span></span>|<span data-ttu-id="865da-148">0</span><span class="sxs-lookup"><span data-stu-id="865da-148">0</span></span>| <span data-ttu-id="865da-149">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="865da-149">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="865da-150">组织</span><span class="sxs-lookup"><span data-stu-id="865da-150">organization</span></span>|<span data-ttu-id="865da-151">1</span><span class="sxs-lookup"><span data-stu-id="865da-151">1</span></span>|<span data-ttu-id="865da-152">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="865da-152">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="865da-153">旁加载</span><span class="sxs-lookup"><span data-stu-id="865da-153">sideloaded</span></span>|<span data-ttu-id="865da-154">2</span><span class="sxs-lookup"><span data-stu-id="865da-154">2</span></span>|<span data-ttu-id="865da-155">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="865da-155">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="865da-156">关系</span><span class="sxs-lookup"><span data-stu-id="865da-156">Relationships</span></span>

| <span data-ttu-id="865da-157">关系</span><span class="sxs-lookup"><span data-stu-id="865da-157">Relationship</span></span> | <span data-ttu-id="865da-158">类型</span><span class="sxs-lookup"><span data-stu-id="865da-158">Type</span></span>   | <span data-ttu-id="865da-159">说明</span><span class="sxs-lookup"><span data-stu-id="865da-159">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="865da-160">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="865da-160">appDefinitions</span></span>|<span data-ttu-id="865da-161">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="865da-161">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="865da-162">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="865da-162">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="865da-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="865da-163">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="865da-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="865da-164">See also</span></span>

- [<span data-ttu-id="865da-165">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="865da-165">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="865da-166">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="865da-166">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="865da-167">teamsTab</span><span class="sxs-lookup"><span data-stu-id="865da-167">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


