# <a name="update-vpptoken"></a><span data-ttu-id="a20a5-101">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="a20a5-101">Update vppToken</span></span>

> <span data-ttu-id="a20a5-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a20a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a20a5-103">更新 [vppToken](../resources/intune_onboarding_vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a20a5-103">Update the properties of a [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a20a5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a20a5-104">Prerequisites</span></span>
<span data-ttu-id="a20a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a20a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a20a5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a20a5-107">Permission type</span></span>|<span data-ttu-id="a20a5-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a20a5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a20a5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a20a5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a20a5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a20a5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a20a5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a20a5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a20a5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a20a5-112">Not supported.</span></span>|
|<span data-ttu-id="a20a5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a20a5-113">Application</span></span>|<span data-ttu-id="a20a5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a20a5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a20a5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a20a5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="a20a5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a20a5-116">Request headers</span></span>
|<span data-ttu-id="a20a5-117">标头</span><span class="sxs-lookup"><span data-stu-id="a20a5-117">Header</span></span>|<span data-ttu-id="a20a5-118">值</span><span class="sxs-lookup"><span data-stu-id="a20a5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a20a5-119">授权</span><span class="sxs-lookup"><span data-stu-id="a20a5-119">Authorization</span></span>|<span data-ttu-id="a20a5-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a20a5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a20a5-121">接受</span><span class="sxs-lookup"><span data-stu-id="a20a5-121">Accept</span></span>|<span data-ttu-id="a20a5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a20a5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a20a5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a20a5-123">Request body</span></span>
<span data-ttu-id="a20a5-124">在请求正文中，提供 [vppToken](../resources/intune_onboarding_vpptoken.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a20a5-124">In the request body, supply a JSON representation for the [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>

<span data-ttu-id="a20a5-125">下表显示创建 [vppToken](../resources/intune_onboarding_vpptoken.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a20a5-125">The following table shows the properties that are required when you create the [vppToken](../resources/intune_onboarding_vpptoken.md).</span></span>

|<span data-ttu-id="a20a5-126">属性</span><span class="sxs-lookup"><span data-stu-id="a20a5-126">Property</span></span>|<span data-ttu-id="a20a5-127">类型</span><span class="sxs-lookup"><span data-stu-id="a20a5-127">Type</span></span>|<span data-ttu-id="a20a5-128">说明</span><span class="sxs-lookup"><span data-stu-id="a20a5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20a5-129">ID</span><span class="sxs-lookup"><span data-stu-id="a20a5-129">id</span></span>|<span data-ttu-id="a20a5-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a20a5-130">String</span></span>|<span data-ttu-id="a20a5-131">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="a20a5-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="a20a5-132">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="a20a5-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="a20a5-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="a20a5-133">organizationName</span></span>|<span data-ttu-id="a20a5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a20a5-134">String</span></span>|<span data-ttu-id="a20a5-135">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="a20a5-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a20a5-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a20a5-136">vppTokenAccountType</span></span>|[<span data-ttu-id="a20a5-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a20a5-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="a20a5-138">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="a20a5-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a20a5-139">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-139">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a20a5-140">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-140">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a20a5-141">appleId</span><span class="sxs-lookup"><span data-stu-id="a20a5-141">appleId</span></span>|<span data-ttu-id="a20a5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a20a5-142">String</span></span>|<span data-ttu-id="a20a5-143">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a20a5-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a20a5-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a20a5-144">expirationDateTime</span></span>|<span data-ttu-id="a20a5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20a5-145">DateTimeOffset</span></span>|<span data-ttu-id="a20a5-146">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="a20a5-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a20a5-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a20a5-147">lastSyncDateTime</span></span>|<span data-ttu-id="a20a5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20a5-148">DateTimeOffset</span></span>|<span data-ttu-id="a20a5-149">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="a20a5-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a20a5-150">令牌</span><span class="sxs-lookup"><span data-stu-id="a20a5-150">token</span></span>|<span data-ttu-id="a20a5-151">字符串</span><span class="sxs-lookup"><span data-stu-id="a20a5-151">String</span></span>|<span data-ttu-id="a20a5-152">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="a20a5-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="a20a5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a20a5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="a20a5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20a5-154">DateTimeOffset</span></span>|<span data-ttu-id="a20a5-155">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="a20a5-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a20a5-156">状态</span><span class="sxs-lookup"><span data-stu-id="a20a5-156">state</span></span>|[<span data-ttu-id="a20a5-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="a20a5-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="a20a5-158">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a20a5-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a20a5-159">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-159">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="a20a5-160">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-160">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="a20a5-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a20a5-161">lastSyncStatus</span></span>|[<span data-ttu-id="a20a5-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a20a5-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="a20a5-163">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="a20a5-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a20a5-164">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-164">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="a20a5-165">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a20a5-165">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a20a5-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="a20a5-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="a20a5-167">布尔</span><span class="sxs-lookup"><span data-stu-id="a20a5-167">Boolean</span></span>|<span data-ttu-id="a20a5-168">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a20a5-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="a20a5-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a20a5-169">countryOrRegion</span></span>|<span data-ttu-id="a20a5-170">字符串</span><span class="sxs-lookup"><span data-stu-id="a20a5-170">String</span></span>|<span data-ttu-id="a20a5-171">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a20a5-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="a20a5-172">响应</span><span class="sxs-lookup"><span data-stu-id="a20a5-172">Response</span></span>
<span data-ttu-id="a20a5-173">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [vppToken](../resources/intune_onboarding_vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a20a5-173">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a20a5-174">示例</span><span class="sxs-lookup"><span data-stu-id="a20a5-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="a20a5-175">请求</span><span class="sxs-lookup"><span data-stu-id="a20a5-175">Request</span></span>
<span data-ttu-id="a20a5-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a20a5-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 478

{
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

### <a name="response"></a><span data-ttu-id="a20a5-177">响应</span><span class="sxs-lookup"><span data-stu-id="a20a5-177">Response</span></span>
<span data-ttu-id="a20a5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a20a5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








