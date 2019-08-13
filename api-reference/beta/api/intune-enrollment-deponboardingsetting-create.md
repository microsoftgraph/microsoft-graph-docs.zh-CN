---
title: 创建 depOnboardingSetting
description: 创建新的 depOnboardingSetting 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2e4b93373181462a4a2e73c4684ebe2599a6c75
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309672"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="8159a-103">创建 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="8159a-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="8159a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8159a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8159a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8159a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8159a-106">创建新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8159a-106">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8159a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8159a-107">Prerequisites</span></span>
<span data-ttu-id="8159a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8159a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8159a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8159a-110">Permission type</span></span>|<span data-ttu-id="8159a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8159a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8159a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8159a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8159a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8159a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8159a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8159a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8159a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8159a-115">Not supported.</span></span>|
|<span data-ttu-id="8159a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8159a-116">Application</span></span>|<span data-ttu-id="8159a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8159a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8159a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8159a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="8159a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8159a-119">Request headers</span></span>
|<span data-ttu-id="8159a-120">标头</span><span class="sxs-lookup"><span data-stu-id="8159a-120">Header</span></span>|<span data-ttu-id="8159a-121">值</span><span class="sxs-lookup"><span data-stu-id="8159a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8159a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8159a-122">Authorization</span></span>|<span data-ttu-id="8159a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8159a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8159a-124">接受</span><span class="sxs-lookup"><span data-stu-id="8159a-124">Accept</span></span>|<span data-ttu-id="8159a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8159a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8159a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8159a-126">Request body</span></span>
<span data-ttu-id="8159a-127">在请求正文中, 提供 depOnboardingSetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8159a-127">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="8159a-128">下表显示创建 depOnboardingSetting 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8159a-128">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="8159a-129">属性</span><span class="sxs-lookup"><span data-stu-id="8159a-129">Property</span></span>|<span data-ttu-id="8159a-130">类型</span><span class="sxs-lookup"><span data-stu-id="8159a-130">Type</span></span>|<span data-ttu-id="8159a-131">说明</span><span class="sxs-lookup"><span data-stu-id="8159a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8159a-132">id</span><span class="sxs-lookup"><span data-stu-id="8159a-132">id</span></span>|<span data-ttu-id="8159a-133">String</span><span class="sxs-lookup"><span data-stu-id="8159a-133">String</span></span>|<span data-ttu-id="8159a-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="8159a-134">UUID for the object</span></span>|
|<span data-ttu-id="8159a-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="8159a-135">appleIdentifier</span></span>|<span data-ttu-id="8159a-136">String</span><span class="sxs-lookup"><span data-stu-id="8159a-136">String</span></span>|<span data-ttu-id="8159a-137">用于获取当前令牌的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="8159a-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="8159a-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8159a-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="8159a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8159a-139">DateTimeOffset</span></span>|<span data-ttu-id="8159a-140">令牌将到期的时间。</span><span class="sxs-lookup"><span data-stu-id="8159a-140">When the token will expire.</span></span>|
|<span data-ttu-id="8159a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8159a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="8159a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8159a-142">DateTimeOffset</span></span>|<span data-ttu-id="8159a-143">在载入服务时。</span><span class="sxs-lookup"><span data-stu-id="8159a-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="8159a-144">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8159a-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="8159a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8159a-145">DateTimeOffset</span></span>|<span data-ttu-id="8159a-146">服务上次使用 Intune syned 时</span><span class="sxs-lookup"><span data-stu-id="8159a-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="8159a-147">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="8159a-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="8159a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8159a-148">DateTimeOffset</span></span>|<span data-ttu-id="8159a-149">Intune 上次请求同步时。</span><span class="sxs-lookup"><span data-stu-id="8159a-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="8159a-150">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="8159a-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="8159a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8159a-151">Boolean</span></span>|<span data-ttu-id="8159a-152">是否启用了与学校数据同步服务的 Dep 令牌共享。</span><span class="sxs-lookup"><span data-stu-id="8159a-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="8159a-153">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="8159a-153">lastSyncErrorCode</span></span>|<span data-ttu-id="8159a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8159a-154">Int32</span></span>|<span data-ttu-id="8159a-155">上一次 dep 同步期间 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="8159a-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="8159a-156">tokenType</span><span class="sxs-lookup"><span data-stu-id="8159a-156">tokenType</span></span>|[<span data-ttu-id="8159a-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="8159a-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="8159a-158">获取或设置 Dep 令牌类型。</span><span class="sxs-lookup"><span data-stu-id="8159a-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="8159a-159">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="8159a-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="8159a-160">tokenName</span><span class="sxs-lookup"><span data-stu-id="8159a-160">tokenName</span></span>|<span data-ttu-id="8159a-161">String</span><span class="sxs-lookup"><span data-stu-id="8159a-161">String</span></span>|<span data-ttu-id="8159a-162">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="8159a-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="8159a-163">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8159a-163">syncedDeviceCount</span></span>|<span data-ttu-id="8159a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8159a-164">Int32</span></span>|<span data-ttu-id="8159a-165">获取同步的设备计数</span><span class="sxs-lookup"><span data-stu-id="8159a-165">Gets synced device count</span></span>|
|<span data-ttu-id="8159a-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="8159a-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="8159a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="8159a-167">Boolean</span></span>|<span data-ttu-id="8159a-168">为使用 Apple Dep 服务进行数据共享而授予的同意</span><span class="sxs-lookup"><span data-stu-id="8159a-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="8159a-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8159a-169">roleScopeTagIds</span></span>|<span data-ttu-id="8159a-170">String collection</span><span class="sxs-lookup"><span data-stu-id="8159a-170">String collection</span></span>|<span data-ttu-id="8159a-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8159a-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8159a-172">响应</span><span class="sxs-lookup"><span data-stu-id="8159a-172">Response</span></span>
<span data-ttu-id="8159a-173">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8159a-173">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8159a-174">示例</span><span class="sxs-lookup"><span data-stu-id="8159a-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="8159a-175">请求</span><span class="sxs-lookup"><span data-stu-id="8159a-175">Request</span></span>
<span data-ttu-id="8159a-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8159a-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
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

### <a name="response"></a><span data-ttu-id="8159a-177">响应</span><span class="sxs-lookup"><span data-stu-id="8159a-177">Response</span></span>
<span data-ttu-id="8159a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8159a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






