# <a name="create-iosvppebookassignment"></a><span data-ttu-id="39075-101">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="39075-101">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="39075-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39075-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39075-103">创建新的 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39075-103">Create a new [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39075-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="39075-104">Prerequisites</span></span>
<span data-ttu-id="39075-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="39075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39075-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="39075-107">Permission type</span></span>|<span data-ttu-id="39075-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39075-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39075-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39075-109">Delegated (work or school account)</span></span>|<span data-ttu-id="39075-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39075-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39075-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39075-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39075-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="39075-112">Not supported.</span></span>|
|<span data-ttu-id="39075-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="39075-113">Application</span></span>|<span data-ttu-id="39075-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="39075-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39075-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39075-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="39075-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="39075-116">Request headers</span></span>
|<span data-ttu-id="39075-117">标头</span><span class="sxs-lookup"><span data-stu-id="39075-117">Header</span></span>|<span data-ttu-id="39075-118">值</span><span class="sxs-lookup"><span data-stu-id="39075-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39075-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="39075-119">Authorization</span></span>|<span data-ttu-id="39075-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39075-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39075-121">Accept</span><span class="sxs-lookup"><span data-stu-id="39075-121">Accept</span></span>|<span data-ttu-id="39075-122">application/json</span><span class="sxs-lookup"><span data-stu-id="39075-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39075-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="39075-123">Request body</span></span>
<span data-ttu-id="39075-124">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39075-124">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="39075-125">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="39075-125">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="39075-126">属性</span><span class="sxs-lookup"><span data-stu-id="39075-126">Property</span></span>|<span data-ttu-id="39075-127">类型</span><span class="sxs-lookup"><span data-stu-id="39075-127">Type</span></span>|<span data-ttu-id="39075-128">说明</span><span class="sxs-lookup"><span data-stu-id="39075-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39075-129">id</span><span class="sxs-lookup"><span data-stu-id="39075-129">id</span></span>|<span data-ttu-id="39075-130">String</span><span class="sxs-lookup"><span data-stu-id="39075-130">String</span></span>|<span data-ttu-id="39075-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="39075-131">Key of the entity.</span></span> <span data-ttu-id="39075-132">继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="39075-132">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="39075-133">target</span><span class="sxs-lookup"><span data-stu-id="39075-133">target</span></span>|[<span data-ttu-id="39075-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="39075-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="39075-135">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="39075-135">The assignment target for eBook.</span></span> <span data-ttu-id="39075-136">继承自 [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="39075-136">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span></span>|
|<span data-ttu-id="39075-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="39075-137">installIntent</span></span>|[<span data-ttu-id="39075-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="39075-138">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="39075-139">电子图书的安装意向。</span><span class="sxs-lookup"><span data-stu-id="39075-139">The install intent for eBook.</span></span> <span data-ttu-id="39075-140">继承自[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="39075-140">Inherited from [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span> <span data-ttu-id="39075-141">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="39075-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="39075-142">响应</span><span class="sxs-lookup"><span data-stu-id="39075-142">Response</span></span>
<span data-ttu-id="39075-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39075-143">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39075-144">示例</span><span class="sxs-lookup"><span data-stu-id="39075-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="39075-145">请求</span><span class="sxs-lookup"><span data-stu-id="39075-145">Request</span></span>
<span data-ttu-id="39075-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39075-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="39075-147">响应</span><span class="sxs-lookup"><span data-stu-id="39075-147">Response</span></span>
<span data-ttu-id="39075-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39075-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



