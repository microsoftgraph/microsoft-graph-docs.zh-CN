---
title: teamsApp 资源类型
description: Microsoft Teams 应用对话框中的应用。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a7cae3ba43915f8dd024e3a9260876adb3ac2a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533509"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="bc96b-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc96b-103">teamsApp resource type</span></span>

<span data-ttu-id="bc96b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc96b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="bc96b-105">[Microsoft Teams](teams-api-overview.md) 应用对话框中的应用。</span><span class="sxs-lookup"><span data-stu-id="bc96b-105">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="bc96b-106">用户可以在 Microsoft Teams 商店中看到这些应用，并且可以使用“[向团队添加应用](../api/teamsappinstallation-add.md)”方法将这些应用安装到 [Teams](team.md) 中。</span><span class="sxs-lookup"><span data-stu-id="bc96b-106">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="bc96b-107">方法</span><span class="sxs-lookup"><span data-stu-id="bc96b-107">Methods</span></span>

| <span data-ttu-id="bc96b-108">方法</span><span class="sxs-lookup"><span data-stu-id="bc96b-108">Method</span></span>       | <span data-ttu-id="bc96b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc96b-109">Return Type</span></span>  |<span data-ttu-id="bc96b-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc96b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc96b-111">列出已发布的应用</span><span class="sxs-lookup"><span data-stu-id="bc96b-111">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="bc96b-112">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc96b-112">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="bc96b-113">列出 Microsoft Teams 应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="bc96b-113">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="bc96b-114">发布应用</span><span class="sxs-lookup"><span data-stu-id="bc96b-114">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="bc96b-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bc96b-115">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="bc96b-116">将应用发布到组织的应用目录。</span><span class="sxs-lookup"><span data-stu-id="bc96b-116">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="bc96b-117">更新已发布的应用</span><span class="sxs-lookup"><span data-stu-id="bc96b-117">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="bc96b-118">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bc96b-118">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="bc96b-119">更新组织应用目录中的已发布应用。</span><span class="sxs-lookup"><span data-stu-id="bc96b-119">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="bc96b-120">删除已发布的应用</span><span class="sxs-lookup"><span data-stu-id="bc96b-120">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="bc96b-121">无</span><span class="sxs-lookup"><span data-stu-id="bc96b-121">None</span></span> | <span data-ttu-id="bc96b-122">更新组织应用目录中已发布的应用。</span><span class="sxs-lookup"><span data-stu-id="bc96b-122">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc96b-123">属性</span><span class="sxs-lookup"><span data-stu-id="bc96b-123">Properties</span></span>

| <span data-ttu-id="bc96b-124">属性</span><span class="sxs-lookup"><span data-stu-id="bc96b-124">Property</span></span>            | <span data-ttu-id="bc96b-125">类型</span><span class="sxs-lookup"><span data-stu-id="bc96b-125">Type</span></span>     | <span data-ttu-id="bc96b-126">说明</span><span class="sxs-lookup"><span data-stu-id="bc96b-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="bc96b-127">id</span><span class="sxs-lookup"><span data-stu-id="bc96b-127">id</span></span>                  | <span data-ttu-id="bc96b-128">string</span><span class="sxs-lookup"><span data-stu-id="bc96b-128">string</span></span>   | <span data-ttu-id="bc96b-129">目录应用生成的应用 ID（不同于开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的 ID）。</span><span class="sxs-lookup"><span data-stu-id="bc96b-129">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bc96b-130">externalId</span><span class="sxs-lookup"><span data-stu-id="bc96b-130">externalId</span></span>          | <span data-ttu-id="bc96b-131">string</span><span class="sxs-lookup"><span data-stu-id="bc96b-131">string</span></span>   | <span data-ttu-id="bc96b-132">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录 ID。</span><span class="sxs-lookup"><span data-stu-id="bc96b-132">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bc96b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bc96b-133">displayName</span></span>                | <span data-ttu-id="bc96b-134">string</span><span class="sxs-lookup"><span data-stu-id="bc96b-134">string</span></span>   | <span data-ttu-id="bc96b-135">应用开发人员在 [Microsoft Teams 应用压缩包](/microsoftteams/platform/concepts/apps/apps-package)中提供的目录名称。</span><span class="sxs-lookup"><span data-stu-id="bc96b-135">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="bc96b-136">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="bc96b-136">distributionMethod</span></span>  | <span data-ttu-id="bc96b-137">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="bc96b-137">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="bc96b-138">应用的分配方法。</span><span class="sxs-lookup"><span data-stu-id="bc96b-138">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="bc96b-139">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="bc96b-139">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="bc96b-140">成员</span><span class="sxs-lookup"><span data-stu-id="bc96b-140">Member</span></span>|<span data-ttu-id="bc96b-141">值</span><span class="sxs-lookup"><span data-stu-id="bc96b-141">Value</span></span>|<span data-ttu-id="bc96b-142">说明</span><span class="sxs-lookup"><span data-stu-id="bc96b-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc96b-143">商店</span><span class="sxs-lookup"><span data-stu-id="bc96b-143">store</span></span>|<span data-ttu-id="bc96b-144">0</span><span class="sxs-lookup"><span data-stu-id="bc96b-144">0</span></span>| <span data-ttu-id="bc96b-145">应用适用于 Microsoft Teams 应用商店中的所有租户。</span><span class="sxs-lookup"><span data-stu-id="bc96b-145">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="bc96b-146">组织</span><span class="sxs-lookup"><span data-stu-id="bc96b-146">organization</span></span>|<span data-ttu-id="bc96b-147">1</span><span class="sxs-lookup"><span data-stu-id="bc96b-147">1</span></span>|<span data-ttu-id="bc96b-148">应用仅适用于此租户。</span><span class="sxs-lookup"><span data-stu-id="bc96b-148">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="bc96b-149">旁加载</span><span class="sxs-lookup"><span data-stu-id="bc96b-149">sideloaded</span></span>|<span data-ttu-id="bc96b-150">2</span><span class="sxs-lookup"><span data-stu-id="bc96b-150">2</span></span>|<span data-ttu-id="bc96b-151">应用仅适用于安装它的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="bc96b-151">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc96b-152">关系</span><span class="sxs-lookup"><span data-stu-id="bc96b-152">Relationships</span></span>

| <span data-ttu-id="bc96b-153">关系</span><span class="sxs-lookup"><span data-stu-id="bc96b-153">Relationship</span></span> | <span data-ttu-id="bc96b-154">类型</span><span class="sxs-lookup"><span data-stu-id="bc96b-154">Type</span></span>   | <span data-ttu-id="bc96b-155">说明</span><span class="sxs-lookup"><span data-stu-id="bc96b-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bc96b-156">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="bc96b-156">appDefinitions</span></span>|<span data-ttu-id="bc96b-157">[teamsAppDefinition](teamsappdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bc96b-157">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="bc96b-158">每个版本的应用的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bc96b-158">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc96b-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc96b-159">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bc96b-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bc96b-160">See also</span></span>

- [<span data-ttu-id="bc96b-161">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bc96b-161">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="bc96b-162">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="bc96b-162">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="bc96b-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bc96b-163">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

