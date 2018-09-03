# <a name="create-managedebookassignment"></a><span data-ttu-id="ec349-101">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ec349-101">Create managedEBookAssignment</span></span>

> <span data-ttu-id="ec349-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ec349-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec349-103">创建新的 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec349-103">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec349-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec349-104">Prerequisites</span></span>
<span data-ttu-id="ec349-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ec349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec349-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec349-107">Permission type</span></span>|<span data-ttu-id="ec349-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec349-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec349-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec349-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec349-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec349-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec349-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec349-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec349-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec349-112">Not supported.</span></span>|
|<span data-ttu-id="ec349-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec349-113">Application</span></span>|<span data-ttu-id="ec349-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec349-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec349-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec349-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ec349-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec349-116">Request headers</span></span>
|<span data-ttu-id="ec349-117">标头</span><span class="sxs-lookup"><span data-stu-id="ec349-117">Header</span></span>|<span data-ttu-id="ec349-118">值</span><span class="sxs-lookup"><span data-stu-id="ec349-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec349-119">授权</span><span class="sxs-lookup"><span data-stu-id="ec349-119">Authorization</span></span>|<span data-ttu-id="ec349-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec349-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec349-121">接受</span><span class="sxs-lookup"><span data-stu-id="ec349-121">Accept</span></span>|<span data-ttu-id="ec349-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ec349-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec349-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec349-123">Request body</span></span>
<span data-ttu-id="ec349-124">在请求正文中，提供 managedEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec349-124">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="ec349-125">下表显示创建 managedEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec349-125">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="ec349-126">属性</span><span class="sxs-lookup"><span data-stu-id="ec349-126">Property</span></span>|<span data-ttu-id="ec349-127">类型</span><span class="sxs-lookup"><span data-stu-id="ec349-127">Type</span></span>|<span data-ttu-id="ec349-128">说明</span><span class="sxs-lookup"><span data-stu-id="ec349-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec349-129">ID</span><span class="sxs-lookup"><span data-stu-id="ec349-129">id</span></span>|<span data-ttu-id="ec349-130">字符串</span><span class="sxs-lookup"><span data-stu-id="ec349-130">String</span></span>|<span data-ttu-id="ec349-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec349-131">Key of the entity.</span></span>|
|<span data-ttu-id="ec349-132">target</span><span class="sxs-lookup"><span data-stu-id="ec349-132">target</span></span>|[<span data-ttu-id="ec349-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ec349-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ec349-134">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="ec349-134">The assignment target for eBook.</span></span>|
|<span data-ttu-id="ec349-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="ec349-135">installIntent</span></span>|[<span data-ttu-id="ec349-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="ec349-136">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="ec349-137">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="ec349-137">The install intent for eBook.</span></span> <span data-ttu-id="ec349-138">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="ec349-138">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="ec349-139">响应</span><span class="sxs-lookup"><span data-stu-id="ec349-139">Response</span></span>
<span data-ttu-id="ec349-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec349-140">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec349-141">示例</span><span class="sxs-lookup"><span data-stu-id="ec349-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec349-142">请求</span><span class="sxs-lookup"><span data-stu-id="ec349-142">Request</span></span>
<span data-ttu-id="ec349-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec349-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="ec349-144">响应</span><span class="sxs-lookup"><span data-stu-id="ec349-144">Response</span></span>
<span data-ttu-id="ec349-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec349-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



