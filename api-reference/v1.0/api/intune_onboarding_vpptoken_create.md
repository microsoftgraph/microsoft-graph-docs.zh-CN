# <a name="create-vpptoken"></a><span data-ttu-id="5cac9-101">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="5cac9-101">Create vppToken</span></span>

> <span data-ttu-id="5cac9-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5cac9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cac9-103">创建新的 [vppToken](../resources/intune_onboarding_vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cac9-103">Create a new [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cac9-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cac9-104">Prerequisites</span></span>
<span data-ttu-id="5cac9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5cac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5cac9-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cac9-107">Permission type</span></span>|<span data-ttu-id="5cac9-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5cac9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cac9-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cac9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5cac9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cac9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5cac9-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cac9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cac9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cac9-112">Not supported.</span></span>|
|<span data-ttu-id="5cac9-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cac9-113">Application</span></span>|<span data-ttu-id="5cac9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cac9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cac9-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cac9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="5cac9-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cac9-116">Request headers</span></span>
|<span data-ttu-id="5cac9-117">标头</span><span class="sxs-lookup"><span data-stu-id="5cac9-117">Header</span></span>|<span data-ttu-id="5cac9-118">值</span><span class="sxs-lookup"><span data-stu-id="5cac9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cac9-119">授权</span><span class="sxs-lookup"><span data-stu-id="5cac9-119">Authorization</span></span>|<span data-ttu-id="5cac9-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cac9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cac9-121">接受</span><span class="sxs-lookup"><span data-stu-id="5cac9-121">Accept</span></span>|<span data-ttu-id="5cac9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5cac9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cac9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cac9-123">Request body</span></span>
<span data-ttu-id="5cac9-124">在请求正文中，提供 vppToken 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cac9-124">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="5cac9-125">下表显示创建 vppToken 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5cac9-125">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="5cac9-126">属性</span><span class="sxs-lookup"><span data-stu-id="5cac9-126">Property</span></span>|<span data-ttu-id="5cac9-127">类型</span><span class="sxs-lookup"><span data-stu-id="5cac9-127">Type</span></span>|<span data-ttu-id="5cac9-128">说明</span><span class="sxs-lookup"><span data-stu-id="5cac9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cac9-129">ID</span><span class="sxs-lookup"><span data-stu-id="5cac9-129">id</span></span>|<span data-ttu-id="5cac9-130">字符串</span><span class="sxs-lookup"><span data-stu-id="5cac9-130">String</span></span>|<span data-ttu-id="5cac9-131">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="5cac9-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="5cac9-132">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="5cac9-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="5cac9-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="5cac9-133">organizationName</span></span>|<span data-ttu-id="5cac9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5cac9-134">String</span></span>|<span data-ttu-id="5cac9-135">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="5cac9-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="5cac9-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5cac9-136">vppTokenAccountType</span></span>|[<span data-ttu-id="5cac9-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5cac9-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="5cac9-p103">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。可取值为：`business`、`education`。可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="5cac9-p103">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with. The possible values are: `business`, `education`. The possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="5cac9-141">appleId</span><span class="sxs-lookup"><span data-stu-id="5cac9-141">appleId</span></span>|<span data-ttu-id="5cac9-142">字符串</span><span class="sxs-lookup"><span data-stu-id="5cac9-142">String</span></span>|<span data-ttu-id="5cac9-143">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="5cac9-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5cac9-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cac9-144">expirationDateTime</span></span>|<span data-ttu-id="5cac9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cac9-145">DateTimeOffset</span></span>|<span data-ttu-id="5cac9-146">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="5cac9-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5cac9-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5cac9-147">lastSyncDateTime</span></span>|<span data-ttu-id="5cac9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cac9-148">DateTimeOffset</span></span>|<span data-ttu-id="5cac9-149">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="5cac9-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5cac9-150">令牌</span><span class="sxs-lookup"><span data-stu-id="5cac9-150">token</span></span>|<span data-ttu-id="5cac9-151">字符串</span><span class="sxs-lookup"><span data-stu-id="5cac9-151">String</span></span>|<span data-ttu-id="5cac9-152">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="5cac9-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="5cac9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cac9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5cac9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cac9-154">DateTimeOffset</span></span>|<span data-ttu-id="5cac9-155">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="5cac9-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5cac9-156">state</span><span class="sxs-lookup"><span data-stu-id="5cac9-156">state</span></span>|[<span data-ttu-id="5cac9-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="5cac9-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="5cac9-p104">Apple Volume Purchase Program 令牌的当前状态。可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="5cac9-p104">Current state of the Apple Volume Purchase Program Token. The possible values are: `unknown`, `valid`, `expired`, `invalid`. The possible values are: `assignedToExternalMDM`, `unknown`, `valid`, `expired`.</span></span>|
|<span data-ttu-id="5cac9-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5cac9-161">lastSyncStatus</span></span>|[<span data-ttu-id="5cac9-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5cac9-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="5cac9-p105">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。可取值为：`none`、`inProgress`、`completed`、`failed`。可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="5cac9-p105">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token. The possible values are: `none`, `inProgress`, `completed`, `failed`. The possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="5cac9-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="5cac9-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="5cac9-167">布尔</span><span class="sxs-lookup"><span data-stu-id="5cac9-167">Boolean</span></span>|<span data-ttu-id="5cac9-168">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="5cac9-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="5cac9-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="5cac9-169">countryOrRegion</span></span>|<span data-ttu-id="5cac9-170">字符串</span><span class="sxs-lookup"><span data-stu-id="5cac9-170">String</span></span>|<span data-ttu-id="5cac9-171">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="5cac9-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="5cac9-172">响应</span><span class="sxs-lookup"><span data-stu-id="5cac9-172">Response</span></span>
<span data-ttu-id="5cac9-173">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [vppToken](../resources/intune_onboarding_vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cac9-173">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cac9-174">示例</span><span class="sxs-lookup"><span data-stu-id="5cac9-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cac9-175">请求</span><span class="sxs-lookup"><span data-stu-id="5cac9-175">Request</span></span>
<span data-ttu-id="5cac9-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cac9-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="5cac9-177">响应</span><span class="sxs-lookup"><span data-stu-id="5cac9-177">Response</span></span>
<span data-ttu-id="5cac9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cac9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```








