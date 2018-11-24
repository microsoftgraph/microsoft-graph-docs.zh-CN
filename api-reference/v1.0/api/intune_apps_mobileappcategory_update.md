# <a name="update-mobileappcategory"></a><span data-ttu-id="550ae-101">更新 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="550ae-101">Update mobileAppCategory</span></span>

> <span data-ttu-id="550ae-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="550ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="550ae-103">更新 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="550ae-103">Update the properties of a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="550ae-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="550ae-104">Prerequisites</span></span>
<span data-ttu-id="550ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="550ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="550ae-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="550ae-107">Permission type</span></span>|<span data-ttu-id="550ae-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="550ae-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="550ae-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="550ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="550ae-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="550ae-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="550ae-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="550ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="550ae-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="550ae-112">Not supported.</span></span>|
|<span data-ttu-id="550ae-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="550ae-113">Application</span></span>|<span data-ttu-id="550ae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="550ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="550ae-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="550ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="550ae-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="550ae-116">Request headers</span></span>
|<span data-ttu-id="550ae-117">标头</span><span class="sxs-lookup"><span data-stu-id="550ae-117">Header</span></span>|<span data-ttu-id="550ae-118">值</span><span class="sxs-lookup"><span data-stu-id="550ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="550ae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="550ae-119">Authorization</span></span>|<span data-ttu-id="550ae-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="550ae-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="550ae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="550ae-121">Accept</span></span>|<span data-ttu-id="550ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="550ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="550ae-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="550ae-123">Request body</span></span>
<span data-ttu-id="550ae-124">在请求正文中，提供 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="550ae-124">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>

<span data-ttu-id="550ae-125">下表显示创建 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="550ae-125">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span></span>

|<span data-ttu-id="550ae-126">属性</span><span class="sxs-lookup"><span data-stu-id="550ae-126">Property</span></span>|<span data-ttu-id="550ae-127">类型</span><span class="sxs-lookup"><span data-stu-id="550ae-127">Type</span></span>|<span data-ttu-id="550ae-128">说明</span><span class="sxs-lookup"><span data-stu-id="550ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="550ae-129">id</span><span class="sxs-lookup"><span data-stu-id="550ae-129">id</span></span>|<span data-ttu-id="550ae-130">String</span><span class="sxs-lookup"><span data-stu-id="550ae-130">String</span></span>|<span data-ttu-id="550ae-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="550ae-131">The key of the entity.</span></span>|
|<span data-ttu-id="550ae-132">displayName</span><span class="sxs-lookup"><span data-stu-id="550ae-132">displayName</span></span>|<span data-ttu-id="550ae-133">String</span><span class="sxs-lookup"><span data-stu-id="550ae-133">String</span></span>|<span data-ttu-id="550ae-134">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="550ae-134">The name of the app category.</span></span>|
|<span data-ttu-id="550ae-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="550ae-135">lastModifiedDateTime</span></span>|<span data-ttu-id="550ae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="550ae-136">DateTimeOffset</span></span>|<span data-ttu-id="550ae-137">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="550ae-137">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="550ae-138">响应</span><span class="sxs-lookup"><span data-stu-id="550ae-138">Response</span></span>
<span data-ttu-id="550ae-139">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="550ae-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="550ae-140">示例</span><span class="sxs-lookup"><span data-stu-id="550ae-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="550ae-141">请求</span><span class="sxs-lookup"><span data-stu-id="550ae-141">Request</span></span>
<span data-ttu-id="550ae-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="550ae-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="550ae-143">响应</span><span class="sxs-lookup"><span data-stu-id="550ae-143">Response</span></span>
<span data-ttu-id="550ae-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="550ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



