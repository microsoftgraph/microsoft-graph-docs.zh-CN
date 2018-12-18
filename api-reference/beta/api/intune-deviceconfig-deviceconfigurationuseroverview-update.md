---
title: 更新 deviceConfigurationUserOverview
description: 更新 deviceConfigurationUserOverview 对象的属性。
author: tfitzmac
ms.openlocfilehash: 9aac0cc7c578ed281999391f4db88e29ee336cfc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311464"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="517bb-103">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="517bb-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="517bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="517bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="517bb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="517bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="517bb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="517bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="517bb-107">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="517bb-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="517bb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="517bb-108">Prerequisites</span></span>
<span data-ttu-id="517bb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="517bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="517bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="517bb-111">Permission type</span></span>|<span data-ttu-id="517bb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="517bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="517bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="517bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="517bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="517bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="517bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="517bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="517bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="517bb-116">Not supported.</span></span>|
|<span data-ttu-id="517bb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="517bb-117">Application</span></span>|<span data-ttu-id="517bb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="517bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="517bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="517bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="517bb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="517bb-120">Request headers</span></span>
|<span data-ttu-id="517bb-121">标头</span><span class="sxs-lookup"><span data-stu-id="517bb-121">Header</span></span>|<span data-ttu-id="517bb-122">值</span><span class="sxs-lookup"><span data-stu-id="517bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="517bb-123">授权</span><span class="sxs-lookup"><span data-stu-id="517bb-123">Authorization</span></span>|<span data-ttu-id="517bb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="517bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="517bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="517bb-125">Accept</span></span>|<span data-ttu-id="517bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="517bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="517bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="517bb-127">Request body</span></span>
<span data-ttu-id="517bb-128">在请求正文中，提供 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="517bb-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="517bb-129">下表显示创建 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="517bb-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="517bb-130">属性</span><span class="sxs-lookup"><span data-stu-id="517bb-130">Property</span></span>|<span data-ttu-id="517bb-131">类型</span><span class="sxs-lookup"><span data-stu-id="517bb-131">Type</span></span>|<span data-ttu-id="517bb-132">说明</span><span class="sxs-lookup"><span data-stu-id="517bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="517bb-133">id</span><span class="sxs-lookup"><span data-stu-id="517bb-133">id</span></span>|<span data-ttu-id="517bb-134">String</span><span class="sxs-lookup"><span data-stu-id="517bb-134">String</span></span>|<span data-ttu-id="517bb-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="517bb-135">Key of the entity.</span></span>|
|<span data-ttu-id="517bb-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="517bb-136">pendingCount</span></span>|<span data-ttu-id="517bb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-137">Int32</span></span>|<span data-ttu-id="517bb-138">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="517bb-138">Number of pending Users</span></span>|
|<span data-ttu-id="517bb-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="517bb-139">notApplicableCount</span></span>|<span data-ttu-id="517bb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-140">Int32</span></span>|<span data-ttu-id="517bb-141">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="517bb-141">Number of not applicable users</span></span>|
|<span data-ttu-id="517bb-142">successCount</span><span class="sxs-lookup"><span data-stu-id="517bb-142">successCount</span></span>|<span data-ttu-id="517bb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-143">Int32</span></span>|<span data-ttu-id="517bb-144">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="517bb-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="517bb-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="517bb-145">errorCount</span></span>|<span data-ttu-id="517bb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-146">Int32</span></span>|<span data-ttu-id="517bb-147">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="517bb-147">Number of error Users</span></span>|
|<span data-ttu-id="517bb-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="517bb-148">failedCount</span></span>|<span data-ttu-id="517bb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-149">Int32</span></span>|<span data-ttu-id="517bb-150">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="517bb-150">Number of failed Users</span></span>|
|<span data-ttu-id="517bb-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="517bb-151">conflictCount</span></span>|<span data-ttu-id="517bb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-152">Int32</span></span>|<span data-ttu-id="517bb-153">存在冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="517bb-153">Number of users in conflict</span></span>|
|<span data-ttu-id="517bb-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="517bb-154">lastUpdateDateTime</span></span>|<span data-ttu-id="517bb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="517bb-155">DateTimeOffset</span></span>|<span data-ttu-id="517bb-156">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="517bb-156">Last update time</span></span>|
|<span data-ttu-id="517bb-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="517bb-157">configurationVersion</span></span>|<span data-ttu-id="517bb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="517bb-158">Int32</span></span>|<span data-ttu-id="517bb-159">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="517bb-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="517bb-160">响应</span><span class="sxs-lookup"><span data-stu-id="517bb-160">Response</span></span>
<span data-ttu-id="517bb-161">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="517bb-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="517bb-162">示例</span><span class="sxs-lookup"><span data-stu-id="517bb-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="517bb-163">请求</span><span class="sxs-lookup"><span data-stu-id="517bb-163">Request</span></span>
<span data-ttu-id="517bb-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="517bb-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 236

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="517bb-165">响应</span><span class="sxs-lookup"><span data-stu-id="517bb-165">Response</span></span>
<span data-ttu-id="517bb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="517bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





