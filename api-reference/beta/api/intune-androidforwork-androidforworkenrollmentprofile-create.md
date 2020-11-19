---
title: 创建 androidForWorkEnrollmentProfile
description: 创建新的 androidForWorkEnrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff6a33bd42d9edcaff5fd39c2757337e71b32a1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255011"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="79885-103">创建 androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="79885-103">Create androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="79885-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79885-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79885-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79885-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79885-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79885-107">创建新的 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79885-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79885-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="79885-108">Prerequisites</span></span>
<span data-ttu-id="79885-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79885-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79885-111">Permission type</span></span>|<span data-ttu-id="79885-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79885-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79885-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79885-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79885-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79885-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79885-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79885-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79885-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="79885-116">Not supported.</span></span>|
|<span data-ttu-id="79885-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="79885-117">Application</span></span>|<span data-ttu-id="79885-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79885-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79885-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79885-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="79885-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="79885-120">Request headers</span></span>
|<span data-ttu-id="79885-121">标头</span><span class="sxs-lookup"><span data-stu-id="79885-121">Header</span></span>|<span data-ttu-id="79885-122">值</span><span class="sxs-lookup"><span data-stu-id="79885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79885-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79885-123">Authorization</span></span>|<span data-ttu-id="79885-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79885-125">接受</span><span class="sxs-lookup"><span data-stu-id="79885-125">Accept</span></span>|<span data-ttu-id="79885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79885-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79885-127">Request body</span></span>
<span data-ttu-id="79885-128">在请求正文中，提供 androidForWorkEnrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79885-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="79885-129">下表显示创建 androidForWorkEnrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79885-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="79885-130">属性</span><span class="sxs-lookup"><span data-stu-id="79885-130">Property</span></span>|<span data-ttu-id="79885-131">类型</span><span class="sxs-lookup"><span data-stu-id="79885-131">Type</span></span>|<span data-ttu-id="79885-132">描述</span><span class="sxs-lookup"><span data-stu-id="79885-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79885-133">accountId</span><span class="sxs-lookup"><span data-stu-id="79885-133">accountId</span></span>|<span data-ttu-id="79885-134">String</span><span class="sxs-lookup"><span data-stu-id="79885-134">String</span></span>|<span data-ttu-id="79885-135">注册配置文件隶属的租户 GUID。</span><span class="sxs-lookup"><span data-stu-id="79885-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="79885-136">id</span><span class="sxs-lookup"><span data-stu-id="79885-136">id</span></span>|<span data-ttu-id="79885-137">String</span><span class="sxs-lookup"><span data-stu-id="79885-137">String</span></span>|<span data-ttu-id="79885-138">注册配置文件的唯一 GUID。</span><span class="sxs-lookup"><span data-stu-id="79885-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="79885-139">displayName</span><span class="sxs-lookup"><span data-stu-id="79885-139">displayName</span></span>|<span data-ttu-id="79885-140">String</span><span class="sxs-lookup"><span data-stu-id="79885-140">String</span></span>|<span data-ttu-id="79885-141">注册配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="79885-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="79885-142">description</span><span class="sxs-lookup"><span data-stu-id="79885-142">description</span></span>|<span data-ttu-id="79885-143">String</span><span class="sxs-lookup"><span data-stu-id="79885-143">String</span></span>|<span data-ttu-id="79885-144">注册配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="79885-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="79885-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79885-145">createdDateTime</span></span>|<span data-ttu-id="79885-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79885-146">DateTimeOffset</span></span>|<span data-ttu-id="79885-147">注册配置文件的创建日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79885-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="79885-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79885-148">lastModifiedDateTime</span></span>|<span data-ttu-id="79885-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79885-149">DateTimeOffset</span></span>|<span data-ttu-id="79885-150">上次修改注册配置文件的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79885-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="79885-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="79885-151">tokenValue</span></span>|<span data-ttu-id="79885-152">String</span><span class="sxs-lookup"><span data-stu-id="79885-152">String</span></span>|<span data-ttu-id="79885-153">为此注册配置文件最新创建的令牌的值。</span><span class="sxs-lookup"><span data-stu-id="79885-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="79885-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="79885-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="79885-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79885-155">DateTimeOffset</span></span>|<span data-ttu-id="79885-156">最新创建的令牌的到期日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79885-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="79885-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79885-157">enrolledDeviceCount</span></span>|<span data-ttu-id="79885-158">Int32</span><span class="sxs-lookup"><span data-stu-id="79885-158">Int32</span></span>|<span data-ttu-id="79885-159">已使用此注册配置文件进行注册的 Android 设备总数。</span><span class="sxs-lookup"><span data-stu-id="79885-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="79885-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="79885-160">qrCodeContent</span></span>|<span data-ttu-id="79885-161">String</span><span class="sxs-lookup"><span data-stu-id="79885-161">String</span></span>|<span data-ttu-id="79885-162">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="79885-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="79885-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="79885-163">qrCodeImage</span></span>|[<span data-ttu-id="79885-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79885-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79885-165">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="79885-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="79885-166">响应</span><span class="sxs-lookup"><span data-stu-id="79885-166">Response</span></span>
<span data-ttu-id="79885-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79885-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79885-168">示例</span><span class="sxs-lookup"><span data-stu-id="79885-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="79885-169">请求</span><span class="sxs-lookup"><span data-stu-id="79885-169">Request</span></span>
<span data-ttu-id="79885-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79885-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="79885-171">响应</span><span class="sxs-lookup"><span data-stu-id="79885-171">Response</span></span>
<span data-ttu-id="79885-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79885-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```




