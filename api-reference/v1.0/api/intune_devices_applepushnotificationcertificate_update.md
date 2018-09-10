# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="f9fc5-101">更新 applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f9fc5-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="f9fc5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9fc5-103">更新 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-103">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9fc5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9fc5-104">Prerequisites</span></span>
<span data-ttu-id="f9fc5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9fc5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9fc5-107">Permission type</span></span>|<span data-ttu-id="f9fc5-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9fc5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9fc5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9fc5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f9fc5-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9fc5-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9fc5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9fc5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9fc5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-112">Not supported.</span></span>|
|<span data-ttu-id="f9fc5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9fc5-113">Application</span></span>|<span data-ttu-id="f9fc5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9fc5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9fc5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f9fc5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9fc5-116">Request headers</span></span>
|<span data-ttu-id="f9fc5-117">标头</span><span class="sxs-lookup"><span data-stu-id="f9fc5-117">Header</span></span>|<span data-ttu-id="f9fc5-118">值</span><span class="sxs-lookup"><span data-stu-id="f9fc5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9fc5-119">授权</span><span class="sxs-lookup"><span data-stu-id="f9fc5-119">Authorization</span></span>|<span data-ttu-id="f9fc5-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9fc5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f9fc5-121">Accept</span></span>|<span data-ttu-id="f9fc5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f9fc5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9fc5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9fc5-123">Request body</span></span>
<span data-ttu-id="f9fc5-124">在请求正文中，提供 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-124">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="f9fc5-125">下表显示创建 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-125">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="f9fc5-126">属性</span><span class="sxs-lookup"><span data-stu-id="f9fc5-126">Property</span></span>|<span data-ttu-id="f9fc5-127">类型</span><span class="sxs-lookup"><span data-stu-id="f9fc5-127">Type</span></span>|<span data-ttu-id="f9fc5-128">说明</span><span class="sxs-lookup"><span data-stu-id="f9fc5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9fc5-129">ID</span><span class="sxs-lookup"><span data-stu-id="f9fc5-129">id</span></span>|<span data-ttu-id="f9fc5-130">String</span><span class="sxs-lookup"><span data-stu-id="f9fc5-130">String</span></span>|<span data-ttu-id="f9fc5-131">证书的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f9fc5-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="f9fc5-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f9fc5-132">appleIdentifier</span></span>|<span data-ttu-id="f9fc5-133">String</span><span class="sxs-lookup"><span data-stu-id="f9fc5-133">String</span></span>|<span data-ttu-id="f9fc5-134">用于创建 MDM 推送证书的帐户 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="f9fc5-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="f9fc5-135">topicIdentifier</span></span>|<span data-ttu-id="f9fc5-136">String</span><span class="sxs-lookup"><span data-stu-id="f9fc5-136">String</span></span>|<span data-ttu-id="f9fc5-137">主题 ID。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-137">Topic Id.</span></span>|
|<span data-ttu-id="f9fc5-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9fc5-138">lastModifiedDateTime</span></span>|<span data-ttu-id="f9fc5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9fc5-139">DateTimeOffset</span></span>|<span data-ttu-id="f9fc5-140">上次修改 Apple 推送通知证书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f9fc5-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9fc5-141">expirationDateTime</span></span>|<span data-ttu-id="f9fc5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9fc5-142">DateTimeOffset</span></span>|<span data-ttu-id="f9fc5-143">Apple 推送通知证书的到期日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="f9fc5-144">certificate</span><span class="sxs-lookup"><span data-stu-id="f9fc5-144">certificate</span></span>|<span data-ttu-id="f9fc5-145">String</span><span class="sxs-lookup"><span data-stu-id="f9fc5-145">String</span></span>|<span data-ttu-id="f9fc5-146">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f9fc5-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f9fc5-147">响应</span><span class="sxs-lookup"><span data-stu-id="f9fc5-147">Response</span></span>
<span data-ttu-id="f9fc5-148">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-148">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9fc5-149">示例</span><span class="sxs-lookup"><span data-stu-id="f9fc5-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9fc5-150">请求</span><span class="sxs-lookup"><span data-stu-id="f9fc5-150">Request</span></span>
<span data-ttu-id="f9fc5-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 264

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="f9fc5-152">响应</span><span class="sxs-lookup"><span data-stu-id="f9fc5-152">Response</span></span>
<span data-ttu-id="f9fc5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9fc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```








