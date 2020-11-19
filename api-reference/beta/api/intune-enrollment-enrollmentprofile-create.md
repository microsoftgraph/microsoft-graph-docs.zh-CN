---
title: 创建 enrollmentProfile
description: 创建新的 enrollmentProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 244644720a8a8a76931a05a590baef666251d0c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263629"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="074b7-103">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="074b7-103">Create enrollmentProfile</span></span>

<span data-ttu-id="074b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="074b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="074b7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="074b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="074b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="074b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="074b7-107">创建新的 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="074b7-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="074b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="074b7-108">Prerequisites</span></span>
<span data-ttu-id="074b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="074b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="074b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="074b7-111">Permission type</span></span>|<span data-ttu-id="074b7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="074b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="074b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="074b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="074b7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="074b7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="074b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="074b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="074b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="074b7-116">Not supported.</span></span>|
|<span data-ttu-id="074b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="074b7-117">Application</span></span>|<span data-ttu-id="074b7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="074b7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="074b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="074b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="074b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="074b7-120">Request headers</span></span>
|<span data-ttu-id="074b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="074b7-121">Header</span></span>|<span data-ttu-id="074b7-122">值</span><span class="sxs-lookup"><span data-stu-id="074b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="074b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="074b7-123">Authorization</span></span>|<span data-ttu-id="074b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="074b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="074b7-125">接受</span><span class="sxs-lookup"><span data-stu-id="074b7-125">Accept</span></span>|<span data-ttu-id="074b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="074b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="074b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="074b7-127">Request body</span></span>
<span data-ttu-id="074b7-128">在请求正文中，提供 enrollmentProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="074b7-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="074b7-129">下表显示创建 enrollmentProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="074b7-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="074b7-130">属性</span><span class="sxs-lookup"><span data-stu-id="074b7-130">Property</span></span>|<span data-ttu-id="074b7-131">类型</span><span class="sxs-lookup"><span data-stu-id="074b7-131">Type</span></span>|<span data-ttu-id="074b7-132">说明</span><span class="sxs-lookup"><span data-stu-id="074b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="074b7-133">id</span><span class="sxs-lookup"><span data-stu-id="074b7-133">id</span></span>|<span data-ttu-id="074b7-134">String</span><span class="sxs-lookup"><span data-stu-id="074b7-134">String</span></span>|<span data-ttu-id="074b7-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="074b7-135">The GUID for the object</span></span>|
|<span data-ttu-id="074b7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="074b7-136">displayName</span></span>|<span data-ttu-id="074b7-137">String</span><span class="sxs-lookup"><span data-stu-id="074b7-137">String</span></span>|<span data-ttu-id="074b7-138">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="074b7-138">Name of the profile</span></span>|
|<span data-ttu-id="074b7-139">description</span><span class="sxs-lookup"><span data-stu-id="074b7-139">description</span></span>|<span data-ttu-id="074b7-140">String</span><span class="sxs-lookup"><span data-stu-id="074b7-140">String</span></span>|<span data-ttu-id="074b7-141">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="074b7-141">Description of the profile</span></span>|
|<span data-ttu-id="074b7-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="074b7-142">requiresUserAuthentication</span></span>|<span data-ttu-id="074b7-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="074b7-143">Boolean</span></span>|<span data-ttu-id="074b7-144">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="074b7-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="074b7-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="074b7-145">configurationEndpointUrl</span></span>|<span data-ttu-id="074b7-146">String</span><span class="sxs-lookup"><span data-stu-id="074b7-146">String</span></span>|<span data-ttu-id="074b7-147">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="074b7-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="074b7-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="074b7-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="074b7-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="074b7-149">Boolean</span></span>|<span data-ttu-id="074b7-150">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="074b7-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="074b7-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="074b7-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="074b7-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="074b7-152">Boolean</span></span>|<span data-ttu-id="074b7-153">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="074b7-153">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|



## <a name="response"></a><span data-ttu-id="074b7-154">响应</span><span class="sxs-lookup"><span data-stu-id="074b7-154">Response</span></span>
<span data-ttu-id="074b7-155">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="074b7-155">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="074b7-156">示例</span><span class="sxs-lookup"><span data-stu-id="074b7-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="074b7-157">请求</span><span class="sxs-lookup"><span data-stu-id="074b7-157">Request</span></span>
<span data-ttu-id="074b7-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="074b7-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="074b7-159">响应</span><span class="sxs-lookup"><span data-stu-id="074b7-159">Response</span></span>
<span data-ttu-id="074b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="074b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




