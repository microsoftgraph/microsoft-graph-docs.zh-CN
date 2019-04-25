---
title: 创建 enrollmentProfile
description: 创建新的 enrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c78d5076038b85140d31e0e9000dda99f9dddff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533120"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="e4b55-103">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e4b55-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="e4b55-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4b55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4b55-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4b55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4b55-106">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4b55-106">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4b55-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4b55-107">Prerequisites</span></span>
<span data-ttu-id="e4b55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4b55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4b55-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4b55-110">Permission type</span></span>|<span data-ttu-id="e4b55-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4b55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4b55-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4b55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4b55-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4b55-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e4b55-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4b55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4b55-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4b55-115">Not supported.</span></span>|
|<span data-ttu-id="e4b55-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4b55-116">Application</span></span>|<span data-ttu-id="e4b55-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4b55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4b55-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4b55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e4b55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4b55-119">Request headers</span></span>
|<span data-ttu-id="e4b55-120">标头</span><span class="sxs-lookup"><span data-stu-id="e4b55-120">Header</span></span>|<span data-ttu-id="e4b55-121">值</span><span class="sxs-lookup"><span data-stu-id="e4b55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4b55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4b55-122">Authorization</span></span>|<span data-ttu-id="e4b55-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4b55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4b55-124">接受</span><span class="sxs-lookup"><span data-stu-id="e4b55-124">Accept</span></span>|<span data-ttu-id="e4b55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4b55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4b55-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4b55-126">Request body</span></span>
<span data-ttu-id="e4b55-127">在请求正文中, 提供 enrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4b55-127">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="e4b55-128">下表显示创建 enrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4b55-128">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="e4b55-129">属性</span><span class="sxs-lookup"><span data-stu-id="e4b55-129">Property</span></span>|<span data-ttu-id="e4b55-130">类型</span><span class="sxs-lookup"><span data-stu-id="e4b55-130">Type</span></span>|<span data-ttu-id="e4b55-131">说明</span><span class="sxs-lookup"><span data-stu-id="e4b55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b55-132">id</span><span class="sxs-lookup"><span data-stu-id="e4b55-132">id</span></span>|<span data-ttu-id="e4b55-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e4b55-133">String</span></span>|<span data-ttu-id="e4b55-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="e4b55-134">The GUID for the object</span></span>|
|<span data-ttu-id="e4b55-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e4b55-135">displayName</span></span>|<span data-ttu-id="e4b55-136">String</span><span class="sxs-lookup"><span data-stu-id="e4b55-136">String</span></span>|<span data-ttu-id="e4b55-137">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="e4b55-137">Name of the profile</span></span>|
|<span data-ttu-id="e4b55-138">description</span><span class="sxs-lookup"><span data-stu-id="e4b55-138">description</span></span>|<span data-ttu-id="e4b55-139">String</span><span class="sxs-lookup"><span data-stu-id="e4b55-139">String</span></span>|<span data-ttu-id="e4b55-140">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="e4b55-140">Description of the profile</span></span>|
|<span data-ttu-id="e4b55-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e4b55-141">requiresUserAuthentication</span></span>|<span data-ttu-id="e4b55-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4b55-142">Boolean</span></span>|<span data-ttu-id="e4b55-143">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="e4b55-143">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="e4b55-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e4b55-144">configurationEndpointUrl</span></span>|<span data-ttu-id="e4b55-145">String</span><span class="sxs-lookup"><span data-stu-id="e4b55-145">String</span></span>|<span data-ttu-id="e4b55-146">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="e4b55-146">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="e4b55-147">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e4b55-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e4b55-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4b55-148">Boolean</span></span>|<span data-ttu-id="e4b55-149">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e4b55-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="e4b55-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e4b55-150">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e4b55-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4b55-151">Boolean</span></span>|<span data-ttu-id="e4b55-152">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="e4b55-152">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="e4b55-153">响应</span><span class="sxs-lookup"><span data-stu-id="e4b55-153">Response</span></span>
<span data-ttu-id="e4b55-154">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4b55-154">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4b55-155">示例</span><span class="sxs-lookup"><span data-stu-id="e4b55-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4b55-156">请求</span><span class="sxs-lookup"><span data-stu-id="e4b55-156">Request</span></span>
<span data-ttu-id="e4b55-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4b55-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="e4b55-158">响应</span><span class="sxs-lookup"><span data-stu-id="e4b55-158">Response</span></span>
<span data-ttu-id="e4b55-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4b55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





