---
title: 更新 androidForWorkSettings
description: 更新 androidForWorkSettings 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7332cc22e32abd3722bb2331c721ef730f0b59b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401738"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="5cda6-103">更新 androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="5cda6-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="5cda6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5cda6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5cda6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5cda6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cda6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cda6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cda6-107">更新 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5cda6-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cda6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cda6-108">Prerequisites</span></span>
<span data-ttu-id="5cda6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5cda6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cda6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cda6-111">Permission type</span></span>|<span data-ttu-id="5cda6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5cda6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cda6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cda6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cda6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cda6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5cda6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cda6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cda6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cda6-116">Not supported.</span></span>|
|<span data-ttu-id="5cda6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cda6-117">Application</span></span>|<span data-ttu-id="5cda6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cda6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cda6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cda6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="5cda6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cda6-120">Request headers</span></span>
|<span data-ttu-id="5cda6-121">标头</span><span class="sxs-lookup"><span data-stu-id="5cda6-121">Header</span></span>|<span data-ttu-id="5cda6-122">值</span><span class="sxs-lookup"><span data-stu-id="5cda6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cda6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cda6-123">Authorization</span></span>|<span data-ttu-id="5cda6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cda6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cda6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5cda6-125">Accept</span></span>|<span data-ttu-id="5cda6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cda6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cda6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cda6-127">Request body</span></span>
<span data-ttu-id="5cda6-128">在请求正文中，提供 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cda6-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="5cda6-129">下表显示了创建 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5cda6-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="5cda6-130">属性</span><span class="sxs-lookup"><span data-stu-id="5cda6-130">Property</span></span>|<span data-ttu-id="5cda6-131">类型</span><span class="sxs-lookup"><span data-stu-id="5cda6-131">Type</span></span>|<span data-ttu-id="5cda6-132">说明</span><span class="sxs-lookup"><span data-stu-id="5cda6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cda6-133">id</span><span class="sxs-lookup"><span data-stu-id="5cda6-133">id</span></span>|<span data-ttu-id="5cda6-134">String</span><span class="sxs-lookup"><span data-stu-id="5cda6-134">String</span></span>|<span data-ttu-id="5cda6-135">Android for Work 设置标识符</span><span class="sxs-lookup"><span data-stu-id="5cda6-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="5cda6-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="5cda6-136">bindStatus</span></span>|[<span data-ttu-id="5cda6-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="5cda6-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="5cda6-138">将绑定使用 Google EMM API 的租户的状态。</span><span class="sxs-lookup"><span data-stu-id="5cda6-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="5cda6-139">可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。</span><span class="sxs-lookup"><span data-stu-id="5cda6-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="5cda6-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5cda6-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="5cda6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cda6-141">DateTimeOffset</span></span>|<span data-ttu-id="5cda6-142">应用同步的上次完成时间</span><span class="sxs-lookup"><span data-stu-id="5cda6-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="5cda6-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5cda6-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="5cda6-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5cda6-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="5cda6-145">最后一个应用程序同步结果。</span><span class="sxs-lookup"><span data-stu-id="5cda6-145">Last application sync result.</span></span> <span data-ttu-id="5cda6-146">可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="5cda6-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="5cda6-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5cda6-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="5cda6-148">String</span><span class="sxs-lookup"><span data-stu-id="5cda6-148">String</span></span>|<span data-ttu-id="5cda6-149">创建了企业的所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="5cda6-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="5cda6-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="5cda6-150">ownerOrganizationName</span></span>|<span data-ttu-id="5cda6-151">String</span><span class="sxs-lookup"><span data-stu-id="5cda6-151">String</span></span>|<span data-ttu-id="5cda6-152">载入 Android for Work 时使用的组织名称</span><span class="sxs-lookup"><span data-stu-id="5cda6-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="5cda6-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cda6-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5cda6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cda6-154">DateTimeOffset</span></span>|<span data-ttu-id="5cda6-155">Android for Work 设置的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="5cda6-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="5cda6-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="5cda6-156">enrollmentTarget</span></span>|[<span data-ttu-id="5cda6-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="5cda6-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="5cda6-158">指示哪些用户可以注册工作设备管理中 Android 设备。</span><span class="sxs-lookup"><span data-stu-id="5cda6-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="5cda6-159">可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="5cda6-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="5cda6-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="5cda6-160">targetGroupIds</span></span>|<span data-ttu-id="5cda6-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="5cda6-161">String collection</span></span>|<span data-ttu-id="5cda6-162">指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="5cda6-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="5cda6-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="5cda6-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="5cda6-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cda6-164">Boolean</span></span>|<span data-ttu-id="5cda6-165">指示是否此帐户 flighting 用于与 CloudDPC Android 设备所有者管理。</span><span class="sxs-lookup"><span data-stu-id="5cda6-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="5cda6-166">响应</span><span class="sxs-lookup"><span data-stu-id="5cda6-166">Response</span></span>
<span data-ttu-id="5cda6-167">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cda6-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cda6-168">示例</span><span class="sxs-lookup"><span data-stu-id="5cda6-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cda6-169">请求</span><span class="sxs-lookup"><span data-stu-id="5cda6-169">Request</span></span>
<span data-ttu-id="5cda6-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cda6-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="5cda6-171">响应</span><span class="sxs-lookup"><span data-stu-id="5cda6-171">Response</span></span>
<span data-ttu-id="5cda6-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cda6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```




