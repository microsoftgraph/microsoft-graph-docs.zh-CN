---
title: 更新 enrollmentProfile
description: 更新 enrollmentProfile 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85cceaaaaa66822340539c38f6ab8ecde88eae1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400737"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="85208-103">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="85208-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="85208-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="85208-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85208-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85208-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85208-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85208-107">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85208-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85208-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85208-108">Prerequisites</span></span>
<span data-ttu-id="85208-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="85208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85208-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85208-111">Permission type</span></span>|<span data-ttu-id="85208-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85208-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85208-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85208-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85208-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85208-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85208-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85208-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85208-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85208-116">Not supported.</span></span>|
|<span data-ttu-id="85208-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85208-117">Application</span></span>|<span data-ttu-id="85208-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="85208-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85208-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85208-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="85208-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85208-120">Request headers</span></span>
|<span data-ttu-id="85208-121">标头</span><span class="sxs-lookup"><span data-stu-id="85208-121">Header</span></span>|<span data-ttu-id="85208-122">值</span><span class="sxs-lookup"><span data-stu-id="85208-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85208-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85208-123">Authorization</span></span>|<span data-ttu-id="85208-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85208-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85208-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85208-125">Accept</span></span>|<span data-ttu-id="85208-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85208-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85208-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85208-127">Request body</span></span>
<span data-ttu-id="85208-128">在请求正文中，提供[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85208-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="85208-129">下表显示时创建[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85208-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="85208-130">属性</span><span class="sxs-lookup"><span data-stu-id="85208-130">Property</span></span>|<span data-ttu-id="85208-131">类型</span><span class="sxs-lookup"><span data-stu-id="85208-131">Type</span></span>|<span data-ttu-id="85208-132">说明</span><span class="sxs-lookup"><span data-stu-id="85208-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85208-133">id</span><span class="sxs-lookup"><span data-stu-id="85208-133">id</span></span>|<span data-ttu-id="85208-134">String</span><span class="sxs-lookup"><span data-stu-id="85208-134">String</span></span>|<span data-ttu-id="85208-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="85208-135">The GUID for the object</span></span>|
|<span data-ttu-id="85208-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85208-136">displayName</span></span>|<span data-ttu-id="85208-137">String</span><span class="sxs-lookup"><span data-stu-id="85208-137">String</span></span>|<span data-ttu-id="85208-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="85208-138">Name of the profile</span></span>|
|<span data-ttu-id="85208-139">说明</span><span class="sxs-lookup"><span data-stu-id="85208-139">description</span></span>|<span data-ttu-id="85208-140">String</span><span class="sxs-lookup"><span data-stu-id="85208-140">String</span></span>|<span data-ttu-id="85208-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="85208-141">Description of the profile</span></span>|
|<span data-ttu-id="85208-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="85208-142">requiresUserAuthentication</span></span>|<span data-ttu-id="85208-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="85208-143">Boolean</span></span>|<span data-ttu-id="85208-144">指示该配置文件是否要求用户身份验证</span><span class="sxs-lookup"><span data-stu-id="85208-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="85208-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="85208-145">configurationEndpointUrl</span></span>|<span data-ttu-id="85208-146">String</span><span class="sxs-lookup"><span data-stu-id="85208-146">String</span></span>|<span data-ttu-id="85208-147">配置用于注册的终结点 url</span><span class="sxs-lookup"><span data-stu-id="85208-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="85208-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="85208-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="85208-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="85208-149">Boolean</span></span>|<span data-ttu-id="85208-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="85208-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="85208-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="85208-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="85208-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="85208-152">Boolean</span></span>|<span data-ttu-id="85208-153">表示安装程序注册的助手设备上必须的公司门户</span><span class="sxs-lookup"><span data-stu-id="85208-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="85208-154">响应</span><span class="sxs-lookup"><span data-stu-id="85208-154">Response</span></span>
<span data-ttu-id="85208-155">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85208-155">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85208-156">示例</span><span class="sxs-lookup"><span data-stu-id="85208-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="85208-157">请求</span><span class="sxs-lookup"><span data-stu-id="85208-157">Request</span></span>
<span data-ttu-id="85208-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85208-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85208-159">响应</span><span class="sxs-lookup"><span data-stu-id="85208-159">Response</span></span>
<span data-ttu-id="85208-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85208-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




