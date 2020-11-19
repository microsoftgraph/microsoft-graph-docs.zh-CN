---
title: 更新 androidManagedStoreAccountEnterpriseSettings
description: 更新 androidManagedStoreAccountEnterpriseSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0216bc5fc529b940eb73313e928704b999b9fdd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254430"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="6282d-103">更新 androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="6282d-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

<span data-ttu-id="6282d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6282d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6282d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6282d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6282d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6282d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6282d-107">更新 [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6282d-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6282d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6282d-108">Prerequisites</span></span>
<span data-ttu-id="6282d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6282d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6282d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6282d-111">Permission type</span></span>|<span data-ttu-id="6282d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6282d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6282d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6282d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6282d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6282d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6282d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6282d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6282d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6282d-116">Not supported.</span></span>|
|<span data-ttu-id="6282d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6282d-117">Application</span></span>|<span data-ttu-id="6282d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6282d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6282d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6282d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="6282d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6282d-120">Request headers</span></span>
|<span data-ttu-id="6282d-121">标头</span><span class="sxs-lookup"><span data-stu-id="6282d-121">Header</span></span>|<span data-ttu-id="6282d-122">值</span><span class="sxs-lookup"><span data-stu-id="6282d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6282d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6282d-123">Authorization</span></span>|<span data-ttu-id="6282d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6282d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6282d-125">接受</span><span class="sxs-lookup"><span data-stu-id="6282d-125">Accept</span></span>|<span data-ttu-id="6282d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6282d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6282d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6282d-127">Request body</span></span>
<span data-ttu-id="6282d-128">在请求正文中，提供 [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6282d-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="6282d-129">下表显示创建 [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6282d-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="6282d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6282d-130">Property</span></span>|<span data-ttu-id="6282d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6282d-131">Type</span></span>|<span data-ttu-id="6282d-132">说明</span><span class="sxs-lookup"><span data-stu-id="6282d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6282d-133">id</span><span class="sxs-lookup"><span data-stu-id="6282d-133">id</span></span>|<span data-ttu-id="6282d-134">String</span><span class="sxs-lookup"><span data-stu-id="6282d-134">String</span></span>|<span data-ttu-id="6282d-135">Android 应用商店帐户企业设置标识符</span><span class="sxs-lookup"><span data-stu-id="6282d-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="6282d-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="6282d-136">bindStatus</span></span>|[<span data-ttu-id="6282d-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="6282d-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="6282d-138">使用 Google EMM API 的租户的绑定状态。</span><span class="sxs-lookup"><span data-stu-id="6282d-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="6282d-139">可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。</span><span class="sxs-lookup"><span data-stu-id="6282d-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="6282d-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6282d-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="6282d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6282d-141">DateTimeOffset</span></span>|<span data-ttu-id="6282d-142">应用同步的上次完成时间</span><span class="sxs-lookup"><span data-stu-id="6282d-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="6282d-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6282d-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="6282d-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6282d-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="6282d-145">上次应用程序同步结果。</span><span class="sxs-lookup"><span data-stu-id="6282d-145">Last application sync result.</span></span> <span data-ttu-id="6282d-146">可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="6282d-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="6282d-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6282d-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="6282d-148">String</span><span class="sxs-lookup"><span data-stu-id="6282d-148">String</span></span>|<span data-ttu-id="6282d-149">创建了企业的所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="6282d-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="6282d-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="6282d-150">ownerOrganizationName</span></span>|<span data-ttu-id="6282d-151">String</span><span class="sxs-lookup"><span data-stu-id="6282d-151">String</span></span>|<span data-ttu-id="6282d-152">在加入 Android 企业时使用的组织名称</span><span class="sxs-lookup"><span data-stu-id="6282d-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="6282d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6282d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="6282d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6282d-154">DateTimeOffset</span></span>|<span data-ttu-id="6282d-155">Android 企业版设置的上次修改时间</span><span class="sxs-lookup"><span data-stu-id="6282d-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="6282d-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="6282d-156">enrollmentTarget</span></span>|[<span data-ttu-id="6282d-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="6282d-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="6282d-158">指示哪些用户可以在 Android 企业版设备管理中注册设备。</span><span class="sxs-lookup"><span data-stu-id="6282d-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="6282d-159">可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="6282d-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="6282d-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="6282d-160">targetGroupIds</span></span>|<span data-ttu-id="6282d-161">String collection</span><span class="sxs-lookup"><span data-stu-id="6282d-161">String collection</span></span>|<span data-ttu-id="6282d-162">指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="6282d-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="6282d-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="6282d-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="6282d-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="6282d-164">Boolean</span></span>|<span data-ttu-id="6282d-165">指示此帐户是否为使用 CloudDPC 的 Android 设备所有者管理 flighting。</span><span class="sxs-lookup"><span data-stu-id="6282d-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="6282d-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="6282d-166">companyCodes</span></span>|<span data-ttu-id="6282d-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6282d-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="6282d-168">AndroidManagedStoreAccountEnterpriseSettings 的公司代码</span><span class="sxs-lookup"><span data-stu-id="6282d-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="6282d-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="6282d-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="6282d-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="6282d-170">Boolean</span></span>|<span data-ttu-id="6282d-171">AndroidManagedStoreAccountEnterpriseSettings 的公司代码</span><span class="sxs-lookup"><span data-stu-id="6282d-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="6282d-172">响应</span><span class="sxs-lookup"><span data-stu-id="6282d-172">Response</span></span>
<span data-ttu-id="6282d-173">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6282d-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6282d-174">示例</span><span class="sxs-lookup"><span data-stu-id="6282d-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="6282d-175">请求</span><span class="sxs-lookup"><span data-stu-id="6282d-175">Request</span></span>
<span data-ttu-id="6282d-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6282d-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="6282d-177">响应</span><span class="sxs-lookup"><span data-stu-id="6282d-177">Response</span></span>
<span data-ttu-id="6282d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6282d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
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
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```




