# <a name="update-remoteassistancepartner"></a><span data-ttu-id="429d9-101">更新 remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="429d9-101">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="429d9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="429d9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="429d9-103">更新 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="429d9-103">Update the properties of a [calendar](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="429d9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="429d9-104">Prerequisites</span></span>
<span data-ttu-id="429d9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="429d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="429d9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="429d9-107">Permission type</span></span>|<span data-ttu-id="429d9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="429d9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="429d9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="429d9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="429d9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429d9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="429d9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="429d9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="429d9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="429d9-112">Not supported.</span></span>|
|<span data-ttu-id="429d9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="429d9-113">Application</span></span>|<span data-ttu-id="429d9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="429d9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="429d9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="429d9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="429d9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="429d9-116">Request headers</span></span>
|<span data-ttu-id="429d9-117">标头</span><span class="sxs-lookup"><span data-stu-id="429d9-117">Header</span></span>|<span data-ttu-id="429d9-118">值</span><span class="sxs-lookup"><span data-stu-id="429d9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="429d9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="429d9-119">Authorization</span></span>|<span data-ttu-id="429d9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="429d9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="429d9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="429d9-121">Accept</span></span>|<span data-ttu-id="429d9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="429d9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="429d9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="429d9-123">Request body</span></span>
<span data-ttu-id="429d9-124">在请求正文中，提供 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="429d9-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="429d9-125">下表显示创建 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="429d9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="429d9-126">属性</span><span class="sxs-lookup"><span data-stu-id="429d9-126">Property</span></span>|<span data-ttu-id="429d9-127">类型</span><span class="sxs-lookup"><span data-stu-id="429d9-127">Type</span></span>|<span data-ttu-id="429d9-128">说明</span><span class="sxs-lookup"><span data-stu-id="429d9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="429d9-129">id</span><span class="sxs-lookup"><span data-stu-id="429d9-129">id</span></span>|<span data-ttu-id="429d9-130">String</span><span class="sxs-lookup"><span data-stu-id="429d9-130">String</span></span>|<span data-ttu-id="429d9-131">合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="429d9-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="429d9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="429d9-132">displayName</span></span>|<span data-ttu-id="429d9-133">String</span><span class="sxs-lookup"><span data-stu-id="429d9-133">String</span></span>|<span data-ttu-id="429d9-134">合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="429d9-134">Display name of the item</span></span>|
|<span data-ttu-id="429d9-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="429d9-135">onboardingUrl</span></span>|<span data-ttu-id="429d9-136">String</span><span class="sxs-lookup"><span data-stu-id="429d9-136">String</span></span>|<span data-ttu-id="429d9-137">合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。</span><span class="sxs-lookup"><span data-stu-id="429d9-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="429d9-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="429d9-138">onboardingStatus</span></span>|<span data-ttu-id="429d9-139">String</span><span class="sxs-lookup"><span data-stu-id="429d9-139">String</span></span>|<span data-ttu-id="429d9-140">TBD。可取值为：`notOnboarded`、`onboarding`、`onboarded`。</span><span class="sxs-lookup"><span data-stu-id="429d9-140">Possible values are: `notOnboarded`, `onboarding`, `onboarded`, .</span></span>|
|<span data-ttu-id="429d9-141">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="429d9-141">lastConnectionDateTime</span></span>|<span data-ttu-id="429d9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="429d9-142">DateTimeOffset</span></span>|<span data-ttu-id="429d9-143">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="429d9-143">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="429d9-144">响应</span><span class="sxs-lookup"><span data-stu-id="429d9-144">Response</span></span>
<span data-ttu-id="429d9-145">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="429d9-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429d9-146">示例</span><span class="sxs-lookup"><span data-stu-id="429d9-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="429d9-147">请求</span><span class="sxs-lookup"><span data-stu-id="429d9-147">Request</span></span>
<span data-ttu-id="429d9-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="429d9-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="429d9-149">响应</span><span class="sxs-lookup"><span data-stu-id="429d9-149">Response</span></span>
<span data-ttu-id="429d9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="429d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



