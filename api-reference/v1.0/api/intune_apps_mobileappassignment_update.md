# <a name="update-mobileappassignment"></a><span data-ttu-id="9d65c-101">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="9d65c-101">Update mobileAppAssignment</span></span>

> <span data-ttu-id="9d65c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d65c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d65c-103">更新 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d65c-103">Update the properties of a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d65c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d65c-104">Prerequisites</span></span>
<span data-ttu-id="9d65c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9d65c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d65c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d65c-107">Permission type</span></span>|<span data-ttu-id="9d65c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d65c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d65c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d65c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9d65c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d65c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d65c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d65c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d65c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d65c-112">Not supported.</span></span>|
|<span data-ttu-id="9d65c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d65c-113">Application</span></span>|<span data-ttu-id="9d65c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d65c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d65c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d65c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9d65c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d65c-116">Request headers</span></span>
|<span data-ttu-id="9d65c-117">标头</span><span class="sxs-lookup"><span data-stu-id="9d65c-117">Header</span></span>|<span data-ttu-id="9d65c-118">值</span><span class="sxs-lookup"><span data-stu-id="9d65c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d65c-119">授权</span><span class="sxs-lookup"><span data-stu-id="9d65c-119">Authorization</span></span>|<span data-ttu-id="9d65c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d65c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d65c-121">接受</span><span class="sxs-lookup"><span data-stu-id="9d65c-121">Accept</span></span>|<span data-ttu-id="9d65c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9d65c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d65c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d65c-123">Request body</span></span>
<span data-ttu-id="9d65c-124">在请求正文中，提供 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d65c-124">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>

<span data-ttu-id="9d65c-125">下表显示创建 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9d65c-125">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span></span>

|<span data-ttu-id="9d65c-126">属性</span><span class="sxs-lookup"><span data-stu-id="9d65c-126">Property</span></span>|<span data-ttu-id="9d65c-127">类型</span><span class="sxs-lookup"><span data-stu-id="9d65c-127">Type</span></span>|<span data-ttu-id="9d65c-128">说明</span><span class="sxs-lookup"><span data-stu-id="9d65c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d65c-129">ID</span><span class="sxs-lookup"><span data-stu-id="9d65c-129">id</span></span>|<span data-ttu-id="9d65c-130">字符串</span><span class="sxs-lookup"><span data-stu-id="9d65c-130">String</span></span>|<span data-ttu-id="9d65c-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9d65c-131">Key of the entity.</span></span>|
|<span data-ttu-id="9d65c-132">intent</span><span class="sxs-lookup"><span data-stu-id="9d65c-132">intent</span></span>|[<span data-ttu-id="9d65c-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="9d65c-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="9d65c-134">由管理员定义的安装意图。可能的值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="9d65c-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="9d65c-135">target</span><span class="sxs-lookup"><span data-stu-id="9d65c-135">target</span></span>|[<span data-ttu-id="9d65c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9d65c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9d65c-137">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="9d65c-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="9d65c-138">settings</span><span class="sxs-lookup"><span data-stu-id="9d65c-138">settings</span></span>|[<span data-ttu-id="9d65c-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9d65c-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="9d65c-140">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="9d65c-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="9d65c-141">响应</span><span class="sxs-lookup"><span data-stu-id="9d65c-141">Response</span></span>
<span data-ttu-id="9d65c-142">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d65c-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d65c-143">示例</span><span class="sxs-lookup"><span data-stu-id="9d65c-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d65c-144">请求</span><span class="sxs-lookup"><span data-stu-id="9d65c-144">Request</span></span>
<span data-ttu-id="9d65c-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d65c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 215

{
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="9d65c-146">响应</span><span class="sxs-lookup"><span data-stu-id="9d65c-146">Response</span></span>
<span data-ttu-id="9d65c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d65c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








