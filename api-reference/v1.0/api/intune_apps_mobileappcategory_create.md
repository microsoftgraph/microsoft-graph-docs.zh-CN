# <a name="create-mobileappcategory"></a><span data-ttu-id="5cc2f-101">创建 mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="5cc2f-101">Create mobileAppCategory</span></span>

> <span data-ttu-id="5cc2f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cc2f-103">创建新的 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-103">Create a new [plannerBucket](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cc2f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cc2f-104">Prerequisites</span></span>
<span data-ttu-id="5cc2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5cc2f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cc2f-107">Permission type</span></span>|<span data-ttu-id="5cc2f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5cc2f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc2f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc2f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc2f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc2f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cc2f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc2f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc2f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-112">Not supported.</span></span>|
|<span data-ttu-id="5cc2f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cc2f-113">Application</span></span>|<span data-ttu-id="5cc2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc2f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cc2f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="5cc2f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cc2f-116">Request headers</span></span>
|<span data-ttu-id="5cc2f-117">标头</span><span class="sxs-lookup"><span data-stu-id="5cc2f-117">Header</span></span>|<span data-ttu-id="5cc2f-118">值</span><span class="sxs-lookup"><span data-stu-id="5cc2f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc2f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc2f-119">Authorization</span></span>|<span data-ttu-id="5cc2f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5cc2f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5cc2f-121">Accept</span></span>|<span data-ttu-id="5cc2f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc2f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc2f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cc2f-123">Request body</span></span>
<span data-ttu-id="5cc2f-124">在请求正文中，提供 mobileAppCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5cc2f-125">下表显示创建 mobileAppCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5cc2f-126">属性</span><span class="sxs-lookup"><span data-stu-id="5cc2f-126">Property</span></span>|<span data-ttu-id="5cc2f-127">类型</span><span class="sxs-lookup"><span data-stu-id="5cc2f-127">Type</span></span>|<span data-ttu-id="5cc2f-128">说明</span><span class="sxs-lookup"><span data-stu-id="5cc2f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc2f-129">id</span><span class="sxs-lookup"><span data-stu-id="5cc2f-129">id</span></span>|<span data-ttu-id="5cc2f-130">String</span><span class="sxs-lookup"><span data-stu-id="5cc2f-130">String</span></span>|<span data-ttu-id="5cc2f-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-131">The key of the entity.</span></span>|
|<span data-ttu-id="5cc2f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5cc2f-132">displayName</span></span>|<span data-ttu-id="5cc2f-133">String</span><span class="sxs-lookup"><span data-stu-id="5cc2f-133">String</span></span>|<span data-ttu-id="5cc2f-134">应用类别的名称。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-134">The name of the category.</span></span>|
|<span data-ttu-id="5cc2f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc2f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5cc2f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc2f-136">DateTimeOffset</span></span>|<span data-ttu-id="5cc2f-137">上次修改 mobileAppCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-137">The date and time when the attachment was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="5cc2f-138">响应</span><span class="sxs-lookup"><span data-stu-id="5cc2f-138">Response</span></span>
<span data-ttu-id="5cc2f-139">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-139">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc2f-140">示例</span><span class="sxs-lookup"><span data-stu-id="5cc2f-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cc2f-141">请求</span><span class="sxs-lookup"><span data-stu-id="5cc2f-141">Request</span></span>
<span data-ttu-id="5cc2f-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5cc2f-143">响应</span><span class="sxs-lookup"><span data-stu-id="5cc2f-143">Response</span></span>
<span data-ttu-id="5cc2f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cc2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



