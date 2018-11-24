# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="7966c-101">列表中的 Microsoft 团队应用程序目录发布应用程序</span><span class="sxs-lookup"><span data-stu-id="7966c-101">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="7966c-102">从 Microsoft 团队应用程序目录的列表[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7966c-102">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="7966c-103">这包括来自 Microsoft 团队商店的应用程序，以及来自您组织的应用程序目录 （租户应用程序目录） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7966c-103">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="7966c-104">若要从您的组织的应用程序目录获取应用程序，请指定`Organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="7966c-104">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7966c-105">权限</span><span class="sxs-lookup"><span data-stu-id="7966c-105">Permissions</span></span>

<span data-ttu-id="7966c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="7966c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7966c-108">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7966c-108">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="7966c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7966c-109">Permission Type</span></span>                        | <span data-ttu-id="7966c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7966c-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7966c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7966c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7966c-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7966c-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="7966c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7966c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7966c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7966c-114">Not supported</span></span>|
| <span data-ttu-id="7966c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7966c-115">Application</span></span>                            | <span data-ttu-id="7966c-116">不支持</span><span class="sxs-lookup"><span data-stu-id="7966c-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7966c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7966c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7966c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7966c-118">Optional query parameters</span></span>
<span data-ttu-id="7966c-119">此方法支持 $filter，$select，和 $expand [OData 查询参数](../../../concepts/query_parameters.md)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="7966c-119">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7966c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7966c-120">Request headers</span></span>

| <span data-ttu-id="7966c-121">标头</span><span class="sxs-lookup"><span data-stu-id="7966c-121">Header</span></span>        | <span data-ttu-id="7966c-122">值</span><span class="sxs-lookup"><span data-stu-id="7966c-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7966c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7966c-123">Authorization</span></span> | <span data-ttu-id="7966c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7966c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7966c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7966c-126">Request body</span></span>
<span data-ttu-id="7966c-127">无。</span><span class="sxs-lookup"><span data-stu-id="7966c-127">None.</span></span>

><span data-ttu-id="7966c-128">**注意：** 您可以在任何[teamsCatalogApp](../resources/teamsapp.md)对象，以缩短结果列表中的字段进行筛选。</span><span class="sxs-lookup"><span data-stu-id="7966c-128">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="7966c-129">您可以使用任何以下筛选器操作： 等于、 不等，或，并且没有。</span><span class="sxs-lookup"><span data-stu-id="7966c-129">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="7966c-130">响应</span><span class="sxs-lookup"><span data-stu-id="7966c-130">Response</span></span>
<span data-ttu-id="7966c-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[teamsCatalogApp](../resources/teamsapp.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7966c-131">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7966c-132">示例</span><span class="sxs-lookup"><span data-stu-id="7966c-132">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="7966c-133">示例 1</span><span class="sxs-lookup"><span data-stu-id="7966c-133">Example 1</span></span>
<span data-ttu-id="7966c-134">以下示例将列出所有特定于您的租户的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7966c-134">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="7966c-135">请求</span><span class="sxs-lookup"><span data-stu-id="7966c-135">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="7966c-136">响应</span><span class="sxs-lookup"><span data-stu-id="7966c-136">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="7966c-137">示例 2</span><span class="sxs-lookup"><span data-stu-id="7966c-137">Example 2</span></span>

<span data-ttu-id="7966c-138">以下示例将列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="7966c-138">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="7966c-139">请求</span><span class="sxs-lookup"><span data-stu-id="7966c-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="7966c-140">响应</span><span class="sxs-lookup"><span data-stu-id="7966c-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

