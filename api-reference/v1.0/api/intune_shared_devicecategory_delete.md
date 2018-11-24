# <a name="delete-devicecategory"></a><span data-ttu-id="44b1b-101">删除 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="44b1b-101">Delete deviceCategory</span></span>

> <span data-ttu-id="44b1b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44b1b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44b1b-103">删除 [deviceCategory](../resources/intune_shared_devicecategory.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-103">Deletes a [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44b1b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="44b1b-104">Prerequisites</span></span>
<span data-ttu-id="44b1b-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="44b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44b1b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="44b1b-107">Permission type</span></span>|<span data-ttu-id="44b1b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44b1b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44b1b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44b1b-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44b1b-110">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="44b1b-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="44b1b-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b1b-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44b1b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44b1b-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44b1b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b1b-113">Not supported.</span></span>|
|<span data-ttu-id="44b1b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="44b1b-114">Application</span></span>|<span data-ttu-id="44b1b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b1b-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44b1b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44b1b-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="44b1b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="44b1b-117">Request headers</span></span>
|<span data-ttu-id="44b1b-118">标头</span><span class="sxs-lookup"><span data-stu-id="44b1b-118">Header</span></span>|<span data-ttu-id="44b1b-119">值</span><span class="sxs-lookup"><span data-stu-id="44b1b-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44b1b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b1b-120">Authorization</span></span>|<span data-ttu-id="44b1b-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44b1b-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44b1b-122">Accept</span><span class="sxs-lookup"><span data-stu-id="44b1b-122">Accept</span></span>|<span data-ttu-id="44b1b-123">application/json</span><span class="sxs-lookup"><span data-stu-id="44b1b-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44b1b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="44b1b-124">Request body</span></span>
<span data-ttu-id="44b1b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44b1b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44b1b-126">响应</span><span class="sxs-lookup"><span data-stu-id="44b1b-126">Response</span></span>
<span data-ttu-id="44b1b-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="44b1b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="44b1b-128">示例</span><span class="sxs-lookup"><span data-stu-id="44b1b-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="44b1b-129">请求</span><span class="sxs-lookup"><span data-stu-id="44b1b-129">Request</span></span>
<span data-ttu-id="44b1b-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44b1b-130">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="44b1b-131">响应</span><span class="sxs-lookup"><span data-stu-id="44b1b-131">Response</span></span>
<span data-ttu-id="44b1b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44b1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



