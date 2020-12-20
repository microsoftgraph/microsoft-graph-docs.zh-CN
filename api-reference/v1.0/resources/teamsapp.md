---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 55fd373fd59f79abdfca8b3e066ca496daf8770b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706001"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="26257-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="26257-103">teamsApp resource type</span></span>

<span data-ttu-id="26257-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26257-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26257-105">代表[Microsoft Teams](teams-api-overview.md) 应用目录中的一个应用.</span><span class="sxs-lookup"><span data-stu-id="26257-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="26257-106">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/team-post-installedapps.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="26257-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/team-post-installedapps.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="26257-107">方法</span><span class="sxs-lookup"><span data-stu-id="26257-107">Methods</span></span>

| <span data-ttu-id="26257-108">方法</span><span class="sxs-lookup"><span data-stu-id="26257-108">Method</span></span>       | <span data-ttu-id="26257-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26257-109">Return Type</span></span>  |<span data-ttu-id="26257-110">说明</span><span class="sxs-lookup"><span data-stu-id="26257-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26257-111">列出目录中的应用</span><span class="sxs-lookup"><span data-stu-id="26257-111">List apps in catalog</span></span>](../api/appcatalogs-list-teamsapps.md) | <span data-ttu-id="26257-112">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26257-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="26257-113">列出 Microsoft Teams 应用目录中的所有应用。</span><span class="sxs-lookup"><span data-stu-id="26257-113">List all the apps in the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="26257-114">上传应用到目录</span><span class="sxs-lookup"><span data-stu-id="26257-114">Upload app to catalog</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="26257-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26257-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="26257-116">将应用上传到组织的应用目录。</span><span class="sxs-lookup"><span data-stu-id="26257-116">Upload an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="26257-117">更新目录中的应用</span><span class="sxs-lookup"><span data-stu-id="26257-117">Update app in catalog</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="26257-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="26257-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="26257-119">更新组织应用目录中的应用。</span><span class="sxs-lookup"><span data-stu-id="26257-119">Update an app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="26257-120">从目录中删除应用</span><span class="sxs-lookup"><span data-stu-id="26257-120">Delete app from catalog</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="26257-121">无</span><span class="sxs-lookup"><span data-stu-id="26257-121">None</span></span> | <span data-ttu-id="26257-122">从组织应用目录中删除应用。</span><span class="sxs-lookup"><span data-stu-id="26257-122">Remove an app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="26257-123">属性</span><span class="sxs-lookup"><span data-stu-id="26257-123">Properties</span></span>

| <span data-ttu-id="26257-124">属性</span><span class="sxs-lookup"><span data-stu-id="26257-124">Property</span></span>            | <span data-ttu-id="26257-125">类型</span><span class="sxs-lookup"><span data-stu-id="26257-125">Type</span></span>     | <span data-ttu-id="26257-126">说明</span><span class="sxs-lookup"><span data-stu-id="26257-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="26257-127">id</span><span class="sxs-lookup"><span data-stu-id="26257-127">id</span></span>                  | <span data-ttu-id="26257-128">string</span><span class="sxs-lookup"><span data-stu-id="26257-128">string</span></span>   | <span data-ttu-id="26257-129">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="26257-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26257-130">externalId</span><span class="sxs-lookup"><span data-stu-id="26257-130">externalId</span></span>          | <span data-ttu-id="26257-131">string</span><span class="sxs-lookup"><span data-stu-id="26257-131">string</span></span>   | <span data-ttu-id="26257-132">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="26257-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26257-133">displayName</span><span class="sxs-lookup"><span data-stu-id="26257-133">displayName</span></span>                | <span data-ttu-id="26257-134">string</span><span class="sxs-lookup"><span data-stu-id="26257-134">string</span></span>   | <span data-ttu-id="26257-135">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="26257-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="26257-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="26257-136">distributionMethod</span></span>  | <span data-ttu-id="26257-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="26257-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="26257-138">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="26257-138">The method of distribution for the app.</span></span> <span data-ttu-id="26257-139">只读。</span><span class="sxs-lookup"><span data-stu-id="26257-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="26257-140">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="26257-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="26257-141">成员</span><span class="sxs-lookup"><span data-stu-id="26257-141">Member</span></span>|<span data-ttu-id="26257-142">值</span><span class="sxs-lookup"><span data-stu-id="26257-142">Value</span></span>|<span data-ttu-id="26257-143">说明</span><span class="sxs-lookup"><span data-stu-id="26257-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26257-144">商店</span><span class="sxs-lookup"><span data-stu-id="26257-144">store</span></span>|<span data-ttu-id="26257-145">0</span><span class="sxs-lookup"><span data-stu-id="26257-145">0</span></span>| <span data-ttu-id="26257-146">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="26257-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="26257-147">组织</span><span class="sxs-lookup"><span data-stu-id="26257-147">organization</span></span>|<span data-ttu-id="26257-148">1</span><span class="sxs-lookup"><span data-stu-id="26257-148">1</span></span>|<span data-ttu-id="26257-149">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="26257-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="26257-150">旁加载</span><span class="sxs-lookup"><span data-stu-id="26257-150">sideloaded</span></span>|<span data-ttu-id="26257-151">2</span><span class="sxs-lookup"><span data-stu-id="26257-151">2</span></span>|<span data-ttu-id="26257-152">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="26257-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26257-153">关系</span><span class="sxs-lookup"><span data-stu-id="26257-153">Relationships</span></span>

| <span data-ttu-id="26257-154">关系</span><span class="sxs-lookup"><span data-stu-id="26257-154">Relationship</span></span> | <span data-ttu-id="26257-155">类型</span><span class="sxs-lookup"><span data-stu-id="26257-155">Type</span></span>   | <span data-ttu-id="26257-156">说明</span><span class="sxs-lookup"><span data-stu-id="26257-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26257-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="26257-157">appDefinitions</span></span>|<span data-ttu-id="26257-158">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26257-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="26257-159">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26257-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26257-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26257-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="26257-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="26257-161">See also</span></span>

- [<span data-ttu-id="26257-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="26257-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="26257-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="26257-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="26257-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="26257-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


