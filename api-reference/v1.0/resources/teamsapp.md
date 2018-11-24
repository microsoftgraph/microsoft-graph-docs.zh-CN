# <a name="teamsapp-resource-type"></a><span data-ttu-id="e23ae-101">teamsApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e23ae-101">teamsApp resource type</span></span>



<span data-ttu-id="e23ae-102">应用程序中[的 Microsoft 团队](teams_api_overview.md)应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e23ae-102">An app in the [Microsoft Teams](teams_api_overview.md) app catalog.</span></span>

<span data-ttu-id="e23ae-103">用户可以看到这些应用程序中 Microsoft 团队存储，并且可以将这些应用程序安装中[团队](team.md)使用[添加到团队的应用程序](../api/teamsappinstallation_add.md)方法。</span><span class="sxs-lookup"><span data-stu-id="e23ae-103">Users can see these apps in the Microsoft Teams Store, and these apps can be installed in [teams](team.md) using the [Add app to team](../api/teamsappinstallation_add.md) method.</span></span>

## <a name="methods"></a><span data-ttu-id="e23ae-104">方法</span><span class="sxs-lookup"><span data-stu-id="e23ae-104">Methods</span></span>

| <span data-ttu-id="e23ae-105">方法</span><span class="sxs-lookup"><span data-stu-id="e23ae-105">Method</span></span>       | <span data-ttu-id="e23ae-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="e23ae-106">Return Type</span></span>  |<span data-ttu-id="e23ae-107">说明</span><span class="sxs-lookup"><span data-stu-id="e23ae-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e23ae-108">列出已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="e23ae-108">List published apps</span></span>](../api/teamsapp_list.md) | <span data-ttu-id="e23ae-109">[teamsApp](teamsApp.md)集合</span><span class="sxs-lookup"><span data-stu-id="e23ae-109">[teamsApp](teamsApp.md) collection</span></span> | <span data-ttu-id="e23ae-110">列出来自 Microsoft 团队的应用程序目录的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="e23ae-110">List published apps from the Microsoft Teams apps catalog.</span></span>|
|[<span data-ttu-id="e23ae-111">发布应用程序</span><span class="sxs-lookup"><span data-stu-id="e23ae-111">Publish an app</span></span>](../api/teamsapp_publish.md) | [<span data-ttu-id="e23ae-112">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e23ae-112">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="e23ae-113">将应用程序发布到组织的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e23ae-113">Publish an app to your organization's app catalog.</span></span>|
|[<span data-ttu-id="e23ae-114">更新的已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="e23ae-114">Update a published app</span></span>](../api/teamsapp_update.md) | [<span data-ttu-id="e23ae-115">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e23ae-115">teamsApp</span></span>](teamsApp.md) | <span data-ttu-id="e23ae-116">更新组织的应用程序目录中的已发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="e23ae-116">Update a published app in your organization's app catalog.</span></span>|
|[<span data-ttu-id="e23ae-117">删除已发布的应用程序</span><span class="sxs-lookup"><span data-stu-id="e23ae-117">Remove a published app</span></span>](../api/teamsapp_delete.md) | <span data-ttu-id="e23ae-118">无</span><span class="sxs-lookup"><span data-stu-id="e23ae-118">None</span></span> | <span data-ttu-id="e23ae-119">从组织的应用程序目录中删除的已发布的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e23ae-119">Remove a published app from your organization's app catalog.</span></span>|

## <a name="properties"></a><span data-ttu-id="e23ae-120">属性</span><span class="sxs-lookup"><span data-stu-id="e23ae-120">Properties</span></span>

| <span data-ttu-id="e23ae-121">属性</span><span class="sxs-lookup"><span data-stu-id="e23ae-121">Property</span></span>            | <span data-ttu-id="e23ae-122">类型</span><span class="sxs-lookup"><span data-stu-id="e23ae-122">Type</span></span>     | <span data-ttu-id="e23ae-123">说明</span><span class="sxs-lookup"><span data-stu-id="e23ae-123">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e23ae-124">ID</span><span class="sxs-lookup"><span data-stu-id="e23ae-124">id</span></span>                  | <span data-ttu-id="e23ae-125">string</span><span class="sxs-lookup"><span data-stu-id="e23ae-125">string</span></span>   | <span data-ttu-id="e23ae-126">目录应用程序的生成应用程序 ID （不同[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中的开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="e23ae-126">The catalog app's generated app ID (different from the developer-provided ID in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e23ae-127">externalId</span><span class="sxs-lookup"><span data-stu-id="e23ae-127">externalId</span></span>          | <span data-ttu-id="e23ae-128">string</span><span class="sxs-lookup"><span data-stu-id="e23ae-128">string</span></span>   | <span data-ttu-id="e23ae-129">目录中[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)的应用程序开发人员提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="e23ae-129">The ID of the catalog provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e23ae-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e23ae-130">displayName</span></span>                | <span data-ttu-id="e23ae-131">string</span><span class="sxs-lookup"><span data-stu-id="e23ae-131">string</span></span>   | <span data-ttu-id="e23ae-132">目录应用程序[的 Microsoft 团队 zip 应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)中应用程序开发人员提供的名称。</span><span class="sxs-lookup"><span data-stu-id="e23ae-132">The name of the catalog app provided by the app developer in the [Microsoft Teams zip app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> |
| <span data-ttu-id="e23ae-133">distributionMethod</span><span class="sxs-lookup"><span data-stu-id="e23ae-133">distributionMethod</span></span>  | <span data-ttu-id="e23ae-134">teamsAppDistributionMethod</span><span class="sxs-lookup"><span data-stu-id="e23ae-134">teamsAppDistributionMethod</span></span>     | <span data-ttu-id="e23ae-135">应用程序分配方法。</span><span class="sxs-lookup"><span data-stu-id="e23ae-135">The method of distribution for the app.</span></span> |

### <a name="teamsappdistributionmethod-values"></a><span data-ttu-id="e23ae-136">teamsAppDistributionMethod 值</span><span class="sxs-lookup"><span data-stu-id="e23ae-136">teamsAppDistributionMethod values</span></span>

|<span data-ttu-id="e23ae-137">成员</span><span class="sxs-lookup"><span data-stu-id="e23ae-137">Member</span></span>|<span data-ttu-id="e23ae-138">值</span><span class="sxs-lookup"><span data-stu-id="e23ae-138">Value</span></span>|<span data-ttu-id="e23ae-139">说明</span><span class="sxs-lookup"><span data-stu-id="e23ae-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23ae-140">存储</span><span class="sxs-lookup"><span data-stu-id="e23ae-140">store</span></span>|<span data-ttu-id="e23ae-141">0</span><span class="sxs-lookup"><span data-stu-id="e23ae-141">0</span></span>| <span data-ttu-id="e23ae-142">应用程序都可以通过 Microsoft 团队应用程序商店的所有租户。</span><span class="sxs-lookup"><span data-stu-id="e23ae-142">The app is available to all tenants through the Microsoft Teams app store.</span></span>|
|<span data-ttu-id="e23ae-143">组织</span><span class="sxs-lookup"><span data-stu-id="e23ae-143">organization</span></span>|<span data-ttu-id="e23ae-144">1</span><span class="sxs-lookup"><span data-stu-id="e23ae-144">1</span></span>|<span data-ttu-id="e23ae-145">只能在此租户应用程序。</span><span class="sxs-lookup"><span data-stu-id="e23ae-145">The app is available only in this tenant.</span></span>|
|<span data-ttu-id="e23ae-146">sideloaded</span><span class="sxs-lookup"><span data-stu-id="e23ae-146">sideloaded</span></span>|<span data-ttu-id="e23ae-147">2</span><span class="sxs-lookup"><span data-stu-id="e23ae-147">2</span></span>|<span data-ttu-id="e23ae-148">应用程序是仅供用户/工作组其安装到。</span><span class="sxs-lookup"><span data-stu-id="e23ae-148">The app is available only to the user/team its installed to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e23ae-149">Relationships</span><span class="sxs-lookup"><span data-stu-id="e23ae-149">Relationships</span></span>

| <span data-ttu-id="e23ae-150">关系</span><span class="sxs-lookup"><span data-stu-id="e23ae-150">Relationship</span></span> | <span data-ttu-id="e23ae-151">类型</span><span class="sxs-lookup"><span data-stu-id="e23ae-151">Type</span></span>   | <span data-ttu-id="e23ae-152">说明</span><span class="sxs-lookup"><span data-stu-id="e23ae-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e23ae-153">appDefinitions</span><span class="sxs-lookup"><span data-stu-id="e23ae-153">appDefinitions</span></span>|<span data-ttu-id="e23ae-154">[teamsAppDefinition](teamsappdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="e23ae-154">[teamsAppDefinition](teamsappdefinition.md) collection</span></span>| <span data-ttu-id="e23ae-155">每个版本的应用程序的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e23ae-155">The details for each version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e23ae-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e23ae-156">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="e23ae-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e23ae-157">See also</span></span>

- [<span data-ttu-id="e23ae-158">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e23ae-158">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="e23ae-159">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e23ae-159">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e23ae-160">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e23ae-160">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

