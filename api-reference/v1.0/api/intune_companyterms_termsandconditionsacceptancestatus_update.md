# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="e630f-101">更新 termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="e630f-101">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="e630f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e630f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e630f-103">更新 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e630f-103">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e630f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e630f-104">Prerequisites</span></span>
<span data-ttu-id="e630f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e630f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e630f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e630f-107">Permission type</span></span>|<span data-ttu-id="e630f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e630f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e630f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e630f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e630f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e630f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e630f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e630f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e630f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e630f-112">Not supported.</span></span>|
|<span data-ttu-id="e630f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e630f-113">Application</span></span>|<span data-ttu-id="e630f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e630f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e630f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e630f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e630f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e630f-116">Request headers</span></span>
|<span data-ttu-id="e630f-117">标头</span><span class="sxs-lookup"><span data-stu-id="e630f-117">Header</span></span>|<span data-ttu-id="e630f-118">值</span><span class="sxs-lookup"><span data-stu-id="e630f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e630f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e630f-119">Authorization</span></span>|<span data-ttu-id="e630f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e630f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e630f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e630f-121">Accept</span></span>|<span data-ttu-id="e630f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e630f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e630f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e630f-123">Request body</span></span>
<span data-ttu-id="e630f-124">在请求正文中，提供 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e630f-124">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="e630f-125">下表显示创建 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e630f-125">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="e630f-126">属性</span><span class="sxs-lookup"><span data-stu-id="e630f-126">Property</span></span>|<span data-ttu-id="e630f-127">类型</span><span class="sxs-lookup"><span data-stu-id="e630f-127">Type</span></span>|<span data-ttu-id="e630f-128">说明</span><span class="sxs-lookup"><span data-stu-id="e630f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e630f-129">id</span><span class="sxs-lookup"><span data-stu-id="e630f-129">id</span></span>|<span data-ttu-id="e630f-130">String</span><span class="sxs-lookup"><span data-stu-id="e630f-130">String</span></span>|<span data-ttu-id="e630f-131">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e630f-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e630f-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e630f-132">userDisplayName</span></span>|<span data-ttu-id="e630f-133">String</span><span class="sxs-lookup"><span data-stu-id="e630f-133">String</span></span>|<span data-ttu-id="e630f-134">实体所表示的接受状态所属用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e630f-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="e630f-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="e630f-135">acceptedVersion</span></span>|<span data-ttu-id="e630f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e630f-136">Int32</span></span>|<span data-ttu-id="e630f-137">用户所接受的最新 T&C 版本号。</span><span class="sxs-lookup"><span data-stu-id="e630f-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="e630f-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="e630f-138">acceptedDateTime</span></span>|<span data-ttu-id="e630f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e630f-139">DateTimeOffset</span></span>|<span data-ttu-id="e630f-140">用户上次接受条款时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e630f-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="e630f-141">响应</span><span class="sxs-lookup"><span data-stu-id="e630f-141">Response</span></span>
<span data-ttu-id="e630f-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e630f-142">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e630f-143">示例</span><span class="sxs-lookup"><span data-stu-id="e630f-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="e630f-144">请求</span><span class="sxs-lookup"><span data-stu-id="e630f-144">Request</span></span>
<span data-ttu-id="e630f-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e630f-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e630f-146">响应</span><span class="sxs-lookup"><span data-stu-id="e630f-146">Response</span></span>
<span data-ttu-id="e630f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e630f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



