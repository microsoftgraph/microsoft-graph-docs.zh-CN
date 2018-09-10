# <a name="delete-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="522bb-101">删除 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="522bb-101">Delete deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="522bb-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="522bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="522bb-103">删除 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="522bb-103">Deletes a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="522bb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="522bb-104">Prerequisites</span></span>
<span data-ttu-id="522bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="522bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="522bb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="522bb-107">Permission type</span></span>|<span data-ttu-id="522bb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="522bb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="522bb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="522bb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="522bb-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522bb-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="522bb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="522bb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="522bb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="522bb-112">Not supported.</span></span>|
|<span data-ttu-id="522bb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="522bb-113">Application</span></span>|<span data-ttu-id="522bb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="522bb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="522bb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="522bb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="522bb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="522bb-116">Request headers</span></span>
|<span data-ttu-id="522bb-117">标头</span><span class="sxs-lookup"><span data-stu-id="522bb-117">Header</span></span>|<span data-ttu-id="522bb-118">值</span><span class="sxs-lookup"><span data-stu-id="522bb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="522bb-119">授权</span><span class="sxs-lookup"><span data-stu-id="522bb-119">Authorization</span></span>|<span data-ttu-id="522bb-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="522bb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="522bb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="522bb-121">Accept</span></span>|<span data-ttu-id="522bb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="522bb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="522bb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="522bb-123">Request body</span></span>
<span data-ttu-id="522bb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="522bb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="522bb-125">响应</span><span class="sxs-lookup"><span data-stu-id="522bb-125">Response</span></span>
<span data-ttu-id="522bb-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="522bb-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="522bb-127">示例</span><span class="sxs-lookup"><span data-stu-id="522bb-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="522bb-128">请求</span><span class="sxs-lookup"><span data-stu-id="522bb-128">Request</span></span>
<span data-ttu-id="522bb-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="522bb-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="522bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="522bb-130">Response</span></span>
<span data-ttu-id="522bb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="522bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








