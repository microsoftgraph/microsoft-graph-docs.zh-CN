---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6579d8fd1b350de425d850115ac0335559462315
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309581"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="82253-103">更新 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="82253-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="82253-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82253-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82253-106">更新[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82253-106">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82253-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="82253-107">Prerequisites</span></span>
<span data-ttu-id="82253-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82253-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82253-110">Permission type</span></span>|<span data-ttu-id="82253-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82253-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82253-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82253-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82253-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82253-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82253-115">Not supported.</span></span>|
|<span data-ttu-id="82253-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82253-116">Application</span></span>|<span data-ttu-id="82253-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82253-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82253-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="82253-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="82253-119">Request headers</span></span>
|<span data-ttu-id="82253-120">标头</span><span class="sxs-lookup"><span data-stu-id="82253-120">Header</span></span>|<span data-ttu-id="82253-121">值</span><span class="sxs-lookup"><span data-stu-id="82253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82253-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82253-122">Authorization</span></span>|<span data-ttu-id="82253-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82253-124">接受</span><span class="sxs-lookup"><span data-stu-id="82253-124">Accept</span></span>|<span data-ttu-id="82253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82253-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82253-126">Request body</span></span>
<span data-ttu-id="82253-127">在请求正文中, 提供[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82253-127">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="82253-128">下表显示创建[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82253-128">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="82253-129">属性</span><span class="sxs-lookup"><span data-stu-id="82253-129">Property</span></span>|<span data-ttu-id="82253-130">类型</span><span class="sxs-lookup"><span data-stu-id="82253-130">Type</span></span>|<span data-ttu-id="82253-131">说明</span><span class="sxs-lookup"><span data-stu-id="82253-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82253-132">id</span><span class="sxs-lookup"><span data-stu-id="82253-132">id</span></span>|<span data-ttu-id="82253-133">String</span><span class="sxs-lookup"><span data-stu-id="82253-133">String</span></span>|<span data-ttu-id="82253-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="82253-134">UUID for the object</span></span>|
|<span data-ttu-id="82253-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="82253-135">appleIdentifier</span></span>|<span data-ttu-id="82253-136">String</span><span class="sxs-lookup"><span data-stu-id="82253-136">String</span></span>|<span data-ttu-id="82253-137">用于获取当前令牌的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="82253-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="82253-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="82253-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="82253-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82253-139">DateTimeOffset</span></span>|<span data-ttu-id="82253-140">令牌将到期的时间。</span><span class="sxs-lookup"><span data-stu-id="82253-140">When the token will expire.</span></span>|
|<span data-ttu-id="82253-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82253-141">lastModifiedDateTime</span></span>|<span data-ttu-id="82253-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82253-142">DateTimeOffset</span></span>|<span data-ttu-id="82253-143">在载入服务时。</span><span class="sxs-lookup"><span data-stu-id="82253-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="82253-144">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="82253-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="82253-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82253-145">DateTimeOffset</span></span>|<span data-ttu-id="82253-146">服务上次使用 Intune syned 时</span><span class="sxs-lookup"><span data-stu-id="82253-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="82253-147">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="82253-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="82253-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82253-148">DateTimeOffset</span></span>|<span data-ttu-id="82253-149">Intune 上次请求同步时。</span><span class="sxs-lookup"><span data-stu-id="82253-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="82253-150">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="82253-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="82253-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="82253-151">Boolean</span></span>|<span data-ttu-id="82253-152">是否启用了与学校数据同步服务的 Dep 令牌共享。</span><span class="sxs-lookup"><span data-stu-id="82253-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="82253-153">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="82253-153">lastSyncErrorCode</span></span>|<span data-ttu-id="82253-154">Int32</span><span class="sxs-lookup"><span data-stu-id="82253-154">Int32</span></span>|<span data-ttu-id="82253-155">上一次 dep 同步期间 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="82253-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="82253-156">tokenType</span><span class="sxs-lookup"><span data-stu-id="82253-156">tokenType</span></span>|[<span data-ttu-id="82253-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="82253-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="82253-158">获取或设置 Dep 令牌类型。</span><span class="sxs-lookup"><span data-stu-id="82253-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="82253-159">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="82253-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="82253-160">tokenName</span><span class="sxs-lookup"><span data-stu-id="82253-160">tokenName</span></span>|<span data-ttu-id="82253-161">String</span><span class="sxs-lookup"><span data-stu-id="82253-161">String</span></span>|<span data-ttu-id="82253-162">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="82253-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="82253-163">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82253-163">syncedDeviceCount</span></span>|<span data-ttu-id="82253-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82253-164">Int32</span></span>|<span data-ttu-id="82253-165">获取同步的设备计数</span><span class="sxs-lookup"><span data-stu-id="82253-165">Gets synced device count</span></span>|
|<span data-ttu-id="82253-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="82253-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="82253-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="82253-167">Boolean</span></span>|<span data-ttu-id="82253-168">为使用 Apple Dep 服务进行数据共享而授予的同意</span><span class="sxs-lookup"><span data-stu-id="82253-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="82253-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82253-169">roleScopeTagIds</span></span>|<span data-ttu-id="82253-170">String collection</span><span class="sxs-lookup"><span data-stu-id="82253-170">String collection</span></span>|<span data-ttu-id="82253-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="82253-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="82253-172">响应</span><span class="sxs-lookup"><span data-stu-id="82253-172">Response</span></span>
<span data-ttu-id="82253-173">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82253-173">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82253-174">示例</span><span class="sxs-lookup"><span data-stu-id="82253-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="82253-175">请求</span><span class="sxs-lookup"><span data-stu-id="82253-175">Request</span></span>
<span data-ttu-id="82253-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82253-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="82253-177">响应</span><span class="sxs-lookup"><span data-stu-id="82253-177">Response</span></span>
<span data-ttu-id="82253-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82253-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






