# <a name="update-termsandconditions"></a><span data-ttu-id="6afed-101">更新 termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6afed-101">Update termsAndConditions</span></span>

> <span data-ttu-id="6afed-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6afed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6afed-103">更新 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6afed-103">Update the properties of a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6afed-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6afed-104">Prerequisites</span></span>
<span data-ttu-id="6afed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6afed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6afed-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6afed-107">Permission type</span></span>|<span data-ttu-id="6afed-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6afed-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6afed-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6afed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6afed-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6afed-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6afed-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6afed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6afed-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6afed-112">Not supported.</span></span>|
|<span data-ttu-id="6afed-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6afed-113">Application</span></span>|<span data-ttu-id="6afed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6afed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6afed-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6afed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="6afed-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6afed-116">Request headers</span></span>
|<span data-ttu-id="6afed-117">标头</span><span class="sxs-lookup"><span data-stu-id="6afed-117">Header</span></span>|<span data-ttu-id="6afed-118">值</span><span class="sxs-lookup"><span data-stu-id="6afed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6afed-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6afed-119">Authorization</span></span>|<span data-ttu-id="6afed-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6afed-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6afed-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6afed-121">Accept</span></span>|<span data-ttu-id="6afed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6afed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6afed-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6afed-123">Request body</span></span>
<span data-ttu-id="6afed-124">在请求正文中，提供 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6afed-124">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>

<span data-ttu-id="6afed-125">下表显示创建 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6afed-125">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span></span>

|<span data-ttu-id="6afed-126">属性</span><span class="sxs-lookup"><span data-stu-id="6afed-126">Property</span></span>|<span data-ttu-id="6afed-127">类型</span><span class="sxs-lookup"><span data-stu-id="6afed-127">Type</span></span>|<span data-ttu-id="6afed-128">说明</span><span class="sxs-lookup"><span data-stu-id="6afed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6afed-129">id</span><span class="sxs-lookup"><span data-stu-id="6afed-129">id</span></span>|<span data-ttu-id="6afed-130">String</span><span class="sxs-lookup"><span data-stu-id="6afed-130">String</span></span>|<span data-ttu-id="6afed-131">T&C 策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6afed-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="6afed-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6afed-132">createdDateTime</span></span>|<span data-ttu-id="6afed-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6afed-133">DateTimeOffset</span></span>|<span data-ttu-id="6afed-134">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6afed-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="6afed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6afed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6afed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6afed-136">DateTimeOffset</span></span>|<span data-ttu-id="6afed-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6afed-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6afed-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6afed-138">displayName</span></span>|<span data-ttu-id="6afed-139">String</span><span class="sxs-lookup"><span data-stu-id="6afed-139">String</span></span>|<span data-ttu-id="6afed-140">管理员提供的 T&C 策略名称。</span><span class="sxs-lookup"><span data-stu-id="6afed-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="6afed-141">description</span><span class="sxs-lookup"><span data-stu-id="6afed-141">description</span></span>|<span data-ttu-id="6afed-142">String</span><span class="sxs-lookup"><span data-stu-id="6afed-142">String</span></span>|<span data-ttu-id="6afed-143">管理员提供的 T&C 策略描述。</span><span class="sxs-lookup"><span data-stu-id="6afed-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="6afed-144">title</span><span class="sxs-lookup"><span data-stu-id="6afed-144">title</span></span>|<span data-ttu-id="6afed-145">String</span><span class="sxs-lookup"><span data-stu-id="6afed-145">String</span></span>|<span data-ttu-id="6afed-146">管理员提供的条款和条件标题。</span><span class="sxs-lookup"><span data-stu-id="6afed-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="6afed-147">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6afed-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6afed-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="6afed-148">bodyText</span></span>|<span data-ttu-id="6afed-149">String</span><span class="sxs-lookup"><span data-stu-id="6afed-149">String</span></span>|<span data-ttu-id="6afed-150">管理员提供的条款和条件正文文本，通常为条款本身。</span><span class="sxs-lookup"><span data-stu-id="6afed-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="6afed-151">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6afed-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6afed-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="6afed-152">acceptanceStatement</span></span>|<span data-ttu-id="6afed-153">String</span><span class="sxs-lookup"><span data-stu-id="6afed-153">String</span></span>|<span data-ttu-id="6afed-154">管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。</span><span class="sxs-lookup"><span data-stu-id="6afed-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="6afed-155">这会向用户显示，提示用户接受 T&C 策略。</span><span class="sxs-lookup"><span data-stu-id="6afed-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="6afed-156">version</span><span class="sxs-lookup"><span data-stu-id="6afed-156">version</span></span>|<span data-ttu-id="6afed-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6afed-157">Int32</span></span>|<span data-ttu-id="6afed-158">指示当前条款版本的整数。</span><span class="sxs-lookup"><span data-stu-id="6afed-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="6afed-159">当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。</span><span class="sxs-lookup"><span data-stu-id="6afed-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6afed-160">响应</span><span class="sxs-lookup"><span data-stu-id="6afed-160">Response</span></span>
<span data-ttu-id="6afed-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6afed-161">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6afed-162">示例</span><span class="sxs-lookup"><span data-stu-id="6afed-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="6afed-163">请求</span><span class="sxs-lookup"><span data-stu-id="6afed-163">Request</span></span>
<span data-ttu-id="6afed-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6afed-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="6afed-165">响应</span><span class="sxs-lookup"><span data-stu-id="6afed-165">Response</span></span>
<span data-ttu-id="6afed-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6afed-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



