---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 519114d38cb41ee6609f15e3d12ffa20c4437dbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466918"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="049e1-103">更新 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="049e1-103">Update depOnboardingSetting</span></span>

<span data-ttu-id="049e1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="049e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="049e1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="049e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="049e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="049e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="049e1-107">更新[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="049e1-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="049e1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="049e1-108">Prerequisites</span></span>
<span data-ttu-id="049e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="049e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="049e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="049e1-111">Permission type</span></span>|<span data-ttu-id="049e1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="049e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="049e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="049e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="049e1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049e1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="049e1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="049e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="049e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="049e1-116">Not supported.</span></span>|
|<span data-ttu-id="049e1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="049e1-117">Application</span></span>|<span data-ttu-id="049e1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="049e1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="049e1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="049e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="049e1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="049e1-120">Request headers</span></span>
|<span data-ttu-id="049e1-121">标头</span><span class="sxs-lookup"><span data-stu-id="049e1-121">Header</span></span>|<span data-ttu-id="049e1-122">值</span><span class="sxs-lookup"><span data-stu-id="049e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="049e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="049e1-123">Authorization</span></span>|<span data-ttu-id="049e1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="049e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="049e1-125">接受</span><span class="sxs-lookup"><span data-stu-id="049e1-125">Accept</span></span>|<span data-ttu-id="049e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="049e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="049e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="049e1-127">Request body</span></span>
<span data-ttu-id="049e1-128">在请求正文中，提供[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="049e1-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="049e1-129">下表显示创建[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="049e1-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="049e1-130">属性</span><span class="sxs-lookup"><span data-stu-id="049e1-130">Property</span></span>|<span data-ttu-id="049e1-131">类型</span><span class="sxs-lookup"><span data-stu-id="049e1-131">Type</span></span>|<span data-ttu-id="049e1-132">说明</span><span class="sxs-lookup"><span data-stu-id="049e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="049e1-133">id</span><span class="sxs-lookup"><span data-stu-id="049e1-133">id</span></span>|<span data-ttu-id="049e1-134">String</span><span class="sxs-lookup"><span data-stu-id="049e1-134">String</span></span>|<span data-ttu-id="049e1-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="049e1-135">UUID for the object</span></span>|
|<span data-ttu-id="049e1-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="049e1-136">appleIdentifier</span></span>|<span data-ttu-id="049e1-137">String</span><span class="sxs-lookup"><span data-stu-id="049e1-137">String</span></span>|<span data-ttu-id="049e1-138">用于获取当前令牌的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="049e1-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="049e1-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="049e1-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="049e1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="049e1-140">DateTimeOffset</span></span>|<span data-ttu-id="049e1-141">令牌将到期的时间。</span><span class="sxs-lookup"><span data-stu-id="049e1-141">When the token will expire.</span></span>|
|<span data-ttu-id="049e1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="049e1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="049e1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="049e1-143">DateTimeOffset</span></span>|<span data-ttu-id="049e1-144">在载入服务时。</span><span class="sxs-lookup"><span data-stu-id="049e1-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="049e1-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="049e1-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="049e1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="049e1-146">DateTimeOffset</span></span>|<span data-ttu-id="049e1-147">服务上次使用 Intune syned 时</span><span class="sxs-lookup"><span data-stu-id="049e1-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="049e1-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="049e1-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="049e1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="049e1-149">DateTimeOffset</span></span>|<span data-ttu-id="049e1-150">Intune 上次请求同步时。</span><span class="sxs-lookup"><span data-stu-id="049e1-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="049e1-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="049e1-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="049e1-152">布尔</span><span class="sxs-lookup"><span data-stu-id="049e1-152">Boolean</span></span>|<span data-ttu-id="049e1-153">是否启用了与学校数据同步服务的 Dep 令牌共享。</span><span class="sxs-lookup"><span data-stu-id="049e1-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="049e1-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="049e1-154">lastSyncErrorCode</span></span>|<span data-ttu-id="049e1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="049e1-155">Int32</span></span>|<span data-ttu-id="049e1-156">上一次 dep 同步期间 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="049e1-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="049e1-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="049e1-157">tokenType</span></span>|[<span data-ttu-id="049e1-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="049e1-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="049e1-159">获取或设置 Dep 令牌类型。</span><span class="sxs-lookup"><span data-stu-id="049e1-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="049e1-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="049e1-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="049e1-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="049e1-161">tokenName</span></span>|<span data-ttu-id="049e1-162">String</span><span class="sxs-lookup"><span data-stu-id="049e1-162">String</span></span>|<span data-ttu-id="049e1-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="049e1-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="049e1-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="049e1-164">syncedDeviceCount</span></span>|<span data-ttu-id="049e1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="049e1-165">Int32</span></span>|<span data-ttu-id="049e1-166">获取同步的设备计数</span><span class="sxs-lookup"><span data-stu-id="049e1-166">Gets synced device count</span></span>|
|<span data-ttu-id="049e1-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="049e1-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="049e1-168">布尔</span><span class="sxs-lookup"><span data-stu-id="049e1-168">Boolean</span></span>|<span data-ttu-id="049e1-169">为使用 Apple Dep 服务进行数据共享而授予的同意</span><span class="sxs-lookup"><span data-stu-id="049e1-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="049e1-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="049e1-170">roleScopeTagIds</span></span>|<span data-ttu-id="049e1-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="049e1-171">String collection</span></span>|<span data-ttu-id="049e1-172">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="049e1-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="049e1-173">响应</span><span class="sxs-lookup"><span data-stu-id="049e1-173">Response</span></span>
<span data-ttu-id="049e1-174">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="049e1-174">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="049e1-175">示例</span><span class="sxs-lookup"><span data-stu-id="049e1-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="049e1-176">请求</span><span class="sxs-lookup"><span data-stu-id="049e1-176">Request</span></span>
<span data-ttu-id="049e1-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="049e1-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="049e1-178">响应</span><span class="sxs-lookup"><span data-stu-id="049e1-178">Response</span></span>
<span data-ttu-id="049e1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="049e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





