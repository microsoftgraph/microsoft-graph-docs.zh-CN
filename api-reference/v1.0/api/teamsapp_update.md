# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="e73d9-101">更新应用程序发布到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="e73d9-101">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="e73d9-102">更新[应用程序](../resources/teamsapp.md)之前发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e73d9-102">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="e73d9-103">此 API 专门更新应用程序发布到组织的应用程序目录 （租户应用程序目录）。</span><span class="sxs-lookup"><span data-stu-id="e73d9-103">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e73d9-104">若要发布到组织的应用程序目录，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="e73d9-104">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e73d9-105">权限</span><span class="sxs-lookup"><span data-stu-id="e73d9-105">Permissions</span></span>

<span data-ttu-id="e73d9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="e73d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e73d9-108">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e73d9-108">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="e73d9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e73d9-109">Permission Type</span></span>                        | <span data-ttu-id="e73d9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e73d9-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e73d9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e73d9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e73d9-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73d9-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e73d9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e73d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73d9-114">不支持</span><span class="sxs-lookup"><span data-stu-id="e73d9-114">Not supported</span></span>|
| <span data-ttu-id="e73d9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e73d9-115">Application</span></span>                            | <span data-ttu-id="e73d9-116">不支持</span><span class="sxs-lookup"><span data-stu-id="e73d9-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e73d9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e73d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e73d9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e73d9-118">Request headers</span></span>

| <span data-ttu-id="e73d9-119">标头</span><span class="sxs-lookup"><span data-stu-id="e73d9-119">Header</span></span>        | <span data-ttu-id="e73d9-120">值</span><span class="sxs-lookup"><span data-stu-id="e73d9-120">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e73d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e73d9-121">Authorization</span></span> | <span data-ttu-id="e73d9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e73d9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e73d9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e73d9-124">Content-Type</span></span>  | <span data-ttu-id="e73d9-125">应用程序/zip</span><span class="sxs-lookup"><span data-stu-id="e73d9-125">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e73d9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e73d9-126">Request body</span></span>

<span data-ttu-id="e73d9-127">团队 Zip 清单负载： 团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e73d9-127">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="e73d9-128">**注意：** 使用从[列表发布应用程序](./teamsapp_list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="e73d9-128">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e73d9-129">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="e73d9-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e73d9-130">响应</span><span class="sxs-lookup"><span data-stu-id="e73d9-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e73d9-131">示例</span><span class="sxs-lookup"><span data-stu-id="e73d9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e73d9-132">请求</span><span class="sxs-lookup"><span data-stu-id="e73d9-132">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e73d9-133">团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e73d9-133">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="e73d9-134">响应</span><span class="sxs-lookup"><span data-stu-id="e73d9-134">Response</span></span>

```
HTTP/1.1 204 No Content
```
