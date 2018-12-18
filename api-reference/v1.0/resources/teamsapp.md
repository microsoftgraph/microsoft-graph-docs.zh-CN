---
title: teamsApp 资源类型
description: 应用程序中的 Microsoft 团队应用程序目录。
author: nkramer
ms.openlocfilehash: 207974800e44e0db29b8c42f260a1ac16a18902f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359582"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="d3f3a-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3f3a-103">teamsApp resource type</span></span>



<span data-ttu-id="d3f3a-104">应用程序中[的 Microsoft 团队](teams-api-overview.md)应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="d3f3a-105">用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation-add.md)方法。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="d3f3a-106">方法</span><span class="sxs-lookup"><span data-stu-id="d3f3a-106">Methods</span></span>

| <span data-ttu-id="d3f3a-107">方法</span><span class="sxs-lookup"><span data-stu-id="d3f3a-107">Method</span></span>       | <span data-ttu-id="d3f3a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3f3a-108">Return Type</span></span>  |<span data-ttu-id="d3f3a-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3f3a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3f3a-110">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="d3f3a-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="d3f3a-111">[teamsApp](teamsapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3f3a-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="d3f3a-112">列出来自 Microsoft 团队的应用程序目录的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="d3f3a-113">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="d3f3a-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="d3f3a-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d3f3a-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d3f3a-115">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="d3f3a-116">更新的已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="d3f3a-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="d3f3a-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d3f3a-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="d3f3a-118">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="d3f3a-119">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="d3f3a-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="d3f3a-120">无</span><span class="sxs-lookup"><span data-stu-id="d3f3a-120">None</span></span> | <span data-ttu-id="d3f3a-121">从组织的应用程序目录中删除的已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3f3a-122">属性</span><span class="sxs-lookup"><span data-stu-id="d3f3a-122">Properties</span></span>

| <span data-ttu-id="d3f3a-123">属性</span><span class="sxs-lookup"><span data-stu-id="d3f3a-123">Property</span></span>            | <span data-ttu-id="d3f3a-124">类型</span><span class="sxs-lookup"><span data-stu-id="d3f3a-124">Type</span></span>     | <span data-ttu-id="d3f3a-125">说明</span><span class="sxs-lookup"><span data-stu-id="d3f3a-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d3f3a-126">ID</span><span class="sxs-lookup"><span data-stu-id="d3f3a-126">id</span></span>                  | <span data-ttu-id="d3f3a-127">string</span><span class="sxs-lookup"><span data-stu-id="d3f3a-127">string</span></span>   | <span data-ttu-id="d3f3a-128">目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d3f3a-129">externalId</span><span class="sxs-lookup"><span data-stu-id="d3f3a-129">externalId</span></span>          | <span data-ttu-id="d3f3a-130">string</span><span class="sxs-lookup"><span data-stu-id="d3f3a-130">string</span></span>   | <span data-ttu-id="d3f3a-131">目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d3f3a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d3f3a-132">displayName</span></span>                | <span data-ttu-id="d3f3a-133">string</span><span class="sxs-lookup"><span data-stu-id="d3f3a-133">string</span></span>   | <span data-ttu-id="d3f3a-134">目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="d3f3a-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="d3f3a-135">distributionMethod</span></span>  | <span data-ttu-id="d3f3a-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="d3f3a-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="d3f3a-137">应用程序分配方法。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="d3f3a-138">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="d3f3a-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="d3f3a-139">Member</span><span class="sxs-lookup"><span data-stu-id="d3f3a-139">Member</span></span>|<span data-ttu-id="d3f3a-140">值</span><span class="sxs-lookup"><span data-stu-id="d3f3a-140">Value</span></span>|<span data-ttu-id="d3f3a-141">说明</span><span class="sxs-lookup"><span data-stu-id="d3f3a-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f3a-142">存储</span><span class="sxs-lookup"><span data-stu-id="d3f3a-142">store</span></span>|<span data-ttu-id="d3f3a-143">0</span><span class="sxs-lookup"><span data-stu-id="d3f3a-143">0</span></span>| <span data-ttu-id="d3f3a-144">应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="d3f3a-145">组织</span><span class="sxs-lookup"><span data-stu-id="d3f3a-145">organization</span></span>|<span data-ttu-id="d3f3a-146">1</span><span class="sxs-lookup"><span data-stu-id="d3f3a-146">1</span></span>|<span data-ttu-id="d3f3a-147">只能在此租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="d3f3a-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="d3f3a-148">sideloaded</span></span>|<span data-ttu-id="d3f3a-149">2</span><span class="sxs-lookup"><span data-stu-id="d3f3a-149">2</span></span>|<span data-ttu-id="d3f3a-150">应用程序是仅供用户/工作组其安装到。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3f3a-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="d3f3a-151">Relationships</span></span>

| <span data-ttu-id="d3f3a-152">关系</span><span class="sxs-lookup"><span data-stu-id="d3f3a-152">Relationship</span></span> | <span data-ttu-id="d3f3a-153">类型</span><span class="sxs-lookup"><span data-stu-id="d3f3a-153">Type</span></span>   | <span data-ttu-id="d3f3a-154">说明</span><span class="sxs-lookup"><span data-stu-id="d3f3a-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d3f3a-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="d3f3a-155">appDefinitions</span></span>|<span data-ttu-id="d3f3a-156">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3f3a-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="d3f3a-157">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d3f3a-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3f3a-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3f3a-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="d3f3a-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d3f3a-159">See also</span></span>

- [<span data-ttu-id="d3f3a-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d3f3a-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="d3f3a-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="d3f3a-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="d3f3a-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d3f3a-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

