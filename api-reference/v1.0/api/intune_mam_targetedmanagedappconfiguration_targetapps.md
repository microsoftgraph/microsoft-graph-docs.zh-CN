# <a name="targetapps-action"></a><span data-ttu-id="9f6bd-101">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="9f6bd-101">targetApps action</span></span>

> <span data-ttu-id="9f6bd-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f6bd-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9f6bd-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f6bd-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f6bd-104">Prerequisites</span></span>
<span data-ttu-id="9f6bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f6bd-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f6bd-107">Permission type</span></span>|<span data-ttu-id="9f6bd-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f6bd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f6bd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f6bd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9f6bd-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f6bd-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f6bd-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f6bd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f6bd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-112">Not supported.</span></span>|
|<span data-ttu-id="9f6bd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f6bd-113">Application</span></span>|<span data-ttu-id="9f6bd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f6bd-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f6bd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="9f6bd-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f6bd-116">Request headers</span></span>
|<span data-ttu-id="9f6bd-117">标头</span><span class="sxs-lookup"><span data-stu-id="9f6bd-117">Header</span></span>|<span data-ttu-id="9f6bd-118">值</span><span class="sxs-lookup"><span data-stu-id="9f6bd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f6bd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f6bd-119">Authorization</span></span>|<span data-ttu-id="9f6bd-120">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9f6bd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9f6bd-121">Accept</span></span>|<span data-ttu-id="9f6bd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9f6bd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f6bd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f6bd-123">Request body</span></span>
<span data-ttu-id="9f6bd-124">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="9f6bd-125">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9f6bd-126">属性</span><span class="sxs-lookup"><span data-stu-id="9f6bd-126">Property</span></span>|<span data-ttu-id="9f6bd-127">类型</span><span class="sxs-lookup"><span data-stu-id="9f6bd-127">Type</span></span>|<span data-ttu-id="9f6bd-128">说明</span><span class="sxs-lookup"><span data-stu-id="9f6bd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f6bd-129">apps</span><span class="sxs-lookup"><span data-stu-id="9f6bd-129">apps</span></span>|<span data-ttu-id="9f6bd-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f6bd-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) collection</span></span>|<span data-ttu-id="9f6bd-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9f6bd-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9f6bd-132">响应</span><span class="sxs-lookup"><span data-stu-id="9f6bd-132">Response</span></span>
<span data-ttu-id="9f6bd-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f6bd-134">示例</span><span class="sxs-lookup"><span data-stu-id="9f6bd-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f6bd-135">请求</span><span class="sxs-lookup"><span data-stu-id="9f6bd-135">Request</span></span>
<span data-ttu-id="9f6bd-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9f6bd-137">响应</span><span class="sxs-lookup"><span data-stu-id="9f6bd-137">Response</span></span>
<span data-ttu-id="9f6bd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f6bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



