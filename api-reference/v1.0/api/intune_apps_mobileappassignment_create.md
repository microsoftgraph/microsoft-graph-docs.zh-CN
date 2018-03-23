# <a name="create-mobileappassignment"></a><span data-ttu-id="3797f-101">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="3797f-101">Create mobileAppAssignment</span></span>

> <span data-ttu-id="3797f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3797f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3797f-103">创建新的 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3797f-103">Create a new [plannerBucket](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3797f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3797f-104">Prerequisites</span></span>
<span data-ttu-id="3797f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3797f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3797f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3797f-107">Permission type</span></span>|<span data-ttu-id="3797f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3797f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3797f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3797f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3797f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3797f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3797f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3797f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3797f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3797f-112">Not supported.</span></span>|
|<span data-ttu-id="3797f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3797f-113">Application</span></span>|<span data-ttu-id="3797f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3797f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3797f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3797f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3797f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3797f-116">Request headers</span></span>
|<span data-ttu-id="3797f-117">标头</span><span class="sxs-lookup"><span data-stu-id="3797f-117">Header</span></span>|<span data-ttu-id="3797f-118">值</span><span class="sxs-lookup"><span data-stu-id="3797f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3797f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3797f-119">Authorization</span></span>|<span data-ttu-id="3797f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3797f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3797f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3797f-121">Accept</span></span>|<span data-ttu-id="3797f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3797f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3797f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3797f-123">Request body</span></span>
<span data-ttu-id="3797f-124">在请求正文中，提供 mobileAppAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3797f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3797f-125">下表显示创建 mobileAppAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3797f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="3797f-126">属性</span><span class="sxs-lookup"><span data-stu-id="3797f-126">Property</span></span>|<span data-ttu-id="3797f-127">类型</span><span class="sxs-lookup"><span data-stu-id="3797f-127">Type</span></span>|<span data-ttu-id="3797f-128">说明</span><span class="sxs-lookup"><span data-stu-id="3797f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3797f-129">id</span><span class="sxs-lookup"><span data-stu-id="3797f-129">id</span></span>|<span data-ttu-id="3797f-130">String</span><span class="sxs-lookup"><span data-stu-id="3797f-130">String</span></span>|<span data-ttu-id="3797f-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3797f-131">Key of the setting.</span></span>|
|<span data-ttu-id="3797f-132">intent</span><span class="sxs-lookup"><span data-stu-id="3797f-132">intent</span></span>|<span data-ttu-id="3797f-133">String</span><span class="sxs-lookup"><span data-stu-id="3797f-133">String</span></span>|<span data-ttu-id="3797f-134">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="3797f-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="3797f-135">target</span><span class="sxs-lookup"><span data-stu-id="3797f-135">target</span></span>|[<span data-ttu-id="3797f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3797f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3797f-137">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="3797f-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="3797f-138">settings</span><span class="sxs-lookup"><span data-stu-id="3797f-138">settings</span></span>|[<span data-ttu-id="3797f-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3797f-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="3797f-140">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="3797f-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="3797f-141">响应</span><span class="sxs-lookup"><span data-stu-id="3797f-141">Response</span></span>
<span data-ttu-id="3797f-142">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3797f-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3797f-143">示例</span><span class="sxs-lookup"><span data-stu-id="3797f-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="3797f-144">请求</span><span class="sxs-lookup"><span data-stu-id="3797f-144">Request</span></span>
<span data-ttu-id="3797f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3797f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="3797f-146">响应</span><span class="sxs-lookup"><span data-stu-id="3797f-146">Response</span></span>
<span data-ttu-id="3797f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3797f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



