# <a name="publish-apps-to-your-organizations-app-catalog"></a><span data-ttu-id="e8028-101">将应用程序发布到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="e8028-101">Publish apps to your organization's app catalog</span></span>



<span data-ttu-id="e8028-102">将[应用程序](../resources/teamsapp.md)发布到 Microsoft 团队的应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="e8028-102">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span> <span data-ttu-id="e8028-103">具体而言，此 API 将应用程序发布到组织的目录 （租户应用程序目录）;创建的资源将具有`distributionMethod`  =  `organization`。</span><span class="sxs-lookup"><span data-stu-id="e8028-103">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have `distributionMethod` = `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8028-104">权限</span><span class="sxs-lookup"><span data-stu-id="e8028-104">Permissions</span></span>

<span data-ttu-id="e8028-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="e8028-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e8028-107">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="e8028-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="e8028-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8028-108">Permission Type</span></span>                        | <span data-ttu-id="e8028-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8028-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e8028-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8028-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8028-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8028-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e8028-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8028-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8028-113">不支持</span><span class="sxs-lookup"><span data-stu-id="e8028-113">Not supported</span></span>|
| <span data-ttu-id="e8028-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8028-114">Application</span></span>                            | <span data-ttu-id="e8028-115">不支持</span><span class="sxs-lookup"><span data-stu-id="e8028-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8028-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8028-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a><span data-ttu-id="e8028-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8028-117">Request headers</span></span>

| <span data-ttu-id="e8028-118">标头</span><span class="sxs-lookup"><span data-stu-id="e8028-118">Header</span></span>        | <span data-ttu-id="e8028-119">值</span><span class="sxs-lookup"><span data-stu-id="e8028-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e8028-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8028-120">Authorization</span></span> | <span data-ttu-id="e8028-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8028-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8028-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8028-123">Content-Type</span></span>  | <span data-ttu-id="e8028-124">应用程序/zip</span><span class="sxs-lookup"><span data-stu-id="e8028-124">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8028-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8028-125">Request body</span></span>

<span data-ttu-id="e8028-126">团队 Zip 清单负载。</span><span class="sxs-lookup"><span data-stu-id="e8028-126">Teams Zip Manifest Payload.</span></span> <span data-ttu-id="e8028-127">团队应用程序 zip 文件，[请参阅创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="e8028-127">For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> <span data-ttu-id="e8028-128">无法创建应用程序的组织的组织中具有相同的清单另一个应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="e8028-128">You can't create an app for an organization that has the same manifest ID as another app in that organization.</span></span>

## <a name="response"></a><span data-ttu-id="e8028-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8028-129">Response</span></span>

<span data-ttu-id="e8028-130">如果成功，此方法返回`200 OK`响应代码和[teamsCatalogApp](../resources/teamsapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8028-130">If successful, this method returns a `200 OK` response code and a [teamsCatalogApp](../resources/teamsapp.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="e8028-131">示例</span><span class="sxs-lookup"><span data-stu-id="e8028-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8028-132">请求</span><span class="sxs-lookup"><span data-stu-id="e8028-132">Request</span></span>

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e8028-133">有关如何创建的 Microsoft 团队应用程序 zip 文件的信息，请参阅[创建应用程序包](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="e8028-133">For information about how to create a Microsoft Teams application zip file, see [Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package).</span></span> 

### <a name="response"></a><span data-ttu-id="e8028-134">响应</span><span class="sxs-lookup"><span data-stu-id="e8028-134">Response</span></span>

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
