---
title: 创建 deviceConfigurationUserStatus
description: 创建新的 deviceConfigurationUserStatus 对象。
ms.openlocfilehash: 26cd6242558a8af1da665a2668e4cd07ddcd68b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048275"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="4a377-103">创建 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4a377-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="4a377-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a377-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a377-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a377-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a377-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4a377-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a377-107">创建新的 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a377-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a377-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a377-108">Prerequisites</span></span>
<span data-ttu-id="4a377-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4a377-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a377-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a377-111">Permission type</span></span>|<span data-ttu-id="4a377-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a377-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a377-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a377-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a377-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a377-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a377-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a377-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a377-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a377-116">Not supported.</span></span>|
|<span data-ttu-id="4a377-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a377-117">Application</span></span>|<span data-ttu-id="4a377-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a377-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a377-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a377-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4a377-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a377-120">Request headers</span></span>
|<span data-ttu-id="4a377-121">标头</span><span class="sxs-lookup"><span data-stu-id="4a377-121">Header</span></span>|<span data-ttu-id="4a377-122">值</span><span class="sxs-lookup"><span data-stu-id="4a377-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a377-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a377-123">Authorization</span></span>|<span data-ttu-id="4a377-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a377-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a377-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a377-125">Accept</span></span>|<span data-ttu-id="4a377-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a377-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a377-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a377-127">Request body</span></span>
<span data-ttu-id="4a377-128">在请求正文中，提供 deviceConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a377-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="4a377-129">下表显示创建 deviceConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4a377-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="4a377-130">属性</span><span class="sxs-lookup"><span data-stu-id="4a377-130">Property</span></span>|<span data-ttu-id="4a377-131">类型</span><span class="sxs-lookup"><span data-stu-id="4a377-131">Type</span></span>|<span data-ttu-id="4a377-132">说明</span><span class="sxs-lookup"><span data-stu-id="4a377-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a377-133">id</span><span class="sxs-lookup"><span data-stu-id="4a377-133">id</span></span>|<span data-ttu-id="4a377-134">String</span><span class="sxs-lookup"><span data-stu-id="4a377-134">String</span></span>|<span data-ttu-id="4a377-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4a377-135">Key of the entity.</span></span>|
|<span data-ttu-id="4a377-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a377-136">userDisplayName</span></span>|<span data-ttu-id="4a377-137">String</span><span class="sxs-lookup"><span data-stu-id="4a377-137">String</span></span>|<span data-ttu-id="4a377-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="4a377-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4a377-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4a377-139">devicesCount</span></span>|<span data-ttu-id="4a377-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4a377-140">Int32</span></span>|<span data-ttu-id="4a377-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="4a377-141">Devices count for that user.</span></span>|
|<span data-ttu-id="4a377-142">状态</span><span class="sxs-lookup"><span data-stu-id="4a377-142">status</span></span>|[<span data-ttu-id="4a377-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4a377-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4a377-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="4a377-144">Compliance status of the policy report.</span></span> <span data-ttu-id="4a377-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4a377-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4a377-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a377-146">lastReportedDateTime</span></span>|<span data-ttu-id="4a377-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a377-147">DateTimeOffset</span></span>|<span data-ttu-id="4a377-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="4a377-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4a377-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a377-149">userPrincipalName</span></span>|<span data-ttu-id="4a377-150">String</span><span class="sxs-lookup"><span data-stu-id="4a377-150">String</span></span>|<span data-ttu-id="4a377-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4a377-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4a377-152">响应</span><span class="sxs-lookup"><span data-stu-id="4a377-152">Response</span></span>
<span data-ttu-id="4a377-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a377-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a377-154">示例</span><span class="sxs-lookup"><span data-stu-id="4a377-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a377-155">请求</span><span class="sxs-lookup"><span data-stu-id="4a377-155">Request</span></span>
<span data-ttu-id="4a377-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a377-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4a377-157">响应</span><span class="sxs-lookup"><span data-stu-id="4a377-157">Response</span></span>
<span data-ttu-id="4a377-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a377-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





