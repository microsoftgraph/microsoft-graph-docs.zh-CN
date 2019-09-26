---
title: 更新 enrollmentProfile
description: 更新 enrollmentProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5a02d72a277cb973d92ba2d96bdecf1978f5e34
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185145"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="391de-103">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="391de-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="391de-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="391de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="391de-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="391de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="391de-106">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="391de-106">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="391de-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="391de-107">Prerequisites</span></span>
<span data-ttu-id="391de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="391de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="391de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="391de-110">Permission type</span></span>|<span data-ttu-id="391de-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="391de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="391de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="391de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="391de-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391de-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="391de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="391de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="391de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="391de-115">Not supported.</span></span>|
|<span data-ttu-id="391de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="391de-116">Application</span></span>|<span data-ttu-id="391de-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391de-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="391de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="391de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="391de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="391de-119">Request headers</span></span>
|<span data-ttu-id="391de-120">标头</span><span class="sxs-lookup"><span data-stu-id="391de-120">Header</span></span>|<span data-ttu-id="391de-121">值</span><span class="sxs-lookup"><span data-stu-id="391de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="391de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="391de-122">Authorization</span></span>|<span data-ttu-id="391de-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="391de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="391de-124">接受</span><span class="sxs-lookup"><span data-stu-id="391de-124">Accept</span></span>|<span data-ttu-id="391de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="391de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="391de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="391de-126">Request body</span></span>
<span data-ttu-id="391de-127">在请求正文中，提供[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="391de-127">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="391de-128">下表显示创建[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="391de-128">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="391de-129">属性</span><span class="sxs-lookup"><span data-stu-id="391de-129">Property</span></span>|<span data-ttu-id="391de-130">类型</span><span class="sxs-lookup"><span data-stu-id="391de-130">Type</span></span>|<span data-ttu-id="391de-131">说明</span><span class="sxs-lookup"><span data-stu-id="391de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="391de-132">id</span><span class="sxs-lookup"><span data-stu-id="391de-132">id</span></span>|<span data-ttu-id="391de-133">字符串</span><span class="sxs-lookup"><span data-stu-id="391de-133">String</span></span>|<span data-ttu-id="391de-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="391de-134">The GUID for the object</span></span>|
|<span data-ttu-id="391de-135">displayName</span><span class="sxs-lookup"><span data-stu-id="391de-135">displayName</span></span>|<span data-ttu-id="391de-136">String</span><span class="sxs-lookup"><span data-stu-id="391de-136">String</span></span>|<span data-ttu-id="391de-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="391de-137">Name of the profile</span></span>|
|<span data-ttu-id="391de-138">说明</span><span class="sxs-lookup"><span data-stu-id="391de-138">description</span></span>|<span data-ttu-id="391de-139">String</span><span class="sxs-lookup"><span data-stu-id="391de-139">String</span></span>|<span data-ttu-id="391de-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="391de-140">Description of the profile</span></span>|
|<span data-ttu-id="391de-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="391de-141">requiresUserAuthentication</span></span>|<span data-ttu-id="391de-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="391de-142">Boolean</span></span>|<span data-ttu-id="391de-143">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="391de-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="391de-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="391de-144">configurationEndpointUrl</span></span>|<span data-ttu-id="391de-145">String</span><span class="sxs-lookup"><span data-stu-id="391de-145">String</span></span>|<span data-ttu-id="391de-146">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="391de-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="391de-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="391de-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="391de-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="391de-148">Boolean</span></span>|<span data-ttu-id="391de-149">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="391de-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="391de-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="391de-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="391de-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="391de-151">Boolean</span></span>|<span data-ttu-id="391de-152">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="391de-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="391de-153">响应</span><span class="sxs-lookup"><span data-stu-id="391de-153">Response</span></span>
<span data-ttu-id="391de-154">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="391de-154">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="391de-155">示例</span><span class="sxs-lookup"><span data-stu-id="391de-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="391de-156">请求</span><span class="sxs-lookup"><span data-stu-id="391de-156">Request</span></span>
<span data-ttu-id="391de-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="391de-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 370

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```

### <a name="response"></a><span data-ttu-id="391de-158">响应</span><span class="sxs-lookup"><span data-stu-id="391de-158">Response</span></span>
<span data-ttu-id="391de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="391de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 419

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




