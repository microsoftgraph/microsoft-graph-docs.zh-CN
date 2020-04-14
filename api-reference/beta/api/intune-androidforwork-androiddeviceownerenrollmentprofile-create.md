---
title: 创建 androidDeviceOwnerEnrollmentProfile
description: 创建新的 androidDeviceOwnerEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c02d06ca269da451112293e833ca2460e95fd3b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395993"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="96770-103">创建 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="96770-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="96770-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96770-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96770-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96770-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96770-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96770-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96770-107">创建新的[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96770-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96770-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="96770-108">Prerequisites</span></span>
<span data-ttu-id="96770-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96770-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96770-111">Permission type</span></span>|<span data-ttu-id="96770-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96770-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96770-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96770-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96770-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96770-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96770-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96770-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96770-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96770-116">Not supported.</span></span>|
|<span data-ttu-id="96770-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="96770-117">Application</span></span>|<span data-ttu-id="96770-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96770-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96770-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96770-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="96770-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="96770-120">Request headers</span></span>
|<span data-ttu-id="96770-121">标头</span><span class="sxs-lookup"><span data-stu-id="96770-121">Header</span></span>|<span data-ttu-id="96770-122">值</span><span class="sxs-lookup"><span data-stu-id="96770-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96770-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96770-123">Authorization</span></span>|<span data-ttu-id="96770-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96770-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96770-125">接受</span><span class="sxs-lookup"><span data-stu-id="96770-125">Accept</span></span>|<span data-ttu-id="96770-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96770-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96770-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="96770-127">Request body</span></span>
<span data-ttu-id="96770-128">在请求正文中，提供 androidDeviceOwnerEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96770-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="96770-129">下表显示创建 androidDeviceOwnerEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="96770-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="96770-130">属性</span><span class="sxs-lookup"><span data-stu-id="96770-130">Property</span></span>|<span data-ttu-id="96770-131">类型</span><span class="sxs-lookup"><span data-stu-id="96770-131">Type</span></span>|<span data-ttu-id="96770-132">说明</span><span class="sxs-lookup"><span data-stu-id="96770-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96770-133">accountId</span><span class="sxs-lookup"><span data-stu-id="96770-133">accountId</span></span>|<span data-ttu-id="96770-134">字符串</span><span class="sxs-lookup"><span data-stu-id="96770-134">String</span></span>|<span data-ttu-id="96770-135">注册配置文件隶属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="96770-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="96770-136">id</span><span class="sxs-lookup"><span data-stu-id="96770-136">id</span></span>|<span data-ttu-id="96770-137">字符串</span><span class="sxs-lookup"><span data-stu-id="96770-137">String</span></span>|<span data-ttu-id="96770-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="96770-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="96770-139">displayName</span><span class="sxs-lookup"><span data-stu-id="96770-139">displayName</span></span>|<span data-ttu-id="96770-140">字符串</span><span class="sxs-lookup"><span data-stu-id="96770-140">String</span></span>|<span data-ttu-id="96770-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="96770-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="96770-142">description</span><span class="sxs-lookup"><span data-stu-id="96770-142">description</span></span>|<span data-ttu-id="96770-143">String</span><span class="sxs-lookup"><span data-stu-id="96770-143">String</span></span>|<span data-ttu-id="96770-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="96770-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="96770-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96770-145">createdDateTime</span></span>|<span data-ttu-id="96770-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96770-146">DateTimeOffset</span></span>|<span data-ttu-id="96770-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="96770-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="96770-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96770-148">lastModifiedDateTime</span></span>|<span data-ttu-id="96770-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96770-149">DateTimeOffset</span></span>|<span data-ttu-id="96770-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="96770-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="96770-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="96770-151">tokenValue</span></span>|<span data-ttu-id="96770-152">字符串</span><span class="sxs-lookup"><span data-stu-id="96770-152">String</span></span>|<span data-ttu-id="96770-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="96770-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="96770-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="96770-154">tokenCreationDateTime</span></span>|<span data-ttu-id="96770-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96770-155">DateTimeOffset</span></span>|<span data-ttu-id="96770-156">创建最近创建的令牌的日期时间。</span><span class="sxs-lookup"><span data-stu-id="96770-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="96770-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="96770-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="96770-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96770-158">DateTimeOffset</span></span>|<span data-ttu-id="96770-159">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="96770-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="96770-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96770-160">enrolledDeviceCount</span></span>|<span data-ttu-id="96770-161">Int32</span><span class="sxs-lookup"><span data-stu-id="96770-161">Int32</span></span>|<span data-ttu-id="96770-162">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="96770-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="96770-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="96770-163">qrCodeContent</span></span>|<span data-ttu-id="96770-164">String</span><span class="sxs-lookup"><span data-stu-id="96770-164">String</span></span>|<span data-ttu-id="96770-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="96770-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="96770-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="96770-166">qrCodeImage</span></span>|[<span data-ttu-id="96770-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="96770-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="96770-168">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="96770-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="96770-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96770-169">roleScopeTagIds</span></span>|<span data-ttu-id="96770-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="96770-170">String collection</span></span>|<span data-ttu-id="96770-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="96770-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="96770-172">响应</span><span class="sxs-lookup"><span data-stu-id="96770-172">Response</span></span>
<span data-ttu-id="96770-173">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96770-173">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96770-174">示例</span><span class="sxs-lookup"><span data-stu-id="96770-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="96770-175">请求</span><span class="sxs-lookup"><span data-stu-id="96770-175">Request</span></span>
<span data-ttu-id="96770-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96770-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 627

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="96770-177">响应</span><span class="sxs-lookup"><span data-stu-id="96770-177">Response</span></span>
<span data-ttu-id="96770-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96770-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
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



