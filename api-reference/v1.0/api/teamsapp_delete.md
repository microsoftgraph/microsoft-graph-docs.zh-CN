# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="13d4c-101">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="13d4c-101">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="13d4c-102">从组织的应用程序目录 （租户应用程序目录） 中删除[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="13d4c-102">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="13d4c-103">若要从您的组织的应用程序目录中删除您的应用程序，请指定`organization`作为**distributionMethod** [teamsCatalogApp](../resources/teamsapp.md)资源中。</span><span class="sxs-lookup"><span data-stu-id="13d4c-103">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="13d4c-104">权限</span><span class="sxs-lookup"><span data-stu-id="13d4c-104">Permissions</span></span>

<span data-ttu-id="13d4c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="13d4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="13d4c-107">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="13d4c-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="13d4c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="13d4c-108">Permission Type</span></span>                        | <span data-ttu-id="13d4c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13d4c-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="13d4c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13d4c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="13d4c-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13d4c-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="13d4c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13d4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13d4c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="13d4c-113">Not supported</span></span>|
| <span data-ttu-id="13d4c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="13d4c-114">Application</span></span>                            | <span data-ttu-id="13d4c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="13d4c-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="13d4c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13d4c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="13d4c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="13d4c-117">Request headers</span></span>

| <span data-ttu-id="13d4c-118">标头</span><span class="sxs-lookup"><span data-stu-id="13d4c-118">Header</span></span>        | <span data-ttu-id="13d4c-119">值</span><span class="sxs-lookup"><span data-stu-id="13d4c-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="13d4c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="13d4c-120">Authorization</span></span> | <span data-ttu-id="13d4c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13d4c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13d4c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="13d4c-123">Request body</span></span>

<span data-ttu-id="13d4c-124">无。</span><span class="sxs-lookup"><span data-stu-id="13d4c-124">None.</span></span>

><span data-ttu-id="13d4c-125">**注意：** 使用从[列表发布应用程序](./teamsapp_list.md)的调用返回引用您想要更新的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="13d4c-125">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="13d4c-126">不要使用 zip 应用程序包的清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="13d4c-126">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="13d4c-127">响应</span><span class="sxs-lookup"><span data-stu-id="13d4c-127">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="13d4c-128">示例</span><span class="sxs-lookup"><span data-stu-id="13d4c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="13d4c-129">请求</span><span class="sxs-lookup"><span data-stu-id="13d4c-129">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="13d4c-130">响应</span><span class="sxs-lookup"><span data-stu-id="13d4c-130">Response</span></span>

```http
HTTP/1.1 204 No Content
```
