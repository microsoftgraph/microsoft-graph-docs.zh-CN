---
title: 更新 androidForWorkSettings
description: 更新 androidForWorkSettings 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f71d9087b457189d3796306e0585981c0e58855
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498212"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="8203c-103">更新 androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="8203c-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="8203c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8203c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8203c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8203c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8203c-106">更新 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8203c-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8203c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8203c-107">Prerequisites</span></span>
<span data-ttu-id="8203c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8203c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8203c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8203c-110">Permission type</span></span>|<span data-ttu-id="8203c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8203c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8203c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8203c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8203c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8203c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8203c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8203c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8203c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8203c-115">Not supported.</span></span>|
|<span data-ttu-id="8203c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8203c-116">Application</span></span>|<span data-ttu-id="8203c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8203c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8203c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8203c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="8203c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8203c-119">Request headers</span></span>
|<span data-ttu-id="8203c-120">标头</span><span class="sxs-lookup"><span data-stu-id="8203c-120">Header</span></span>|<span data-ttu-id="8203c-121">值</span><span class="sxs-lookup"><span data-stu-id="8203c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8203c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8203c-122">Authorization</span></span>|<span data-ttu-id="8203c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8203c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8203c-124">接受</span><span class="sxs-lookup"><span data-stu-id="8203c-124">Accept</span></span>|<span data-ttu-id="8203c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8203c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8203c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8203c-126">Request body</span></span>
<span data-ttu-id="8203c-127">在请求正文中，提供 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8203c-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="8203c-128">下表显示了创建 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8203c-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="8203c-129">属性</span><span class="sxs-lookup"><span data-stu-id="8203c-129">Property</span></span>|<span data-ttu-id="8203c-130">类型</span><span class="sxs-lookup"><span data-stu-id="8203c-130">Type</span></span>|<span data-ttu-id="8203c-131">说明</span><span class="sxs-lookup"><span data-stu-id="8203c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8203c-132">id</span><span class="sxs-lookup"><span data-stu-id="8203c-132">id</span></span>|<span data-ttu-id="8203c-133">String</span><span class="sxs-lookup"><span data-stu-id="8203c-133">String</span></span>|<span data-ttu-id="8203c-134">Android for Work 设置标识符</span><span class="sxs-lookup"><span data-stu-id="8203c-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="8203c-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="8203c-135">bindStatus</span></span>|[<span data-ttu-id="8203c-136">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="8203c-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="8203c-137">使用 Google EMM API 的租户的绑定状态。</span><span class="sxs-lookup"><span data-stu-id="8203c-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="8203c-138">可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。</span><span class="sxs-lookup"><span data-stu-id="8203c-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="8203c-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8203c-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="8203c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8203c-140">DateTimeOffset</span></span>|<span data-ttu-id="8203c-141">应用同步的上次完成时间</span><span class="sxs-lookup"><span data-stu-id="8203c-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="8203c-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8203c-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="8203c-143">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8203c-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="8203c-144">上次应用程序同步结果。</span><span class="sxs-lookup"><span data-stu-id="8203c-144">Last application sync result.</span></span> <span data-ttu-id="8203c-145">可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="8203c-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="8203c-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8203c-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="8203c-147">字符串</span><span class="sxs-lookup"><span data-stu-id="8203c-147">String</span></span>|<span data-ttu-id="8203c-148">创建了企业的所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="8203c-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="8203c-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="8203c-149">ownerOrganizationName</span></span>|<span data-ttu-id="8203c-150">String</span><span class="sxs-lookup"><span data-stu-id="8203c-150">String</span></span>|<span data-ttu-id="8203c-151">载入 Android for Work 时使用的组织名称</span><span class="sxs-lookup"><span data-stu-id="8203c-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="8203c-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8203c-152">lastModifiedDateTime</span></span>|<span data-ttu-id="8203c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8203c-153">DateTimeOffset</span></span>|<span data-ttu-id="8203c-154">Android for Work 设置的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="8203c-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="8203c-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="8203c-155">enrollmentTarget</span></span>|[<span data-ttu-id="8203c-156">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="8203c-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="8203c-157">指示哪些用户可以在 Android for Work 设备管理中注册设备。</span><span class="sxs-lookup"><span data-stu-id="8203c-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="8203c-158">可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="8203c-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="8203c-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="8203c-159">targetGroupIds</span></span>|<span data-ttu-id="8203c-160">String collection</span><span class="sxs-lookup"><span data-stu-id="8203c-160">String collection</span></span>|<span data-ttu-id="8203c-161">指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="8203c-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="8203c-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="8203c-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="8203c-163">布尔</span><span class="sxs-lookup"><span data-stu-id="8203c-163">Boolean</span></span>|<span data-ttu-id="8203c-164">指示此帐户是否为使用 CloudDPC 的 Android 设备所有者管理 flighting。</span><span class="sxs-lookup"><span data-stu-id="8203c-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="8203c-165">响应</span><span class="sxs-lookup"><span data-stu-id="8203c-165">Response</span></span>
<span data-ttu-id="8203c-166">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8203c-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8203c-167">示例</span><span class="sxs-lookup"><span data-stu-id="8203c-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="8203c-168">请求</span><span class="sxs-lookup"><span data-stu-id="8203c-168">Request</span></span>
<span data-ttu-id="8203c-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8203c-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8203c-170">响应</span><span class="sxs-lookup"><span data-stu-id="8203c-170">Response</span></span>
<span data-ttu-id="8203c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8203c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





