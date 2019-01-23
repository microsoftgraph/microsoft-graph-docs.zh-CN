---
title: 更新 depOnboardingSetting
description: 更新 depOnboardingSetting 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 78d3138950776dd74a055fbb00339e9e69b5f0f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412287"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="18db8-103">更新 depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="18db8-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="18db8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="18db8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18db8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="18db8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18db8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18db8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18db8-107">更新[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="18db8-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18db8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18db8-108">Prerequisites</span></span>
<span data-ttu-id="18db8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="18db8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18db8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18db8-111">Permission type</span></span>|<span data-ttu-id="18db8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18db8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18db8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18db8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18db8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18db8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18db8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18db8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18db8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18db8-116">Not supported.</span></span>|
|<span data-ttu-id="18db8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18db8-117">Application</span></span>|<span data-ttu-id="18db8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="18db8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18db8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18db8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="18db8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18db8-120">Request headers</span></span>
|<span data-ttu-id="18db8-121">标头</span><span class="sxs-lookup"><span data-stu-id="18db8-121">Header</span></span>|<span data-ttu-id="18db8-122">值</span><span class="sxs-lookup"><span data-stu-id="18db8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18db8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18db8-123">Authorization</span></span>|<span data-ttu-id="18db8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18db8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18db8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18db8-125">Accept</span></span>|<span data-ttu-id="18db8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18db8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18db8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18db8-127">Request body</span></span>
<span data-ttu-id="18db8-128">在请求正文中，提供[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18db8-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="18db8-129">下表显示时创建[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18db8-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="18db8-130">属性</span><span class="sxs-lookup"><span data-stu-id="18db8-130">Property</span></span>|<span data-ttu-id="18db8-131">类型</span><span class="sxs-lookup"><span data-stu-id="18db8-131">Type</span></span>|<span data-ttu-id="18db8-132">说明</span><span class="sxs-lookup"><span data-stu-id="18db8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18db8-133">id</span><span class="sxs-lookup"><span data-stu-id="18db8-133">id</span></span>|<span data-ttu-id="18db8-134">String</span><span class="sxs-lookup"><span data-stu-id="18db8-134">String</span></span>|<span data-ttu-id="18db8-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="18db8-135">UUID for the object</span></span>|
|<span data-ttu-id="18db8-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="18db8-136">appleIdentifier</span></span>|<span data-ttu-id="18db8-137">String</span><span class="sxs-lookup"><span data-stu-id="18db8-137">String</span></span>|<span data-ttu-id="18db8-138">Apple ID 用来获取当前的令牌。</span><span class="sxs-lookup"><span data-stu-id="18db8-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="18db8-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18db8-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="18db8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18db8-140">DateTimeOffset</span></span>|<span data-ttu-id="18db8-141">该令牌将过期时。</span><span class="sxs-lookup"><span data-stu-id="18db8-141">When the token will expire.</span></span>|
|<span data-ttu-id="18db8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18db8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="18db8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18db8-143">DateTimeOffset</span></span>|<span data-ttu-id="18db8-144">当该服务已 onboarded。</span><span class="sxs-lookup"><span data-stu-id="18db8-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="18db8-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="18db8-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="18db8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18db8-146">DateTimeOffset</span></span>|<span data-ttu-id="18db8-147">当服务与 Intune 的最后一个 syned</span><span class="sxs-lookup"><span data-stu-id="18db8-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="18db8-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="18db8-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="18db8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18db8-149">DateTimeOffset</span></span>|<span data-ttu-id="18db8-150">当 Intune 上次请求同步。</span><span class="sxs-lookup"><span data-stu-id="18db8-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="18db8-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="18db8-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="18db8-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="18db8-152">Boolean</span></span>|<span data-ttu-id="18db8-153">是否 Dep 令牌共享将启用学校数据同步服务。</span><span class="sxs-lookup"><span data-stu-id="18db8-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="18db8-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="18db8-154">lastSyncErrorCode</span></span>|<span data-ttu-id="18db8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="18db8-155">Int32</span></span>|<span data-ttu-id="18db8-156">在最后一个 dep 同步过程中由 Apple 报告的错误代码。</span><span class="sxs-lookup"><span data-stu-id="18db8-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="18db8-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="18db8-157">tokenType</span></span>|[<span data-ttu-id="18db8-158">depTokenType</span><span class="sxs-lookup"><span data-stu-id="18db8-158">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="18db8-159">获取或设置 Dep 标记类型。</span><span class="sxs-lookup"><span data-stu-id="18db8-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="18db8-160">可取值为：`none`、`dep`、`appleSchoolManager`。</span><span class="sxs-lookup"><span data-stu-id="18db8-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="18db8-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="18db8-161">tokenName</span></span>|<span data-ttu-id="18db8-162">String</span><span class="sxs-lookup"><span data-stu-id="18db8-162">String</span></span>|<span data-ttu-id="18db8-163">Dep 令牌的友好名称</span><span class="sxs-lookup"><span data-stu-id="18db8-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="18db8-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="18db8-164">syncedDeviceCount</span></span>|<span data-ttu-id="18db8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18db8-165">Int32</span></span>|<span data-ttu-id="18db8-166">获取同步设备计数</span><span class="sxs-lookup"><span data-stu-id="18db8-166">Gets synced device count</span></span>|
|<span data-ttu-id="18db8-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="18db8-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="18db8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="18db8-168">Boolean</span></span>|<span data-ttu-id="18db8-169">授予许可与 Apple Dep 服务共享的数据</span><span class="sxs-lookup"><span data-stu-id="18db8-169">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="18db8-170">响应</span><span class="sxs-lookup"><span data-stu-id="18db8-170">Response</span></span>
<span data-ttu-id="18db8-171">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="18db8-171">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18db8-172">示例</span><span class="sxs-lookup"><span data-stu-id="18db8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="18db8-173">请求</span><span class="sxs-lookup"><span data-stu-id="18db8-173">Request</span></span>
<span data-ttu-id="18db8-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18db8-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 514

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
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="18db8-175">响应</span><span class="sxs-lookup"><span data-stu-id="18db8-175">Response</span></span>
<span data-ttu-id="18db8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18db8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

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
  "dataSharingConsentGranted": true
}
```




