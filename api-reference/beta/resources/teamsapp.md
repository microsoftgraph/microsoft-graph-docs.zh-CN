---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a890cea9763bd8615495d4d9597601a508fafc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046599"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="08547-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="08547-103">teamsApp resource type</span></span>

<span data-ttu-id="08547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08547-105">代表[Microsoft Teams](teams-api-overview.md) 应用目录中的一个应用.</span><span class="sxs-lookup"><span data-stu-id="08547-105">Represents an app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="08547-106">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/teamsappinstallation-add.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="08547-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="08547-107">方法</span><span class="sxs-lookup"><span data-stu-id="08547-107">Methods</span></span>

| <span data-ttu-id="08547-108">方法</span><span class="sxs-lookup"><span data-stu-id="08547-108">Method</span></span>       | <span data-ttu-id="08547-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="08547-109">Return Type</span></span>  |<span data-ttu-id="08547-110">说明</span><span class="sxs-lookup"><span data-stu-id="08547-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08547-111">列出已发布的应用</span><span class="sxs-lookup"><span data-stu-id="08547-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="08547-112">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08547-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="08547-113">列出 Microsoft Teams 应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="08547-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="08547-114">发布应用</span><span class="sxs-lookup"><span data-stu-id="08547-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="08547-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="08547-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="08547-116">将应用发布到组织的应用目录。</span><span class="sxs-lookup"><span data-stu-id="08547-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="08547-117">更新已发布的应用</span><span class="sxs-lookup"><span data-stu-id="08547-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="08547-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="08547-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="08547-119">更新组织应用目录中的已发布应用。</span><span class="sxs-lookup"><span data-stu-id="08547-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="08547-120">删除已发布的应用</span><span class="sxs-lookup"><span data-stu-id="08547-120">Delete a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="08547-121">无</span><span class="sxs-lookup"><span data-stu-id="08547-121">None</span></span> | <span data-ttu-id="08547-122">更新组织应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="08547-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="08547-123">属性</span><span class="sxs-lookup"><span data-stu-id="08547-123">Properties</span></span>

| <span data-ttu-id="08547-124">属性</span><span class="sxs-lookup"><span data-stu-id="08547-124">Property</span></span>            | <span data-ttu-id="08547-125">类型</span><span class="sxs-lookup"><span data-stu-id="08547-125">Type</span></span>     | <span data-ttu-id="08547-126">说明</span><span class="sxs-lookup"><span data-stu-id="08547-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="08547-127">id</span><span class="sxs-lookup"><span data-stu-id="08547-127">id</span></span>                  | <span data-ttu-id="08547-128">string</span><span class="sxs-lookup"><span data-stu-id="08547-128">string</span></span>   | <span data-ttu-id="08547-129">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="08547-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="08547-130">externalId</span><span class="sxs-lookup"><span data-stu-id="08547-130">externalId</span></span>          | <span data-ttu-id="08547-131">string</span><span class="sxs-lookup"><span data-stu-id="08547-131">string</span></span>   | <span data-ttu-id="08547-132">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="08547-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="08547-133">displayName</span><span class="sxs-lookup"><span data-stu-id="08547-133">displayName</span></span>                | <span data-ttu-id="08547-134">string</span><span class="sxs-lookup"><span data-stu-id="08547-134">string</span></span>   | <span data-ttu-id="08547-135">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="08547-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="08547-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="08547-136">distributionMethod</span></span>  | <span data-ttu-id="08547-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="08547-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="08547-138">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="08547-138">The method of distribution for the app.</span></span> <span data-ttu-id="08547-139">只读。</span><span class="sxs-lookup"><span data-stu-id="08547-139">Read-only.</span></span>|

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="08547-140">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="08547-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="08547-141">成员</span><span class="sxs-lookup"><span data-stu-id="08547-141">Member</span></span>|<span data-ttu-id="08547-142">值</span><span class="sxs-lookup"><span data-stu-id="08547-142">Value</span></span>|<span data-ttu-id="08547-143">说明</span><span class="sxs-lookup"><span data-stu-id="08547-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08547-144">商店</span><span class="sxs-lookup"><span data-stu-id="08547-144">store</span></span>|<span data-ttu-id="08547-145">0</span><span class="sxs-lookup"><span data-stu-id="08547-145">0</span></span>| <span data-ttu-id="08547-146">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="08547-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="08547-147">组织</span><span class="sxs-lookup"><span data-stu-id="08547-147">organization</span></span>|<span data-ttu-id="08547-148">1</span><span class="sxs-lookup"><span data-stu-id="08547-148">1</span></span>|<span data-ttu-id="08547-149">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="08547-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="08547-150">旁加载</span><span class="sxs-lookup"><span data-stu-id="08547-150">sideloaded</span></span>|<span data-ttu-id="08547-151">2</span><span class="sxs-lookup"><span data-stu-id="08547-151">2</span></span>|<span data-ttu-id="08547-152">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="08547-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08547-153">关系</span><span class="sxs-lookup"><span data-stu-id="08547-153">Relationships</span></span>

| <span data-ttu-id="08547-154">关系</span><span class="sxs-lookup"><span data-stu-id="08547-154">Relationship</span></span> | <span data-ttu-id="08547-155">类型</span><span class="sxs-lookup"><span data-stu-id="08547-155">Type</span></span>   | <span data-ttu-id="08547-156">说明</span><span class="sxs-lookup"><span data-stu-id="08547-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="08547-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="08547-157">appDefinitions</span></span>|<span data-ttu-id="08547-158">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="08547-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="08547-159">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="08547-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08547-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08547-160">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="08547-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="08547-161">See also</span></span>

- [<span data-ttu-id="08547-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="08547-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="08547-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="08547-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="08547-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="08547-164">teamsTab</span></span>](../resources/teamstab.md)

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



