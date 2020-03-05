---
title: 创建 depOnboardingSetting
description: 创建新的 depOnboardingSetting 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 971702dfab6c4782bfe314d4061fd5cbaccc3794
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467135"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="3d72f-103">创建 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="3d72f-103">Create depOnboardingSetting</span></span>

<span data-ttu-id="3d72f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3d72f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d72f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d72f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d72f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d72f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d72f-107">创建新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d72f-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d72f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d72f-108">Prerequisites</span></span>
<span data-ttu-id="3d72f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d72f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d72f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d72f-111">Permission type</span></span>|<span data-ttu-id="3d72f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d72f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d72f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d72f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d72f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d72f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d72f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d72f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d72f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d72f-116">Not supported.</span></span>|
|<span data-ttu-id="3d72f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d72f-117">Application</span></span>|<span data-ttu-id="3d72f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d72f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d72f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d72f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="3d72f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d72f-120">Request headers</span></span>
|<span data-ttu-id="3d72f-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d72f-121">Header</span></span>|<span data-ttu-id="3d72f-122">值</span><span class="sxs-lookup"><span data-stu-id="3d72f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d72f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d72f-123">Authorization</span></span>|<span data-ttu-id="3d72f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d72f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d72f-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d72f-125">Accept</span></span>|<span data-ttu-id="3d72f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d72f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d72f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d72f-127">Request body</span></span>
<span data-ttu-id="3d72f-128">在请求正文中，提供 depOnboardingSetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d72f-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="3d72f-129">下表显示创建 depOnboardingSetting 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d72f-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="3d72f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d72f-130">Property</span></span>|<span data-ttu-id="3d72f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d72f-131">Type</span></span>|<span data-ttu-id="3d72f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d72f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d72f-133">id</span><span class="sxs-lookup"><span data-stu-id="3d72f-133">id</span></span>|<span data-ttu-id="3d72f-134">String</span><span class="sxs-lookup"><span data-stu-id="3d72f-134">String</span></span>|<span data-ttu-id="3d72f-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="3d72f-135">UUID for the object</span></span>|
|<span data-ttu-id="3d72f-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d72f-136">appleIdentifier</span></span>|<span data-ttu-id="3d72f-137">String</span><span class="sxs-lookup"><span data-stu-id="3d72f-137">String</span></span>|<span data-ttu-id="3d72f-138">用于获取当前令牌的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="3d72f-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="3d72f-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d72f-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="3d72f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d72f-140">DateTimeOffset</span></span>|<span data-ttu-id="3d72f-141">令牌将到期的时间。</span><span class="sxs-lookup"><span data-stu-id="3d72f-141">When the token will expire.</span></span>|
|<span data-ttu-id="3d72f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d72f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3d72f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d72f-143">DateTimeOffset</span></span>|<span data-ttu-id="3d72f-144">在载入服务时。</span><span class="sxs-lookup"><span data-stu-id="3d72f-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="3d72f-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3d72f-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3d72f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d72f-146">DateTimeOffset</span></span>|<span data-ttu-id="3d72f-147">服务上次使用 Intune syned 时</span><span class="sxs-lookup"><span data-stu-id="3d72f-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="3d72f-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="3d72f-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="3d72f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d72f-149">DateTimeOffset</span></span>|<span data-ttu-id="3d72f-150">Intune 上次请求同步时。</span><span class="sxs-lookup"><span data-stu-id="3d72f-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="3d72f-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="3d72f-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="3d72f-152">布尔</span><span class="sxs-lookup"><span data-stu-id="3d72f-152">Boolean</span></span>|<span data-ttu-id="3d72f-153">是否启用了与学校数据同步服务的 Dep 令牌共享。</span><span class="sxs-lookup"><span data-stu-id="3d72f-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="3d72f-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="3d72f-154">lastSyncErrorCode</span></span>|<span data-ttu-id="3d72f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3d72f-155">Int32</span></span>|<span data-ttu-id="3d72f-156">上一次 dep 同步期间 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="3d72f-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="3d72f-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="3d72f-157">tokenType</span></span>|[<span data-ttu-id="3d72f-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="3d72f-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="3d72f-159">获取或设置 Dep 令牌类型。</span><span class="sxs-lookup"><span data-stu-id="3d72f-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="3d72f-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="3d72f-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="3d72f-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="3d72f-161">tokenName</span></span>|<span data-ttu-id="3d72f-162">String</span><span class="sxs-lookup"><span data-stu-id="3d72f-162">String</span></span>|<span data-ttu-id="3d72f-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="3d72f-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="3d72f-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3d72f-164">syncedDeviceCount</span></span>|<span data-ttu-id="3d72f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3d72f-165">Int32</span></span>|<span data-ttu-id="3d72f-166">获取同步的设备计数</span><span class="sxs-lookup"><span data-stu-id="3d72f-166">Gets synced device count</span></span>|
|<span data-ttu-id="3d72f-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="3d72f-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="3d72f-168">布尔</span><span class="sxs-lookup"><span data-stu-id="3d72f-168">Boolean</span></span>|<span data-ttu-id="3d72f-169">为使用 Apple Dep 服务进行数据共享而授予的同意</span><span class="sxs-lookup"><span data-stu-id="3d72f-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="3d72f-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d72f-170">roleScopeTagIds</span></span>|<span data-ttu-id="3d72f-171">String 集合</span><span class="sxs-lookup"><span data-stu-id="3d72f-171">String collection</span></span>|<span data-ttu-id="3d72f-172">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3d72f-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3d72f-173">响应</span><span class="sxs-lookup"><span data-stu-id="3d72f-173">Response</span></span>
<span data-ttu-id="3d72f-174">如果成功，此方法在响应`201 Created`正文中返回响应代码和[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3d72f-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d72f-175">示例</span><span class="sxs-lookup"><span data-stu-id="3d72f-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d72f-176">请求</span><span class="sxs-lookup"><span data-stu-id="3d72f-176">Request</span></span>
<span data-ttu-id="3d72f-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d72f-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3d72f-178">响应</span><span class="sxs-lookup"><span data-stu-id="3d72f-178">Response</span></span>
<span data-ttu-id="3d72f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d72f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





