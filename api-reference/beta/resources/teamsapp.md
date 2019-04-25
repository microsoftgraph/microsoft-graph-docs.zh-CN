---
title: teamsApp 资源类型
description: Microsoft 团队应用程序目录中的应用程序。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553948"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="495dd-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="495dd-103">teamsApp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="495dd-104">[Microsoft 团队](teams-api-overview.md)应用程序目录中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="495dd-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="495dd-105">用户可以在 Microsoft 团队存储中查看这些应用程序, 并且可以使用 "向[团队添加应用程序](../api/teamsappinstallation-add.md)" 方法在[团队](team.md)中安装这些应用程序。</span><span class="sxs-lookup"><span data-stu-id="495dd-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="495dd-106">方法</span><span class="sxs-lookup"><span data-stu-id="495dd-106">Methods</span></span>

| <span data-ttu-id="495dd-107">方法</span><span class="sxs-lookup"><span data-stu-id="495dd-107">Method</span></span>       | <span data-ttu-id="495dd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="495dd-108">Return Type</span></span>  |<span data-ttu-id="495dd-109">说明</span><span class="sxs-lookup"><span data-stu-id="495dd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="495dd-110">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="495dd-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="495dd-111">[teamsApp](teamsapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="495dd-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="495dd-112">列出 Microsoft 团队应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="495dd-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="495dd-113">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="495dd-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="495dd-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="495dd-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="495dd-115">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="495dd-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="495dd-116">更新已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="495dd-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="495dd-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="495dd-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="495dd-118">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="495dd-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="495dd-119">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="495dd-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="495dd-120">无</span><span class="sxs-lookup"><span data-stu-id="495dd-120">None</span></span> | <span data-ttu-id="495dd-121">从组织的应用程序目录中删除已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="495dd-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="495dd-122">属性</span><span class="sxs-lookup"><span data-stu-id="495dd-122">Properties</span></span>

| <span data-ttu-id="495dd-123">属性</span><span class="sxs-lookup"><span data-stu-id="495dd-123">Property</span></span>            | <span data-ttu-id="495dd-124">类型</span><span class="sxs-lookup"><span data-stu-id="495dd-124">Type</span></span>     | <span data-ttu-id="495dd-125">说明</span><span class="sxs-lookup"><span data-stu-id="495dd-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="495dd-126">id</span><span class="sxs-lookup"><span data-stu-id="495dd-126">id</span></span>                  | <span data-ttu-id="495dd-127">string</span><span class="sxs-lookup"><span data-stu-id="495dd-127">string</span></span>   | <span data-ttu-id="495dd-128">目录应用程序生成的应用程序 id (与[Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中开发人员提供的 id 不同。</span><span class="sxs-lookup"><span data-stu-id="495dd-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="495dd-129">externalId</span><span class="sxs-lookup"><span data-stu-id="495dd-129">externalId</span></span>          | <span data-ttu-id="495dd-130">string</span><span class="sxs-lookup"><span data-stu-id="495dd-130">string</span></span>   | <span data-ttu-id="495dd-131">[Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的应用程序开发人员提供的目录的 ID。</span><span class="sxs-lookup"><span data-stu-id="495dd-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="495dd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="495dd-132">displayName</span></span>                | <span data-ttu-id="495dd-133">string</span><span class="sxs-lookup"><span data-stu-id="495dd-133">string</span></span>   | <span data-ttu-id="495dd-134">[Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的应用程序开发人员提供的目录应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="495dd-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="495dd-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="495dd-135">distributionMethod</span></span>  | <span data-ttu-id="495dd-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="495dd-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="495dd-137">应用的分发方法。</span><span class="sxs-lookup"><span data-stu-id="495dd-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="495dd-138">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="495dd-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="495dd-139">Member</span><span class="sxs-lookup"><span data-stu-id="495dd-139">Member</span></span>|<span data-ttu-id="495dd-140">值</span><span class="sxs-lookup"><span data-stu-id="495dd-140">Value</span></span>|<span data-ttu-id="495dd-141">说明</span><span class="sxs-lookup"><span data-stu-id="495dd-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="495dd-142">microsoft</span><span class="sxs-lookup"><span data-stu-id="495dd-142">store</span></span>|<span data-ttu-id="495dd-143">0</span><span class="sxs-lookup"><span data-stu-id="495dd-143">0</span></span>| <span data-ttu-id="495dd-144">该应用程序可通过 Microsoft 团队应用商店对所有租户可用。</span><span class="sxs-lookup"><span data-stu-id="495dd-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="495dd-145">组织</span><span class="sxs-lookup"><span data-stu-id="495dd-145">organization</span></span>|<span data-ttu-id="495dd-146">1</span><span class="sxs-lookup"><span data-stu-id="495dd-146">1</span></span>|<span data-ttu-id="495dd-147">该应用程序仅在此租户中可用。</span><span class="sxs-lookup"><span data-stu-id="495dd-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="495dd-148">旁加载</span><span class="sxs-lookup"><span data-stu-id="495dd-148">sideloaded</span></span>|<span data-ttu-id="495dd-149">2 </span><span class="sxs-lookup"><span data-stu-id="495dd-149">2</span></span>|<span data-ttu-id="495dd-150">该应用程序仅适用于其安装到的用户/团队。</span><span class="sxs-lookup"><span data-stu-id="495dd-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="495dd-151">关系</span><span class="sxs-lookup"><span data-stu-id="495dd-151">Relationships</span></span>

| <span data-ttu-id="495dd-152">关系</span><span class="sxs-lookup"><span data-stu-id="495dd-152">Relationship</span></span> | <span data-ttu-id="495dd-153">类型</span><span class="sxs-lookup"><span data-stu-id="495dd-153">Type</span></span>   | <span data-ttu-id="495dd-154">说明</span><span class="sxs-lookup"><span data-stu-id="495dd-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="495dd-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="495dd-155">appDefinitions</span></span>|<span data-ttu-id="495dd-156">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="495dd-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="495dd-157">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="495dd-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="495dd-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="495dd-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="495dd-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="495dd-159">See also</span></span>

- [<span data-ttu-id="495dd-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="495dd-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="495dd-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="495dd-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="495dd-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="495dd-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

