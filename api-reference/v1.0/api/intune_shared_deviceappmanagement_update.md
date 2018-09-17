# <a name="update-deviceappmanagement"></a><span data-ttu-id="d05f5-101">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="d05f5-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="d05f5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d05f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d05f5-103">更新 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d05f5-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d05f5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d05f5-104">Prerequisites</span></span>
<span data-ttu-id="d05f5-105">需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d05f5-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="d05f5-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d05f5-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="d05f5-107">请注意，相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="d05f5-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="d05f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d05f5-108">Permission type</span></span>|<span data-ttu-id="d05f5-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d05f5-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d05f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d05f5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="d05f5-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05f5-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d05f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d05f5-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d05f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d05f5-113">Not supported.</span></span>|
|<span data-ttu-id="d05f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d05f5-114">Application</span></span>|<span data-ttu-id="d05f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d05f5-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d05f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d05f5-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="d05f5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d05f5-117">Request headers</span></span>
|<span data-ttu-id="d05f5-118">标头</span><span class="sxs-lookup"><span data-stu-id="d05f5-118">Header</span></span>|<span data-ttu-id="d05f5-119">值</span><span class="sxs-lookup"><span data-stu-id="d05f5-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d05f5-120">授权</span><span class="sxs-lookup"><span data-stu-id="d05f5-120">Authorization</span></span>|<span data-ttu-id="d05f5-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d05f5-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d05f5-122">接受</span><span class="sxs-lookup"><span data-stu-id="d05f5-122">Accept</span></span>|<span data-ttu-id="d05f5-123">application/json</span><span class="sxs-lookup"><span data-stu-id="d05f5-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d05f5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d05f5-124">Request body</span></span>
<span data-ttu-id="d05f5-125">在请求正文中，提供 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d05f5-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="d05f5-126">下表显示创建 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d05f5-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="d05f5-127">属性</span><span class="sxs-lookup"><span data-stu-id="d05f5-127">Property</span></span>|<span data-ttu-id="d05f5-128">类型</span><span class="sxs-lookup"><span data-stu-id="d05f5-128">Type</span></span>|<span data-ttu-id="d05f5-129">说明</span><span class="sxs-lookup"><span data-stu-id="d05f5-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05f5-130">ID</span><span class="sxs-lookup"><span data-stu-id="d05f5-130">id</span></span>|<span data-ttu-id="d05f5-131">字符串</span><span class="sxs-lookup"><span data-stu-id="d05f5-131">String</span></span>|<span data-ttu-id="d05f5-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d05f5-132">Key of the entity.</span></span>|
|<span data-ttu-id="d05f5-133">**参与／有份**</span><span class="sxs-lookup"><span data-stu-id="d05f5-133">**On-boarding**</span></span>|
|<span data-ttu-id="d05f5-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="d05f5-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="d05f5-135">布尔</span><span class="sxs-lookup"><span data-stu-id="d05f5-135">Boolean</span></span>|<span data-ttu-id="d05f5-136">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="d05f5-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="d05f5-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="d05f5-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="d05f5-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d05f5-138">String</span></span>|<span data-ttu-id="d05f5-139">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="d05f5-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="d05f5-140">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="d05f5-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="d05f5-141">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d05f5-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="d05f5-142">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="d05f5-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="d05f5-143">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="d05f5-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="d05f5-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="d05f5-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="d05f5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05f5-145">DateTimeOffset</span></span>|<span data-ttu-id="d05f5-146">从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。</span><span class="sxs-lookup"><span data-stu-id="d05f5-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="d05f5-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d05f5-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d05f5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d05f5-148">DateTimeOffset</span></span>|<span data-ttu-id="d05f5-149">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="d05f5-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="d05f5-150">响应</span><span class="sxs-lookup"><span data-stu-id="d05f5-150">Response</span></span>
<span data-ttu-id="d05f5-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d05f5-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="d05f5-152">示例请求</span><span class="sxs-lookup"><span data-stu-id="d05f5-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="d05f5-153">响应示例</span><span class="sxs-lookup"><span data-stu-id="d05f5-153">Example response</span></span>

<span data-ttu-id="d05f5-154">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d05f5-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d05f5-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d05f5-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



