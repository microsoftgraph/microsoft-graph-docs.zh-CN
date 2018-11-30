---
title: teamsApp 资源类型
description: 应用程序中的 Microsoft 团队应用程序目录。
ms.openlocfilehash: bb9081306cbcc5d8537c86e7f3f59afff89a03b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044479"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="b67ba-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-103">teamsApp resource type</span></span>

> <span data-ttu-id="b67ba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b67ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b67ba-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b67ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b67ba-106">应用程序中[的 Microsoft 团队](teams-api-overview.md)应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="b67ba-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="b67ba-107">用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation-add.md)方法。</span><span class="sxs-lookup"><span data-stu-id="b67ba-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="b67ba-108">方法</span><span class="sxs-lookup"><span data-stu-id="b67ba-108">Methods</span></span>

| <span data-ttu-id="b67ba-109">方法</span><span class="sxs-lookup"><span data-stu-id="b67ba-109">Method</span></span>       | <span data-ttu-id="b67ba-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-110">Return Type</span></span>  |<span data-ttu-id="b67ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b67ba-112">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="b67ba-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="b67ba-113">[teamsApp](teamsapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="b67ba-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="b67ba-114">列出来自 Microsoft 团队的应用程序目录的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="b67ba-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="b67ba-115">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="b67ba-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="b67ba-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b67ba-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b67ba-117">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="b67ba-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="b67ba-118">更新的已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="b67ba-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="b67ba-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b67ba-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="b67ba-120">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="b67ba-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="b67ba-121">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="b67ba-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="b67ba-122">无</span><span class="sxs-lookup"><span data-stu-id="b67ba-122">None</span></span> | <span data-ttu-id="b67ba-123">从组织的应用程序目录中删除的已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b67ba-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="b67ba-124">属性</span><span class="sxs-lookup"><span data-stu-id="b67ba-124">Properties</span></span>

| <span data-ttu-id="b67ba-125">属性</span><span class="sxs-lookup"><span data-stu-id="b67ba-125">Property</span></span>            | <span data-ttu-id="b67ba-126">类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-126">Type</span></span>     | <span data-ttu-id="b67ba-127">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b67ba-128">ID</span><span class="sxs-lookup"><span data-stu-id="b67ba-128">id</span></span>                  | <span data-ttu-id="b67ba-129">string</span><span class="sxs-lookup"><span data-stu-id="b67ba-129">string</span></span>   | <span data-ttu-id="b67ba-130">目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="b67ba-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b67ba-131">externalId</span><span class="sxs-lookup"><span data-stu-id="b67ba-131">externalId</span></span>          | <span data-ttu-id="b67ba-132">string</span><span class="sxs-lookup"><span data-stu-id="b67ba-132">string</span></span>   | <span data-ttu-id="b67ba-133">目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="b67ba-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b67ba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b67ba-134">displayName</span></span>                | <span data-ttu-id="b67ba-135">string</span><span class="sxs-lookup"><span data-stu-id="b67ba-135">string</span></span>   | <span data-ttu-id="b67ba-136">目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="b67ba-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="b67ba-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="b67ba-137">distributionMethod</span></span>  | <span data-ttu-id="b67ba-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="b67ba-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="b67ba-139">应用程序分配方法。</span><span class="sxs-lookup"><span data-stu-id="b67ba-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="b67ba-140">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="b67ba-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="b67ba-141">成员</span><span class="sxs-lookup"><span data-stu-id="b67ba-141">Member</span></span>|<span data-ttu-id="b67ba-142">值</span><span class="sxs-lookup"><span data-stu-id="b67ba-142">Value</span></span>|<span data-ttu-id="b67ba-143">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67ba-144">存储</span><span class="sxs-lookup"><span data-stu-id="b67ba-144">store</span></span>|<span data-ttu-id="b67ba-145">0</span><span class="sxs-lookup"><span data-stu-id="b67ba-145">0</span></span>| <span data-ttu-id="b67ba-146">应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。</span><span class="sxs-lookup"><span data-stu-id="b67ba-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="b67ba-147">组织</span><span class="sxs-lookup"><span data-stu-id="b67ba-147">organization</span></span>|<span data-ttu-id="b67ba-148">1</span><span class="sxs-lookup"><span data-stu-id="b67ba-148">1</span></span>|<span data-ttu-id="b67ba-149">只能在此租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="b67ba-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="b67ba-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="b67ba-150">sideloaded</span></span>|<span data-ttu-id="b67ba-151">2</span><span class="sxs-lookup"><span data-stu-id="b67ba-151">2</span></span>|<span data-ttu-id="b67ba-152">应用程序是仅供用户/工作组其安装到。</span><span class="sxs-lookup"><span data-stu-id="b67ba-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b67ba-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="b67ba-153">Relationships</span></span>

| <span data-ttu-id="b67ba-154">关系</span><span class="sxs-lookup"><span data-stu-id="b67ba-154">Relationship</span></span> | <span data-ttu-id="b67ba-155">类型</span><span class="sxs-lookup"><span data-stu-id="b67ba-155">Type</span></span>   | <span data-ttu-id="b67ba-156">说明</span><span class="sxs-lookup"><span data-stu-id="b67ba-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b67ba-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="b67ba-157">appDefinitions</span></span>|<span data-ttu-id="b67ba-158">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="b67ba-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="b67ba-159">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b67ba-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b67ba-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b67ba-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="b67ba-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b67ba-161">See also</span></span>

- [<span data-ttu-id="b67ba-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b67ba-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="b67ba-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b67ba-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="b67ba-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b67ba-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

