# <a name="update-managedebookassignment"></a><span data-ttu-id="89ad6-101">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="89ad6-101">Update managedEBookAssignment</span></span>

> <span data-ttu-id="89ad6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89ad6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89ad6-103">更新 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89ad6-103">Update the properties of a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89ad6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="89ad6-104">Prerequisites</span></span>
<span data-ttu-id="89ad6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="89ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="89ad6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="89ad6-107">Permission type</span></span>|<span data-ttu-id="89ad6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="89ad6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ad6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89ad6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="89ad6-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ad6-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89ad6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89ad6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ad6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="89ad6-112">Not supported.</span></span>|
|<span data-ttu-id="89ad6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="89ad6-113">Application</span></span>|<span data-ttu-id="89ad6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89ad6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ad6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89ad6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="89ad6-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="89ad6-116">Request headers</span></span>
|<span data-ttu-id="89ad6-117">标头</span><span class="sxs-lookup"><span data-stu-id="89ad6-117">Header</span></span>|<span data-ttu-id="89ad6-118">值</span><span class="sxs-lookup"><span data-stu-id="89ad6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ad6-119">授权</span><span class="sxs-lookup"><span data-stu-id="89ad6-119">Authorization</span></span>|<span data-ttu-id="89ad6-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="89ad6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ad6-121">接受</span><span class="sxs-lookup"><span data-stu-id="89ad6-121">Accept</span></span>|<span data-ttu-id="89ad6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="89ad6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ad6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="89ad6-123">Request body</span></span>
<span data-ttu-id="89ad6-124">在请求正文中，提供 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89ad6-124">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>

<span data-ttu-id="89ad6-125">下表显示创建 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89ad6-125">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span>

|<span data-ttu-id="89ad6-126">属性</span><span class="sxs-lookup"><span data-stu-id="89ad6-126">Property</span></span>|<span data-ttu-id="89ad6-127">类型</span><span class="sxs-lookup"><span data-stu-id="89ad6-127">Type</span></span>|<span data-ttu-id="89ad6-128">说明</span><span class="sxs-lookup"><span data-stu-id="89ad6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ad6-129">id</span><span class="sxs-lookup"><span data-stu-id="89ad6-129">id</span></span>|<span data-ttu-id="89ad6-130">字符串</span><span class="sxs-lookup"><span data-stu-id="89ad6-130">String</span></span>|<span data-ttu-id="89ad6-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="89ad6-131">Key of the entity.</span></span>|
|<span data-ttu-id="89ad6-132">target</span><span class="sxs-lookup"><span data-stu-id="89ad6-132">target</span></span>|[<span data-ttu-id="89ad6-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="89ad6-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="89ad6-134">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="89ad6-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="89ad6-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="89ad6-135">installIntent</span></span>|[<span data-ttu-id="89ad6-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="89ad6-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="89ad6-137">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="89ad6-137">The install intent for eBook.</span></span> <span data-ttu-id="89ad6-138">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="89ad6-138">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="89ad6-139">响应</span><span class="sxs-lookup"><span data-stu-id="89ad6-139">Response</span></span>
<span data-ttu-id="89ad6-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89ad6-140">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ad6-141">示例</span><span class="sxs-lookup"><span data-stu-id="89ad6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="89ad6-142">请求</span><span class="sxs-lookup"><span data-stu-id="89ad6-142">Request</span></span>
<span data-ttu-id="89ad6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89ad6-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89ad6-144">响应</span><span class="sxs-lookup"><span data-stu-id="89ad6-144">Response</span></span>
<span data-ttu-id="89ad6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="89ad6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



