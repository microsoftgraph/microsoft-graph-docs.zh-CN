---
title: teamsApp 资源类型
description: 应用程序中的 Microsoft 团队应用程序目录。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2f1b45f60e9586d148a08310e9d19b1a3e6c52e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912055"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="5319d-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="5319d-103">teamsApp resource type</span></span>

> <span data-ttu-id="5319d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5319d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5319d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5319d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5319d-106">应用程序中[的 Microsoft 团队](teams-api-overview.md)应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="5319d-106">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="5319d-107">用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation-add.md)方法。</span><span class="sxs-lookup"><span data-stu-id="5319d-107">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="5319d-108">方法</span><span class="sxs-lookup"><span data-stu-id="5319d-108">Methods</span></span>

| <span data-ttu-id="5319d-109">方法</span><span class="sxs-lookup"><span data-stu-id="5319d-109">Method</span></span>       | <span data-ttu-id="5319d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5319d-110">Return Type</span></span>  |<span data-ttu-id="5319d-111">说明</span><span class="sxs-lookup"><span data-stu-id="5319d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5319d-112">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="5319d-112">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="5319d-113">[teamsApp](teamsapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="5319d-113">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="5319d-114">列出来自 Microsoft 团队的应用程序目录的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="5319d-114">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="5319d-115">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="5319d-115">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="5319d-116">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5319d-116">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5319d-117">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="5319d-117">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="5319d-118">更新的已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="5319d-118">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="5319d-119">teamsApp</span><span class="sxs-lookup"><span data-stu-id="5319d-119">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="5319d-120">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="5319d-120">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="5319d-121">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="5319d-121">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="5319d-122">无</span><span class="sxs-lookup"><span data-stu-id="5319d-122">None</span></span> | <span data-ttu-id="5319d-123">从组织的应用程序目录中删除的已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5319d-123">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="5319d-124">属性</span><span class="sxs-lookup"><span data-stu-id="5319d-124">Properties</span></span>

| <span data-ttu-id="5319d-125">属性</span><span class="sxs-lookup"><span data-stu-id="5319d-125">Property</span></span>            | <span data-ttu-id="5319d-126">类型</span><span class="sxs-lookup"><span data-stu-id="5319d-126">Type</span></span>     | <span data-ttu-id="5319d-127">说明</span><span class="sxs-lookup"><span data-stu-id="5319d-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="5319d-128">ID</span><span class="sxs-lookup"><span data-stu-id="5319d-128">id</span></span>                  | <span data-ttu-id="5319d-129">string</span><span class="sxs-lookup"><span data-stu-id="5319d-129">string</span></span>   | <span data-ttu-id="5319d-130">目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="5319d-130">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5319d-131">externalId</span><span class="sxs-lookup"><span data-stu-id="5319d-131">externalId</span></span>          | <span data-ttu-id="5319d-132">string</span><span class="sxs-lookup"><span data-stu-id="5319d-132">string</span></span>   | <span data-ttu-id="5319d-133">目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="5319d-133">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5319d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5319d-134">displayName</span></span>                | <span data-ttu-id="5319d-135">string</span><span class="sxs-lookup"><span data-stu-id="5319d-135">string</span></span>   | <span data-ttu-id="5319d-136">目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="5319d-136">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="5319d-137">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="5319d-137">distributionMethod</span></span>  | <span data-ttu-id="5319d-138">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="5319d-138">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="5319d-139">应用程序分配方法。</span><span class="sxs-lookup"><span data-stu-id="5319d-139">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="5319d-140">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="5319d-140">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="5319d-141">成员</span><span class="sxs-lookup"><span data-stu-id="5319d-141">Member</span></span>|<span data-ttu-id="5319d-142">值</span><span class="sxs-lookup"><span data-stu-id="5319d-142">Value</span></span>|<span data-ttu-id="5319d-143">Description</span><span class="sxs-lookup"><span data-stu-id="5319d-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5319d-144">存储</span><span class="sxs-lookup"><span data-stu-id="5319d-144">store</span></span>|<span data-ttu-id="5319d-145">0</span><span class="sxs-lookup"><span data-stu-id="5319d-145">0</span></span>| <span data-ttu-id="5319d-146">应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。</span><span class="sxs-lookup"><span data-stu-id="5319d-146">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="5319d-147">组织</span><span class="sxs-lookup"><span data-stu-id="5319d-147">organization</span></span>|<span data-ttu-id="5319d-148">1</span><span class="sxs-lookup"><span data-stu-id="5319d-148">1</span></span>|<span data-ttu-id="5319d-149">只能在此租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="5319d-149">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="5319d-150">sideloaded</span><span class="sxs-lookup"><span data-stu-id="5319d-150">sideloaded</span></span>|<span data-ttu-id="5319d-151">2</span><span class="sxs-lookup"><span data-stu-id="5319d-151">2</span></span>|<span data-ttu-id="5319d-152">应用程序是仅供用户/工作组其安装到。</span><span class="sxs-lookup"><span data-stu-id="5319d-152">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5319d-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="5319d-153">Relationships</span></span>

| <span data-ttu-id="5319d-154">关系</span><span class="sxs-lookup"><span data-stu-id="5319d-154">Relationship</span></span> | <span data-ttu-id="5319d-155">类型</span><span class="sxs-lookup"><span data-stu-id="5319d-155">Type</span></span>   | <span data-ttu-id="5319d-156">Description</span><span class="sxs-lookup"><span data-stu-id="5319d-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5319d-157">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="5319d-157">appDefinitions</span></span>|<span data-ttu-id="5319d-158">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="5319d-158">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="5319d-159">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5319d-159">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5319d-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5319d-160">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="5319d-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5319d-161">See also</span></span>

- [<span data-ttu-id="5319d-162">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="5319d-162">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="5319d-163">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="5319d-163">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="5319d-164">teamsTab</span><span class="sxs-lookup"><span data-stu-id="5319d-164">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

