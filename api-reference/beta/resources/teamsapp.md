---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2686bddad3c70e60c764647d5bef453fd7524462
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345762"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="eee67-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="eee67-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee67-104">[Microsoft Teams](teams-api-overview.md) 应用对话框中的应用。</span><span class="sxs-lookup"><span data-stu-id="eee67-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="eee67-105">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/teamsappinstallation-add.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="eee67-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="eee67-106">方法</span><span class="sxs-lookup"><span data-stu-id="eee67-106">Methods</span></span>

| <span data-ttu-id="eee67-107">方法</span><span class="sxs-lookup"><span data-stu-id="eee67-107">Method</span></span>       | <span data-ttu-id="eee67-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eee67-108">Return Type</span></span>  |<span data-ttu-id="eee67-109">说明</span><span class="sxs-lookup"><span data-stu-id="eee67-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eee67-110">列出已发布的应用</span><span class="sxs-lookup"><span data-stu-id="eee67-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="eee67-111">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eee67-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="eee67-112">列出 Microsoft Teams 应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="eee67-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="eee67-113">发布应用</span><span class="sxs-lookup"><span data-stu-id="eee67-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="eee67-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eee67-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="eee67-115">将应用发布到组织的应用目录。</span><span class="sxs-lookup"><span data-stu-id="eee67-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="eee67-116">更新已发布的应用</span><span class="sxs-lookup"><span data-stu-id="eee67-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="eee67-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eee67-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="eee67-118">更新组织应用目录中的已发布应用。</span><span class="sxs-lookup"><span data-stu-id="eee67-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="eee67-119">删除已发布的应用</span><span class="sxs-lookup"><span data-stu-id="eee67-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="eee67-120">无</span><span class="sxs-lookup"><span data-stu-id="eee67-120">None</span></span> | <span data-ttu-id="eee67-121">更新组织应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="eee67-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="eee67-122">属性</span><span class="sxs-lookup"><span data-stu-id="eee67-122">Properties</span></span>

| <span data-ttu-id="eee67-123">属性</span><span class="sxs-lookup"><span data-stu-id="eee67-123">Property</span></span>            | <span data-ttu-id="eee67-124">类型</span><span class="sxs-lookup"><span data-stu-id="eee67-124">Type</span></span>     | <span data-ttu-id="eee67-125">说明</span><span class="sxs-lookup"><span data-stu-id="eee67-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="eee67-126">id</span><span class="sxs-lookup"><span data-stu-id="eee67-126">id</span></span>                  | <span data-ttu-id="eee67-127">string</span><span class="sxs-lookup"><span data-stu-id="eee67-127">string</span></span>   | <span data-ttu-id="eee67-128">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="eee67-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eee67-129">externalId</span><span class="sxs-lookup"><span data-stu-id="eee67-129">externalId</span></span>          | <span data-ttu-id="eee67-130">string</span><span class="sxs-lookup"><span data-stu-id="eee67-130">string</span></span>   | <span data-ttu-id="eee67-131">应用开发人员在 [Microsoft Teams 应用压缩包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="eee67-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eee67-132">displayName</span><span class="sxs-lookup"><span data-stu-id="eee67-132">displayName</span></span>                | <span data-ttu-id="eee67-133">string</span><span class="sxs-lookup"><span data-stu-id="eee67-133">string</span></span>   | <span data-ttu-id="eee67-134">应用开发人员在 [Microsoft Teams 应用压缩包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="eee67-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="eee67-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="eee67-135">distributionMethod</span></span>  | <span data-ttu-id="eee67-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="eee67-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="eee67-137">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="eee67-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="eee67-138">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="eee67-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="eee67-139">成员</span><span class="sxs-lookup"><span data-stu-id="eee67-139">Member</span></span>|<span data-ttu-id="eee67-140">值</span><span class="sxs-lookup"><span data-stu-id="eee67-140">Value</span></span>|<span data-ttu-id="eee67-141">说明</span><span class="sxs-lookup"><span data-stu-id="eee67-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee67-142">商店</span><span class="sxs-lookup"><span data-stu-id="eee67-142">store</span></span>|<span data-ttu-id="eee67-143">0</span><span class="sxs-lookup"><span data-stu-id="eee67-143">0</span></span>| <span data-ttu-id="eee67-144">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="eee67-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="eee67-145">组织</span><span class="sxs-lookup"><span data-stu-id="eee67-145">organization</span></span>|<span data-ttu-id="eee67-146">1</span><span class="sxs-lookup"><span data-stu-id="eee67-146">1</span></span>|<span data-ttu-id="eee67-147">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="eee67-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="eee67-148">旁加载</span><span class="sxs-lookup"><span data-stu-id="eee67-148">sideloaded</span></span>|<span data-ttu-id="eee67-149">2</span><span class="sxs-lookup"><span data-stu-id="eee67-149">2</span></span>|<span data-ttu-id="eee67-150">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="eee67-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eee67-151">关系</span><span class="sxs-lookup"><span data-stu-id="eee67-151">Relationships</span></span>

| <span data-ttu-id="eee67-152">关系</span><span class="sxs-lookup"><span data-stu-id="eee67-152">Relationship</span></span> | <span data-ttu-id="eee67-153">类型</span><span class="sxs-lookup"><span data-stu-id="eee67-153">Type</span></span>   | <span data-ttu-id="eee67-154">说明</span><span class="sxs-lookup"><span data-stu-id="eee67-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eee67-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="eee67-155">appDefinitions</span></span>|<span data-ttu-id="eee67-156">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eee67-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="eee67-157">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="eee67-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eee67-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eee67-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a><span data-ttu-id="eee67-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eee67-159">See also</span></span>

- [<span data-ttu-id="eee67-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="eee67-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="eee67-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="eee67-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="eee67-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eee67-162">teamsTab</span></span>](../resources/teamstab.md)

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

