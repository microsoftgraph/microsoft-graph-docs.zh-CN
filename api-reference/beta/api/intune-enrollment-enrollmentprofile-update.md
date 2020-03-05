---
title: 更新 enrollmentProfile
description: 更新 enrollmentProfile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 637760dbde82fc3d00bbfef0d9547b543c36ab38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466882"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="7091f-103">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="7091f-103">Update enrollmentProfile</span></span>

<span data-ttu-id="7091f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7091f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7091f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7091f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7091f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7091f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7091f-107">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7091f-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7091f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7091f-108">Prerequisites</span></span>
<span data-ttu-id="7091f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7091f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7091f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7091f-111">Permission type</span></span>|<span data-ttu-id="7091f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7091f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7091f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7091f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7091f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7091f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7091f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7091f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7091f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7091f-116">Not supported.</span></span>|
|<span data-ttu-id="7091f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7091f-117">Application</span></span>|<span data-ttu-id="7091f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7091f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7091f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7091f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="7091f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7091f-120">Request headers</span></span>
|<span data-ttu-id="7091f-121">标头</span><span class="sxs-lookup"><span data-stu-id="7091f-121">Header</span></span>|<span data-ttu-id="7091f-122">值</span><span class="sxs-lookup"><span data-stu-id="7091f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7091f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7091f-123">Authorization</span></span>|<span data-ttu-id="7091f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7091f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7091f-125">接受</span><span class="sxs-lookup"><span data-stu-id="7091f-125">Accept</span></span>|<span data-ttu-id="7091f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7091f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7091f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7091f-127">Request body</span></span>
<span data-ttu-id="7091f-128">在请求正文中，提供[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7091f-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="7091f-129">下表显示创建[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7091f-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="7091f-130">属性</span><span class="sxs-lookup"><span data-stu-id="7091f-130">Property</span></span>|<span data-ttu-id="7091f-131">类型</span><span class="sxs-lookup"><span data-stu-id="7091f-131">Type</span></span>|<span data-ttu-id="7091f-132">说明</span><span class="sxs-lookup"><span data-stu-id="7091f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7091f-133">id</span><span class="sxs-lookup"><span data-stu-id="7091f-133">id</span></span>|<span data-ttu-id="7091f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7091f-134">String</span></span>|<span data-ttu-id="7091f-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="7091f-135">The GUID for the object</span></span>|
|<span data-ttu-id="7091f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7091f-136">displayName</span></span>|<span data-ttu-id="7091f-137">String</span><span class="sxs-lookup"><span data-stu-id="7091f-137">String</span></span>|<span data-ttu-id="7091f-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="7091f-138">Name of the profile</span></span>|
|<span data-ttu-id="7091f-139">说明</span><span class="sxs-lookup"><span data-stu-id="7091f-139">description</span></span>|<span data-ttu-id="7091f-140">String</span><span class="sxs-lookup"><span data-stu-id="7091f-140">String</span></span>|<span data-ttu-id="7091f-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="7091f-141">Description of the profile</span></span>|
|<span data-ttu-id="7091f-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="7091f-142">requiresUserAuthentication</span></span>|<span data-ttu-id="7091f-143">布尔</span><span class="sxs-lookup"><span data-stu-id="7091f-143">Boolean</span></span>|<span data-ttu-id="7091f-144">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="7091f-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="7091f-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="7091f-145">configurationEndpointUrl</span></span>|<span data-ttu-id="7091f-146">String</span><span class="sxs-lookup"><span data-stu-id="7091f-146">String</span></span>|<span data-ttu-id="7091f-147">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="7091f-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="7091f-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="7091f-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="7091f-149">布尔</span><span class="sxs-lookup"><span data-stu-id="7091f-149">Boolean</span></span>|<span data-ttu-id="7091f-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="7091f-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="7091f-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="7091f-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="7091f-152">布尔</span><span class="sxs-lookup"><span data-stu-id="7091f-152">Boolean</span></span>|<span data-ttu-id="7091f-153">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="7091f-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="7091f-154">响应</span><span class="sxs-lookup"><span data-stu-id="7091f-154">Response</span></span>
<span data-ttu-id="7091f-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7091f-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7091f-156">示例</span><span class="sxs-lookup"><span data-stu-id="7091f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="7091f-157">请求</span><span class="sxs-lookup"><span data-stu-id="7091f-157">Request</span></span>
<span data-ttu-id="7091f-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7091f-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7091f-159">响应</span><span class="sxs-lookup"><span data-stu-id="7091f-159">Response</span></span>
<span data-ttu-id="7091f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7091f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





