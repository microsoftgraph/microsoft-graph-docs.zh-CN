---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36e173595f1199000f912c3ba4ff8a96e99df8b9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135668"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="ec921-103">更新 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="ec921-103">Update depOnboardingSetting</span></span>

<span data-ttu-id="ec921-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec921-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec921-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec921-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec921-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec921-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec921-107">更新 [depOnboardingSetting 对象](../resources/intune-enrollment-deponboardingsetting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ec921-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec921-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec921-108">Prerequisites</span></span>
<span data-ttu-id="ec921-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec921-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec921-111">Permission type</span></span>|<span data-ttu-id="ec921-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec921-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec921-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec921-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec921-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec921-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ec921-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec921-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec921-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec921-116">Not supported.</span></span>|
|<span data-ttu-id="ec921-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec921-117">Application</span></span>|<span data-ttu-id="ec921-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec921-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec921-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec921-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="ec921-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec921-120">Request headers</span></span>
|<span data-ttu-id="ec921-121">标头</span><span class="sxs-lookup"><span data-stu-id="ec921-121">Header</span></span>|<span data-ttu-id="ec921-122">值</span><span class="sxs-lookup"><span data-stu-id="ec921-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec921-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec921-123">Authorization</span></span>|<span data-ttu-id="ec921-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec921-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec921-125">接受</span><span class="sxs-lookup"><span data-stu-id="ec921-125">Accept</span></span>|<span data-ttu-id="ec921-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec921-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec921-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec921-127">Request body</span></span>
<span data-ttu-id="ec921-128">在请求正文中，提供 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec921-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="ec921-129">下表显示创建 [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec921-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="ec921-130">属性</span><span class="sxs-lookup"><span data-stu-id="ec921-130">Property</span></span>|<span data-ttu-id="ec921-131">类型</span><span class="sxs-lookup"><span data-stu-id="ec921-131">Type</span></span>|<span data-ttu-id="ec921-132">说明</span><span class="sxs-lookup"><span data-stu-id="ec921-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec921-133">id</span><span class="sxs-lookup"><span data-stu-id="ec921-133">id</span></span>|<span data-ttu-id="ec921-134">String</span><span class="sxs-lookup"><span data-stu-id="ec921-134">String</span></span>|<span data-ttu-id="ec921-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="ec921-135">UUID for the object</span></span>|
|<span data-ttu-id="ec921-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec921-136">appleIdentifier</span></span>|<span data-ttu-id="ec921-137">String</span><span class="sxs-lookup"><span data-stu-id="ec921-137">String</span></span>|<span data-ttu-id="ec921-138">用于获取当前令牌的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ec921-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="ec921-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ec921-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="ec921-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec921-140">DateTimeOffset</span></span>|<span data-ttu-id="ec921-141">令牌将过期的时间。</span><span class="sxs-lookup"><span data-stu-id="ec921-141">When the token will expire.</span></span>|
|<span data-ttu-id="ec921-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec921-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ec921-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec921-143">DateTimeOffset</span></span>|<span data-ttu-id="ec921-144">载入服务时。</span><span class="sxs-lookup"><span data-stu-id="ec921-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="ec921-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ec921-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="ec921-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec921-146">DateTimeOffset</span></span>|<span data-ttu-id="ec921-147">服务最后一次与 Intune 进行联合时</span><span class="sxs-lookup"><span data-stu-id="ec921-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="ec921-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="ec921-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="ec921-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec921-149">DateTimeOffset</span></span>|<span data-ttu-id="ec921-150">Intune 上次请求同步时。</span><span class="sxs-lookup"><span data-stu-id="ec921-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="ec921-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="ec921-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="ec921-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec921-152">Boolean</span></span>|<span data-ttu-id="ec921-153">是否使用学校数据同步服务启用 Dep 令牌共享。</span><span class="sxs-lookup"><span data-stu-id="ec921-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="ec921-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="ec921-154">lastSyncErrorCode</span></span>|<span data-ttu-id="ec921-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ec921-155">Int32</span></span>|<span data-ttu-id="ec921-156">Apple 在上次取消同步期间报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ec921-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="ec921-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="ec921-157">tokenType</span></span>|[<span data-ttu-id="ec921-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="ec921-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="ec921-159">获取或设置 Dep 令牌类型。</span><span class="sxs-lookup"><span data-stu-id="ec921-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="ec921-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="ec921-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="ec921-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="ec921-161">tokenName</span></span>|<span data-ttu-id="ec921-162">String</span><span class="sxs-lookup"><span data-stu-id="ec921-162">String</span></span>|<span data-ttu-id="ec921-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="ec921-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="ec921-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ec921-164">syncedDeviceCount</span></span>|<span data-ttu-id="ec921-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ec921-165">Int32</span></span>|<span data-ttu-id="ec921-166">获取同步的设备计数</span><span class="sxs-lookup"><span data-stu-id="ec921-166">Gets synced device count</span></span>|
|<span data-ttu-id="ec921-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="ec921-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="ec921-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec921-168">Boolean</span></span>|<span data-ttu-id="ec921-169">同意与 Apple Dep 服务共享数据</span><span class="sxs-lookup"><span data-stu-id="ec921-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="ec921-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec921-170">roleScopeTagIds</span></span>|<span data-ttu-id="ec921-171">String collection</span><span class="sxs-lookup"><span data-stu-id="ec921-171">String collection</span></span>|<span data-ttu-id="ec921-172">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ec921-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="ec921-173">响应</span><span class="sxs-lookup"><span data-stu-id="ec921-173">Response</span></span>
<span data-ttu-id="ec921-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec921-174">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec921-175">示例</span><span class="sxs-lookup"><span data-stu-id="ec921-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec921-176">请求</span><span class="sxs-lookup"><span data-stu-id="ec921-176">Request</span></span>
<span data-ttu-id="ec921-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec921-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec921-178">响应</span><span class="sxs-lookup"><span data-stu-id="ec921-178">Response</span></span>
<span data-ttu-id="ec921-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec921-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




