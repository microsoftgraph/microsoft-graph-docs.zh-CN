# <a name="create-mobileappcontent"></a><span data-ttu-id="a478f-101">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="a478f-101">Create mobileAppContent</span></span>

> <span data-ttu-id="a478f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a478f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a478f-103">创建新的 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a478f-103">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a478f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a478f-104">Prerequisites</span></span>
<span data-ttu-id="a478f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a478f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a478f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a478f-107">Permission type</span></span>|<span data-ttu-id="a478f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a478f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a478f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a478f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a478f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a478f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a478f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a478f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a478f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a478f-112">Not supported.</span></span>|
|<span data-ttu-id="a478f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a478f-113">Application</span></span>|<span data-ttu-id="a478f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a478f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a478f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a478f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="a478f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a478f-116">Request headers</span></span>
|<span data-ttu-id="a478f-117">标头</span><span class="sxs-lookup"><span data-stu-id="a478f-117">Header</span></span>|<span data-ttu-id="a478f-118">值</span><span class="sxs-lookup"><span data-stu-id="a478f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a478f-119">授权</span><span class="sxs-lookup"><span data-stu-id="a478f-119">Authorization</span></span>|<span data-ttu-id="a478f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a478f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a478f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a478f-121">Accept</span></span>|<span data-ttu-id="a478f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a478f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a478f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a478f-123">Request body</span></span>
<span data-ttu-id="a478f-124">在请求正文中，提供 mobileAppContent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a478f-124">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="a478f-125">下表显示创建 mobileAppContent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a478f-125">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="a478f-126">属性</span><span class="sxs-lookup"><span data-stu-id="a478f-126">Property</span></span>|<span data-ttu-id="a478f-127">类型</span><span class="sxs-lookup"><span data-stu-id="a478f-127">Type</span></span>|<span data-ttu-id="a478f-128">说明</span><span class="sxs-lookup"><span data-stu-id="a478f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a478f-129">ID</span><span class="sxs-lookup"><span data-stu-id="a478f-129">id</span></span>|<span data-ttu-id="a478f-130">String</span><span class="sxs-lookup"><span data-stu-id="a478f-130">String</span></span>|<span data-ttu-id="a478f-131">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="a478f-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="a478f-132">响应</span><span class="sxs-lookup"><span data-stu-id="a478f-132">Response</span></span>
<span data-ttu-id="a478f-133">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a478f-133">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a478f-134">示例</span><span class="sxs-lookup"><span data-stu-id="a478f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a478f-135">请求</span><span class="sxs-lookup"><span data-stu-id="a478f-135">Request</span></span>
<span data-ttu-id="a478f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a478f-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="a478f-137">响应</span><span class="sxs-lookup"><span data-stu-id="a478f-137">Response</span></span>
<span data-ttu-id="a478f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a478f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```








