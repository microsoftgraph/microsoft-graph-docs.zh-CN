---
title: teamsApp 资源类型
description: 应用程序中的 Microsoft 团队应用程序目录。
ms.openlocfilehash: f8a96355c572287fc8bacc48f9a72e5da8d0f380
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010153"
---
# <a name="teamsapp-resource-type"></a><span data-ttu-id="0728e-103">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="0728e-103">teamsApp resource type</span></span>



<span data-ttu-id="0728e-104">应用程序中[的 Microsoft 团队](teams-api-overview.md)应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="0728e-104">An app in the [Microsoft Teams](teams-api-overview.md) app catalog.</span></span>

<span data-ttu-id="0728e-105">用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation-add.md)方法。</span><span class="sxs-lookup"><span data-stu-id="0728e-105">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation-add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="0728e-106">方法</span><span class="sxs-lookup"><span data-stu-id="0728e-106">Methods</span></span>

| <span data-ttu-id="0728e-107">方法</span><span class="sxs-lookup"><span data-stu-id="0728e-107">Method</span></span>       | <span data-ttu-id="0728e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0728e-108">Return Type</span></span>  |<span data-ttu-id="0728e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0728e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0728e-110">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="0728e-110">List published apps</span></span>](../api/teamsapp-list.md) | <span data-ttu-id="0728e-111">[teamsApp](teamsapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="0728e-111">[teamsApp](teamsapp.md) collection</span></span> | <span data-ttu-id="0728e-112">列出来自 Microsoft 团队的应用程序目录的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="0728e-112">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="0728e-113">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="0728e-113">Publish an app</span></span>](../api/teamsapp-publish.md) | [<span data-ttu-id="0728e-114">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0728e-114">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0728e-115">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="0728e-115">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="0728e-116">更新的已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="0728e-116">Update a published app</span></span>](../api/teamsapp-update.md) | [<span data-ttu-id="0728e-117">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0728e-117">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0728e-118">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="0728e-118">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="0728e-119">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="0728e-119">Remove a published app</span></span>](../api/teamsapp-delete.md) | <span data-ttu-id="0728e-120">无</span><span class="sxs-lookup"><span data-stu-id="0728e-120">None</span></span> | <span data-ttu-id="0728e-121">从组织的应用程序目录中删除的已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0728e-121">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="0728e-122">属性</span><span class="sxs-lookup"><span data-stu-id="0728e-122">Properties</span></span>

| <span data-ttu-id="0728e-123">属性</span><span class="sxs-lookup"><span data-stu-id="0728e-123">Property</span></span>            | <span data-ttu-id="0728e-124">类型</span><span class="sxs-lookup"><span data-stu-id="0728e-124">Type</span></span>     | <span data-ttu-id="0728e-125">说明</span><span class="sxs-lookup"><span data-stu-id="0728e-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="0728e-126">ID</span><span class="sxs-lookup"><span data-stu-id="0728e-126">id</span></span>                  | <span data-ttu-id="0728e-127">string</span><span class="sxs-lookup"><span data-stu-id="0728e-127">string</span></span>   | <span data-ttu-id="0728e-128">目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="0728e-128">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0728e-129">externalId</span><span class="sxs-lookup"><span data-stu-id="0728e-129">externalId</span></span>          | <span data-ttu-id="0728e-130">string</span><span class="sxs-lookup"><span data-stu-id="0728e-130">string</span></span>   | <span data-ttu-id="0728e-131">目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="0728e-131">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0728e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0728e-132">displayName</span></span>                | <span data-ttu-id="0728e-133">string</span><span class="sxs-lookup"><span data-stu-id="0728e-133">string</span></span>   | <span data-ttu-id="0728e-134">目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="0728e-134">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="0728e-135">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="0728e-135">distributionMethod</span></span>  | <span data-ttu-id="0728e-136">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="0728e-136">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="0728e-137">应用程序分配方法。</span><span class="sxs-lookup"><span data-stu-id="0728e-137">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="0728e-138">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="0728e-138">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="0728e-139">成员</span><span class="sxs-lookup"><span data-stu-id="0728e-139">Member</span></span>|<span data-ttu-id="0728e-140">值</span><span class="sxs-lookup"><span data-stu-id="0728e-140">Value</span></span>|<span data-ttu-id="0728e-141">说明</span><span class="sxs-lookup"><span data-stu-id="0728e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0728e-142">存储</span><span class="sxs-lookup"><span data-stu-id="0728e-142">store</span></span>|<span data-ttu-id="0728e-143">0</span><span class="sxs-lookup"><span data-stu-id="0728e-143">0</span></span>| <span data-ttu-id="0728e-144">应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。</span><span class="sxs-lookup"><span data-stu-id="0728e-144">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="0728e-145">组织</span><span class="sxs-lookup"><span data-stu-id="0728e-145">organization</span></span>|<span data-ttu-id="0728e-146">1</span><span class="sxs-lookup"><span data-stu-id="0728e-146">1</span></span>|<span data-ttu-id="0728e-147">只能在此租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="0728e-147">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="0728e-148">sideloaded</span><span class="sxs-lookup"><span data-stu-id="0728e-148">sideloaded</span></span>|<span data-ttu-id="0728e-149">2</span><span class="sxs-lookup"><span data-stu-id="0728e-149">2</span></span>|<span data-ttu-id="0728e-150">应用程序是仅供用户/工作组其安装到。</span><span class="sxs-lookup"><span data-stu-id="0728e-150">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0728e-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="0728e-151">Relationships</span></span>

| <span data-ttu-id="0728e-152">关系</span><span class="sxs-lookup"><span data-stu-id="0728e-152">Relationship</span></span> | <span data-ttu-id="0728e-153">类型</span><span class="sxs-lookup"><span data-stu-id="0728e-153">Type</span></span>   | <span data-ttu-id="0728e-154">说明</span><span class="sxs-lookup"><span data-stu-id="0728e-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0728e-155">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="0728e-155">appDefinitions</span></span>|<span data-ttu-id="0728e-156">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="0728e-156">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="0728e-157">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0728e-157">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0728e-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0728e-158">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="0728e-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0728e-159">See also</span></span>

- [<span data-ttu-id="0728e-160">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="0728e-160">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="0728e-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="0728e-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="0728e-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0728e-162">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

