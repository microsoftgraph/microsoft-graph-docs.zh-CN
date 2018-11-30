---
title: 更新 enrollmentProfile
description: 更新 enrollmentProfile 对象的属性。
ms.openlocfilehash: 6d8d0b6650c1094f1d2c46ab197eeb1781e097d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047317"
---
# <a name="update-enrollmentprofile"></a><span data-ttu-id="316be-103">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="316be-103">Update enrollmentProfile</span></span>

> <span data-ttu-id="316be-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="316be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="316be-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="316be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="316be-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="316be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="316be-107">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="316be-107">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="316be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="316be-108">Prerequisites</span></span>
<span data-ttu-id="316be-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="316be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="316be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="316be-111">Permission type</span></span>|<span data-ttu-id="316be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="316be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="316be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="316be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="316be-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="316be-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="316be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="316be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="316be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="316be-116">Not supported.</span></span>|
|<span data-ttu-id="316be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="316be-117">Application</span></span>|<span data-ttu-id="316be-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="316be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="316be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="316be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="316be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="316be-120">Request headers</span></span>
|<span data-ttu-id="316be-121">标头</span><span class="sxs-lookup"><span data-stu-id="316be-121">Header</span></span>|<span data-ttu-id="316be-122">值</span><span class="sxs-lookup"><span data-stu-id="316be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="316be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="316be-123">Authorization</span></span>|<span data-ttu-id="316be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="316be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="316be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="316be-125">Accept</span></span>|<span data-ttu-id="316be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="316be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="316be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="316be-127">Request body</span></span>
<span data-ttu-id="316be-128">在请求正文中，提供[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="316be-128">In the request body, supply a JSON representation for the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

<span data-ttu-id="316be-129">下表显示时创建[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="316be-129">The following table shows the properties that are required when you create the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

|<span data-ttu-id="316be-130">属性</span><span class="sxs-lookup"><span data-stu-id="316be-130">Property</span></span>|<span data-ttu-id="316be-131">类型</span><span class="sxs-lookup"><span data-stu-id="316be-131">Type</span></span>|<span data-ttu-id="316be-132">说明</span><span class="sxs-lookup"><span data-stu-id="316be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="316be-133">id</span><span class="sxs-lookup"><span data-stu-id="316be-133">id</span></span>|<span data-ttu-id="316be-134">字符串</span><span class="sxs-lookup"><span data-stu-id="316be-134">String</span></span>|<span data-ttu-id="316be-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="316be-135">The GUID for the object</span></span>|
|<span data-ttu-id="316be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="316be-136">displayName</span></span>|<span data-ttu-id="316be-137">字符串</span><span class="sxs-lookup"><span data-stu-id="316be-137">String</span></span>|<span data-ttu-id="316be-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="316be-138">Name of the profile</span></span>|
|<span data-ttu-id="316be-139">说明</span><span class="sxs-lookup"><span data-stu-id="316be-139">description</span></span>|<span data-ttu-id="316be-140">字符串</span><span class="sxs-lookup"><span data-stu-id="316be-140">String</span></span>|<span data-ttu-id="316be-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="316be-141">Description of the profile</span></span>|
|<span data-ttu-id="316be-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="316be-142">requiresUserAuthentication</span></span>|<span data-ttu-id="316be-143">布尔</span><span class="sxs-lookup"><span data-stu-id="316be-143">Boolean</span></span>|<span data-ttu-id="316be-144">指示该配置文件是否要求用户身份验证</span><span class="sxs-lookup"><span data-stu-id="316be-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="316be-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="316be-145">configurationEndpointUrl</span></span>|<span data-ttu-id="316be-146">字符串</span><span class="sxs-lookup"><span data-stu-id="316be-146">String</span></span>|<span data-ttu-id="316be-147">配置用于注册的终结点 url</span><span class="sxs-lookup"><span data-stu-id="316be-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="316be-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="316be-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="316be-149">布尔</span><span class="sxs-lookup"><span data-stu-id="316be-149">Boolean</span></span>|<span data-ttu-id="316be-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="316be-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="316be-151">响应</span><span class="sxs-lookup"><span data-stu-id="316be-151">Response</span></span>
<span data-ttu-id="316be-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="316be-152">If successful, this method returns a `200 OK` response code and an updated [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="316be-153">示例</span><span class="sxs-lookup"><span data-stu-id="316be-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="316be-154">请求</span><span class="sxs-lookup"><span data-stu-id="316be-154">Request</span></span>
<span data-ttu-id="316be-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="316be-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 250

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="316be-156">响应</span><span class="sxs-lookup"><span data-stu-id="316be-156">Response</span></span>
<span data-ttu-id="316be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="316be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```





