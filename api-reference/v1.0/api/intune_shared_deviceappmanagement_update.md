# <a name="update-deviceappmanagement"></a><span data-ttu-id="015e0-101">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="015e0-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="015e0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="015e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="015e0-103">更新 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="015e0-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="015e0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="015e0-104">Prerequisites</span></span>
<span data-ttu-id="015e0-105">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="015e0-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="015e0-106">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="015e0-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="015e0-107">请注意，在相应权限根据工作流而有所不同。</span><span class="sxs-lookup"><span data-stu-id="015e0-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="015e0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="015e0-108">Permission type</span></span>|<span data-ttu-id="015e0-109">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="015e0-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="015e0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="015e0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="015e0-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="015e0-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="015e0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="015e0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="015e0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="015e0-113">Not supported.</span></span>|
|<span data-ttu-id="015e0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="015e0-114">Application</span></span>|<span data-ttu-id="015e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="015e0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="015e0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="015e0-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="015e0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="015e0-117">Request headers</span></span>
|<span data-ttu-id="015e0-118">标头</span><span class="sxs-lookup"><span data-stu-id="015e0-118">Header</span></span>|<span data-ttu-id="015e0-119">值</span><span class="sxs-lookup"><span data-stu-id="015e0-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="015e0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="015e0-120">Authorization</span></span>|<span data-ttu-id="015e0-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="015e0-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="015e0-122">Accept</span><span class="sxs-lookup"><span data-stu-id="015e0-122">Accept</span></span>|<span data-ttu-id="015e0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="015e0-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="015e0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="015e0-124">Request body</span></span>
<span data-ttu-id="015e0-125">在请求正文中，提供 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="015e0-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="015e0-126">下表显示创建 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="015e0-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="015e0-127">属性</span><span class="sxs-lookup"><span data-stu-id="015e0-127">Property</span></span>|<span data-ttu-id="015e0-128">类型</span><span class="sxs-lookup"><span data-stu-id="015e0-128">Type</span></span>|<span data-ttu-id="015e0-129">说明</span><span class="sxs-lookup"><span data-stu-id="015e0-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="015e0-130">id</span><span class="sxs-lookup"><span data-stu-id="015e0-130">id</span></span>|<span data-ttu-id="015e0-131">String</span><span class="sxs-lookup"><span data-stu-id="015e0-131">String</span></span>|<span data-ttu-id="015e0-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="015e0-132">Key of the entity.</span></span>|
|<span data-ttu-id="015e0-133">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="015e0-133">**Onboarding**</span></span>|
|<span data-ttu-id="015e0-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="015e0-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="015e0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="015e0-135">Boolean</span></span>|<span data-ttu-id="015e0-136">帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。</span><span class="sxs-lookup"><span data-stu-id="015e0-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="015e0-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="015e0-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="015e0-138">String</span><span class="sxs-lookup"><span data-stu-id="015e0-138">String</span></span>|<span data-ttu-id="015e0-139">用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。</span><span class="sxs-lookup"><span data-stu-id="015e0-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="015e0-140">特定于国家/地区的区域性。</span><span class="sxs-lookup"><span data-stu-id="015e0-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="015e0-141">这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。</span><span class="sxs-lookup"><span data-stu-id="015e0-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="015e0-142">格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="015e0-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="015e0-143">例如，“en-US”（“英语(美国)）是一个特定的区域性。</span><span class="sxs-lookup"><span data-stu-id="015e0-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="015e0-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="015e0-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="015e0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="015e0-145">DateTimeOffset</span></span>|<span data-ttu-id="015e0-146">从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。</span><span class="sxs-lookup"><span data-stu-id="015e0-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="015e0-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="015e0-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="015e0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="015e0-148">DateTimeOffset</span></span>|<span data-ttu-id="015e0-149">适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。</span><span class="sxs-lookup"><span data-stu-id="015e0-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="015e0-150">响应</span><span class="sxs-lookup"><span data-stu-id="015e0-150">Response</span></span>
<span data-ttu-id="015e0-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="015e0-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="015e0-152">示例请求</span><span class="sxs-lookup"><span data-stu-id="015e0-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="015e0-153">响应示例</span><span class="sxs-lookup"><span data-stu-id="015e0-153">Example response</span></span>

<span data-ttu-id="015e0-154">为简便起见，如下所示的响应对象可能会被截断。</span><span class="sxs-lookup"><span data-stu-id="015e0-154">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="015e0-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="015e0-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



