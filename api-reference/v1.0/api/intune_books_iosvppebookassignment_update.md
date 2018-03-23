# <a name="update-iosvppebookassignment"></a><span data-ttu-id="eb34e-101">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="eb34e-101">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="eb34e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb34e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb34e-103">更新 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb34e-103">Update the properties of a [calendar](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb34e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb34e-104">Prerequisites</span></span>
<span data-ttu-id="eb34e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eb34e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb34e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb34e-107">Permission type</span></span>|<span data-ttu-id="eb34e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb34e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb34e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb34e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eb34e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb34e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eb34e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb34e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb34e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb34e-112">Not supported.</span></span>|
|<span data-ttu-id="eb34e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb34e-113">Application</span></span>|<span data-ttu-id="eb34e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb34e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb34e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb34e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eb34e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb34e-116">Request headers</span></span>
|<span data-ttu-id="eb34e-117">标头</span><span class="sxs-lookup"><span data-stu-id="eb34e-117">Header</span></span>|<span data-ttu-id="eb34e-118">值</span><span class="sxs-lookup"><span data-stu-id="eb34e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb34e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb34e-119">Authorization</span></span>|<span data-ttu-id="eb34e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb34e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eb34e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="eb34e-121">Accept</span></span>|<span data-ttu-id="eb34e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eb34e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb34e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb34e-123">Request body</span></span>
<span data-ttu-id="eb34e-124">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb34e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="eb34e-125">下表显示创建 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb34e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="eb34e-126">属性</span><span class="sxs-lookup"><span data-stu-id="eb34e-126">Property</span></span>|<span data-ttu-id="eb34e-127">类型</span><span class="sxs-lookup"><span data-stu-id="eb34e-127">Type</span></span>|<span data-ttu-id="eb34e-128">说明</span><span class="sxs-lookup"><span data-stu-id="eb34e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb34e-129">id</span><span class="sxs-lookup"><span data-stu-id="eb34e-129">id</span></span>|<span data-ttu-id="eb34e-130">String</span><span class="sxs-lookup"><span data-stu-id="eb34e-130">String</span></span>|<span data-ttu-id="eb34e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eb34e-131">Key of the setting.</span></span> <span data-ttu-id="eb34e-132">继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eb34e-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="eb34e-133">target</span><span class="sxs-lookup"><span data-stu-id="eb34e-133">target</span></span>|[<span data-ttu-id="eb34e-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eb34e-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_books_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eb34e-135">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="eb34e-135">The assignment target for eBook.</span></span> <span data-ttu-id="eb34e-136">继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eb34e-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="eb34e-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="eb34e-137">installIntent</span></span>|<span data-ttu-id="eb34e-138">String</span><span class="sxs-lookup"><span data-stu-id="eb34e-138">String</span></span>|<span data-ttu-id="eb34e-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="eb34e-139">The install intent for eBook.</span></span> <span data-ttu-id="eb34e-140">继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="eb34e-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="eb34e-141">响应</span><span class="sxs-lookup"><span data-stu-id="eb34e-141">Response</span></span>
<span data-ttu-id="eb34e-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb34e-142">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb34e-143">示例</span><span class="sxs-lookup"><span data-stu-id="eb34e-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb34e-144">请求</span><span class="sxs-lookup"><span data-stu-id="eb34e-144">Request</span></span>
<span data-ttu-id="eb34e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb34e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="eb34e-146">响应</span><span class="sxs-lookup"><span data-stu-id="eb34e-146">Response</span></span>
<span data-ttu-id="eb34e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb34e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



