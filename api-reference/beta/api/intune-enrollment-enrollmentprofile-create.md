---
title: 创建 enrollmentProfile
description: 创建新的 enrollmentProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4133e636cd9eedf7737e2003d1ba733a6e08ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934140"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="e6870-103">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e6870-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="e6870-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e6870-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6870-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e6870-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6870-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6870-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6870-107">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6870-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6870-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6870-108">Prerequisites</span></span>
<span data-ttu-id="e6870-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e6870-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6870-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6870-111">Permission type</span></span>|<span data-ttu-id="e6870-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6870-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6870-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6870-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6870-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6870-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6870-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6870-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6870-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6870-116">Not supported.</span></span>|
|<span data-ttu-id="e6870-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6870-117">Application</span></span>|<span data-ttu-id="e6870-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6870-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6870-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6870-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e6870-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6870-120">Request headers</span></span>
|<span data-ttu-id="e6870-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6870-121">Header</span></span>|<span data-ttu-id="e6870-122">值</span><span class="sxs-lookup"><span data-stu-id="e6870-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6870-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6870-123">Authorization</span></span>|<span data-ttu-id="e6870-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6870-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6870-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6870-125">Accept</span></span>|<span data-ttu-id="e6870-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6870-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6870-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6870-127">Request body</span></span>
<span data-ttu-id="e6870-128">在请求正文中，提供 enrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6870-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="e6870-129">下表显示时创建 enrollmentProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6870-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="e6870-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6870-130">Property</span></span>|<span data-ttu-id="e6870-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6870-131">Type</span></span>|<span data-ttu-id="e6870-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6870-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6870-133">id</span><span class="sxs-lookup"><span data-stu-id="e6870-133">id</span></span>|<span data-ttu-id="e6870-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e6870-134">String</span></span>|<span data-ttu-id="e6870-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="e6870-135">The GUID for the object</span></span>|
|<span data-ttu-id="e6870-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e6870-136">displayName</span></span>|<span data-ttu-id="e6870-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e6870-137">String</span></span>|<span data-ttu-id="e6870-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="e6870-138">Name of the profile</span></span>|
|<span data-ttu-id="e6870-139">说明</span><span class="sxs-lookup"><span data-stu-id="e6870-139">description</span></span>|<span data-ttu-id="e6870-140">字符串</span><span class="sxs-lookup"><span data-stu-id="e6870-140">String</span></span>|<span data-ttu-id="e6870-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="e6870-141">Description of the profile</span></span>|
|<span data-ttu-id="e6870-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e6870-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e6870-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6870-143">Boolean</span></span>|<span data-ttu-id="e6870-144">指示该配置文件是否要求用户身份验证</span><span class="sxs-lookup"><span data-stu-id="e6870-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="e6870-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e6870-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e6870-146">字符串</span><span class="sxs-lookup"><span data-stu-id="e6870-146">String</span></span>|<span data-ttu-id="e6870-147">配置用于注册的终结点 url</span><span class="sxs-lookup"><span data-stu-id="e6870-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="e6870-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e6870-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e6870-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6870-149">Boolean</span></span>|<span data-ttu-id="e6870-150">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e6870-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="e6870-151">响应</span><span class="sxs-lookup"><span data-stu-id="e6870-151">Response</span></span>
<span data-ttu-id="e6870-152">如果成功，此方法返回`201 Created`响应代码和响应正文中的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6870-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6870-153">示例</span><span class="sxs-lookup"><span data-stu-id="e6870-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6870-154">请求</span><span class="sxs-lookup"><span data-stu-id="e6870-154">Request</span></span>
<span data-ttu-id="e6870-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6870-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="e6870-156">响应</span><span class="sxs-lookup"><span data-stu-id="e6870-156">Response</span></span>
<span data-ttu-id="e6870-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6870-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





