# <a name="update-deviceappmanagement"></a><span data-ttu-id="12d35-101">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="12d35-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="12d35-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12d35-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12d35-103">更新 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12d35-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12d35-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="12d35-104">Prerequisites</span></span>
<span data-ttu-id="12d35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="12d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12d35-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="12d35-107">Permission type</span></span>|<span data-ttu-id="12d35-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12d35-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d35-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12d35-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12d35-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d35-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12d35-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12d35-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d35-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="12d35-112">Not supported.</span></span>|
|<span data-ttu-id="12d35-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="12d35-113">Application</span></span>|<span data-ttu-id="12d35-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="12d35-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d35-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12d35-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="12d35-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="12d35-116">Request headers</span></span>
|<span data-ttu-id="12d35-117">标头</span><span class="sxs-lookup"><span data-stu-id="12d35-117">Header</span></span>|<span data-ttu-id="12d35-118">值</span><span class="sxs-lookup"><span data-stu-id="12d35-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d35-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="12d35-119">Authorization</span></span>|<span data-ttu-id="12d35-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12d35-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="12d35-121">Accept</span><span class="sxs-lookup"><span data-stu-id="12d35-121">Accept</span></span>|<span data-ttu-id="12d35-122">application/json</span><span class="sxs-lookup"><span data-stu-id="12d35-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d35-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="12d35-123">Request body</span></span>
<span data-ttu-id="12d35-124">在请求正文中，提供 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12d35-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="12d35-125">下表显示创建 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12d35-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="12d35-126">属性</span><span class="sxs-lookup"><span data-stu-id="12d35-126">Property</span></span>|<span data-ttu-id="12d35-127">类型</span><span class="sxs-lookup"><span data-stu-id="12d35-127">Type</span></span>|<span data-ttu-id="12d35-128">说明</span><span class="sxs-lookup"><span data-stu-id="12d35-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d35-129">id</span><span class="sxs-lookup"><span data-stu-id="12d35-129">id</span></span>|<span data-ttu-id="12d35-130">String</span><span class="sxs-lookup"><span data-stu-id="12d35-130">String</span></span>|<span data-ttu-id="12d35-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12d35-131">Not yet documented</span></span>|
|<span data-ttu-id="12d35-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="12d35-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="12d35-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d35-133">DateTimeOffset</span></span>|<span data-ttu-id="12d35-134">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="12d35-134">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="12d35-135">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="12d35-135">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="12d35-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d35-136">Boolean</span></span>|<span data-ttu-id="12d35-137">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="12d35-137">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="12d35-138">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="12d35-138">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="12d35-139">String</span><span class="sxs-lookup"><span data-stu-id="12d35-139">String</span></span>|<span data-ttu-id="12d35-140">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="12d35-140">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="12d35-141">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="12d35-141">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="12d35-142">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="12d35-142">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="12d35-143">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="12d35-143">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="12d35-144">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="12d35-144">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="12d35-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="12d35-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="12d35-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d35-146">DateTimeOffset</span></span>|<span data-ttu-id="12d35-147">上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="12d35-147">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="12d35-148">响应</span><span class="sxs-lookup"><span data-stu-id="12d35-148">Response</span></span>
<span data-ttu-id="12d35-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12d35-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d35-150">示例</span><span class="sxs-lookup"><span data-stu-id="12d35-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="12d35-151">请求</span><span class="sxs-lookup"><span data-stu-id="12d35-151">Request</span></span>
<span data-ttu-id="12d35-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12d35-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 336

{
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="12d35-153">响应</span><span class="sxs-lookup"><span data-stu-id="12d35-153">Response</span></span>
<span data-ttu-id="12d35-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12d35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```



