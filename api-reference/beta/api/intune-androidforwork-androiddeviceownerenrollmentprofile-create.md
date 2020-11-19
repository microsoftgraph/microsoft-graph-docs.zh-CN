---
title: 创建 androidDeviceOwnerEnrollmentProfile
description: 创建新的 androidDeviceOwnerEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06e20735d0e6ba15328b7373a12769bd1895e6c4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255292"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="90ae5-103">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="90ae5-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="90ae5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90ae5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90ae5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90ae5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ae5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90ae5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ae5-107">创建新的 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90ae5-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90ae5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="90ae5-108">Prerequisites</span></span>
<span data-ttu-id="90ae5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90ae5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="90ae5-111">Permission type</span></span>|<span data-ttu-id="90ae5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90ae5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90ae5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90ae5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90ae5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ae5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90ae5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90ae5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90ae5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90ae5-116">Not supported.</span></span>|
|<span data-ttu-id="90ae5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="90ae5-117">Application</span></span>|<span data-ttu-id="90ae5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90ae5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90ae5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90ae5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="90ae5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90ae5-120">Request headers</span></span>
|<span data-ttu-id="90ae5-121">标头</span><span class="sxs-lookup"><span data-stu-id="90ae5-121">Header</span></span>|<span data-ttu-id="90ae5-122">值</span><span class="sxs-lookup"><span data-stu-id="90ae5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90ae5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90ae5-123">Authorization</span></span>|<span data-ttu-id="90ae5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90ae5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90ae5-125">接受</span><span class="sxs-lookup"><span data-stu-id="90ae5-125">Accept</span></span>|<span data-ttu-id="90ae5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90ae5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ae5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="90ae5-127">Request body</span></span>
<span data-ttu-id="90ae5-128">在请求正文中，提供 androidDeviceOwnerEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90ae5-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="90ae5-129">下表显示创建 androidDeviceOwnerEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90ae5-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="90ae5-130">属性</span><span class="sxs-lookup"><span data-stu-id="90ae5-130">Property</span></span>|<span data-ttu-id="90ae5-131">类型</span><span class="sxs-lookup"><span data-stu-id="90ae5-131">Type</span></span>|<span data-ttu-id="90ae5-132">描述</span><span class="sxs-lookup"><span data-stu-id="90ae5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ae5-133">accountId</span><span class="sxs-lookup"><span data-stu-id="90ae5-133">accountId</span></span>|<span data-ttu-id="90ae5-134">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-134">String</span></span>|<span data-ttu-id="90ae5-135">注册配置文件隶属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="90ae5-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="90ae5-136">id</span><span class="sxs-lookup"><span data-stu-id="90ae5-136">id</span></span>|<span data-ttu-id="90ae5-137">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-137">String</span></span>|<span data-ttu-id="90ae5-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="90ae5-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="90ae5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="90ae5-139">displayName</span></span>|<span data-ttu-id="90ae5-140">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-140">String</span></span>|<span data-ttu-id="90ae5-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="90ae5-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="90ae5-142">description</span><span class="sxs-lookup"><span data-stu-id="90ae5-142">description</span></span>|<span data-ttu-id="90ae5-143">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-143">String</span></span>|<span data-ttu-id="90ae5-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="90ae5-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="90ae5-145">enrollmentMode</span><span class="sxs-lookup"><span data-stu-id="90ae5-145">enrollmentMode</span></span>|[<span data-ttu-id="90ae5-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="90ae5-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="90ae5-147">使用此注册配置文件的设备的注册模式。</span><span class="sxs-lookup"><span data-stu-id="90ae5-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="90ae5-148">可取值为：`corporateOwnedDedicatedDevice`、`corporateOwnedFullyManaged`、`corporateOwnedWorkProfile`、`corporateOwnedAOSPUserlessDevice`。</span><span class="sxs-lookup"><span data-stu-id="90ae5-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`, `corporateOwnedAOSPUserlessDevice`.</span></span>|
|<span data-ttu-id="90ae5-149">enrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="90ae5-149">enrollmentTokenType</span></span>|[<span data-ttu-id="90ae5-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="90ae5-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="90ae5-151">注册配置文件的注册令牌类型。</span><span class="sxs-lookup"><span data-stu-id="90ae5-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="90ae5-152">可取值为：`default`、`corporateOwnedDedicatedDeviceWithAzureADSharedMode`。</span><span class="sxs-lookup"><span data-stu-id="90ae5-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="90ae5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90ae5-153">createdDateTime</span></span>|<span data-ttu-id="90ae5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ae5-154">DateTimeOffset</span></span>|<span data-ttu-id="90ae5-155">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90ae5-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="90ae5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90ae5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="90ae5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ae5-157">DateTimeOffset</span></span>|<span data-ttu-id="90ae5-158">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90ae5-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="90ae5-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="90ae5-159">tokenValue</span></span>|<span data-ttu-id="90ae5-160">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-160">String</span></span>|<span data-ttu-id="90ae5-161">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="90ae5-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="90ae5-162">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="90ae5-162">tokenCreationDateTime</span></span>|<span data-ttu-id="90ae5-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ae5-163">DateTimeOffset</span></span>|<span data-ttu-id="90ae5-164">创建最近创建的令牌的日期时间。</span><span class="sxs-lookup"><span data-stu-id="90ae5-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="90ae5-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="90ae5-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="90ae5-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90ae5-166">DateTimeOffset</span></span>|<span data-ttu-id="90ae5-167">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90ae5-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="90ae5-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="90ae5-168">enrolledDeviceCount</span></span>|<span data-ttu-id="90ae5-169">Int32</span><span class="sxs-lookup"><span data-stu-id="90ae5-169">Int32</span></span>|<span data-ttu-id="90ae5-170">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="90ae5-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="90ae5-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="90ae5-171">qrCodeContent</span></span>|<span data-ttu-id="90ae5-172">String</span><span class="sxs-lookup"><span data-stu-id="90ae5-172">String</span></span>|<span data-ttu-id="90ae5-173">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="90ae5-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="90ae5-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="90ae5-174">qrCodeImage</span></span>|[<span data-ttu-id="90ae5-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="90ae5-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="90ae5-176">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="90ae5-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="90ae5-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90ae5-177">roleScopeTagIds</span></span>|<span data-ttu-id="90ae5-178">String 集合</span><span class="sxs-lookup"><span data-stu-id="90ae5-178">String collection</span></span>|<span data-ttu-id="90ae5-179">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="90ae5-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="90ae5-180">响应</span><span class="sxs-lookup"><span data-stu-id="90ae5-180">Response</span></span>
<span data-ttu-id="90ae5-181">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90ae5-181">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90ae5-182">示例</span><span class="sxs-lookup"><span data-stu-id="90ae5-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="90ae5-183">请求</span><span class="sxs-lookup"><span data-stu-id="90ae5-183">Request</span></span>
<span data-ttu-id="90ae5-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90ae5-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 758

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="90ae5-185">响应</span><span class="sxs-lookup"><span data-stu-id="90ae5-185">Response</span></span>
<span data-ttu-id="90ae5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90ae5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




