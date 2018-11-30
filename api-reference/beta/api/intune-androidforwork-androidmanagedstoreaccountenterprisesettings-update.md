---
title: 更新 androidManagedStoreAccountEnterpriseSettings
description: 更新 androidManagedStoreAccountEnterpriseSettings 对象的属性。
ms.openlocfilehash: 383c9225076e9e68e9b34d89b7fe904ccf747224
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044585"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="a9cda-103">更新 androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="a9cda-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="a9cda-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a9cda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9cda-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a9cda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9cda-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a9cda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9cda-107">更新[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a9cda-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9cda-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9cda-108">Prerequisites</span></span>
<span data-ttu-id="a9cda-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a9cda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9cda-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9cda-111">Permission type</span></span>|<span data-ttu-id="a9cda-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9cda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9cda-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9cda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9cda-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9cda-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9cda-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9cda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9cda-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9cda-116">Not supported.</span></span>|
|<span data-ttu-id="a9cda-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9cda-117">Application</span></span>|<span data-ttu-id="a9cda-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9cda-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9cda-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9cda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="a9cda-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9cda-120">Request headers</span></span>
|<span data-ttu-id="a9cda-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9cda-121">Header</span></span>|<span data-ttu-id="a9cda-122">值</span><span class="sxs-lookup"><span data-stu-id="a9cda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9cda-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9cda-123">Authorization</span></span>|<span data-ttu-id="a9cda-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9cda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9cda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9cda-125">Accept</span></span>|<span data-ttu-id="a9cda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9cda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9cda-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9cda-127">Request body</span></span>
<span data-ttu-id="a9cda-128">在请求正文中，提供[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9cda-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="a9cda-129">下表显示时创建[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9cda-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="a9cda-130">属性</span><span class="sxs-lookup"><span data-stu-id="a9cda-130">Property</span></span>|<span data-ttu-id="a9cda-131">类型</span><span class="sxs-lookup"><span data-stu-id="a9cda-131">Type</span></span>|<span data-ttu-id="a9cda-132">说明</span><span class="sxs-lookup"><span data-stu-id="a9cda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9cda-133">id</span><span class="sxs-lookup"><span data-stu-id="a9cda-133">id</span></span>|<span data-ttu-id="a9cda-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a9cda-134">String</span></span>|<span data-ttu-id="a9cda-135">Android 存储帐户企业设置标识符</span><span class="sxs-lookup"><span data-stu-id="a9cda-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="a9cda-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="a9cda-136">bindStatus</span></span>|[<span data-ttu-id="a9cda-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="a9cda-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="a9cda-138">将绑定使用 Google EMM API 的租户的状态。</span><span class="sxs-lookup"><span data-stu-id="a9cda-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="a9cda-139">可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。</span><span class="sxs-lookup"><span data-stu-id="a9cda-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="a9cda-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9cda-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="a9cda-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9cda-141">DateTimeOffset</span></span>|<span data-ttu-id="a9cda-142">应用同步的上次完成时间</span><span class="sxs-lookup"><span data-stu-id="a9cda-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="a9cda-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a9cda-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="a9cda-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a9cda-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="a9cda-145">最后一个应用程序同步结果。</span><span class="sxs-lookup"><span data-stu-id="a9cda-145">Last application sync result.</span></span> <span data-ttu-id="a9cda-146">可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。</span><span class="sxs-lookup"><span data-stu-id="a9cda-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="a9cda-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9cda-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="a9cda-148">String</span><span class="sxs-lookup"><span data-stu-id="a9cda-148">String</span></span>|<span data-ttu-id="a9cda-149">创建了企业的所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="a9cda-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="a9cda-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a9cda-150">ownerOrganizationName</span></span>|<span data-ttu-id="a9cda-151">String</span><span class="sxs-lookup"><span data-stu-id="a9cda-151">String</span></span>|<span data-ttu-id="a9cda-152">何时使用组织名称入职培训 Android 企业</span><span class="sxs-lookup"><span data-stu-id="a9cda-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="a9cda-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9cda-153">lastModifiedDateTime</span></span>|<span data-ttu-id="a9cda-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9cda-154">DateTimeOffset</span></span>|<span data-ttu-id="a9cda-155">上次修改时间 Android 企业设置</span><span class="sxs-lookup"><span data-stu-id="a9cda-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="a9cda-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9cda-156">enrollmentTarget</span></span>|[<span data-ttu-id="a9cda-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9cda-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="a9cda-158">指示哪些用户可以注册 Android 企业设备管理的设备。</span><span class="sxs-lookup"><span data-stu-id="a9cda-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="a9cda-159">可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="a9cda-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="a9cda-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="a9cda-160">targetGroupIds</span></span>|<span data-ttu-id="a9cda-161">String 集合</span><span class="sxs-lookup"><span data-stu-id="a9cda-161">String collection</span></span>|<span data-ttu-id="a9cda-162">指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。</span><span class="sxs-lookup"><span data-stu-id="a9cda-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="a9cda-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="a9cda-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="a9cda-164">布尔</span><span class="sxs-lookup"><span data-stu-id="a9cda-164">Boolean</span></span>|<span data-ttu-id="a9cda-165">指示是否此帐户 flighting 用于与 CloudDPC Android 设备所有者管理。</span><span class="sxs-lookup"><span data-stu-id="a9cda-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="a9cda-166">响应</span><span class="sxs-lookup"><span data-stu-id="a9cda-166">Response</span></span>
<span data-ttu-id="a9cda-167">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a9cda-167">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9cda-168">示例</span><span class="sxs-lookup"><span data-stu-id="a9cda-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9cda-169">请求</span><span class="sxs-lookup"><span data-stu-id="a9cda-169">Request</span></span>
<span data-ttu-id="a9cda-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9cda-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 458

{
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

### <a name="response"></a><span data-ttu-id="a9cda-171">响应</span><span class="sxs-lookup"><span data-stu-id="a9cda-171">Response</span></span>
<span data-ttu-id="a9cda-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9cda-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  "deviceOwnerManagementEnabled": true
}
```





