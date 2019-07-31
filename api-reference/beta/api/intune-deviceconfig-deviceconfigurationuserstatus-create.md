---
title: 创建 deviceConfigurationUserStatus
description: 创建新的 deviceConfigurationUserStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d33aa0fdcb33fd702678e8ddfb8faeaddcbdc18a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948941"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="2499c-103">创建 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="2499c-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="2499c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2499c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2499c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2499c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2499c-106">创建新的 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2499c-106">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2499c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2499c-107">Prerequisites</span></span>
<span data-ttu-id="2499c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2499c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2499c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2499c-110">Permission type</span></span>|<span data-ttu-id="2499c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2499c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2499c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2499c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2499c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2499c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2499c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2499c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2499c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2499c-115">Not supported.</span></span>|
|<span data-ttu-id="2499c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2499c-116">Application</span></span>|<span data-ttu-id="2499c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2499c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2499c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2499c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2499c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2499c-119">Request headers</span></span>
|<span data-ttu-id="2499c-120">标头</span><span class="sxs-lookup"><span data-stu-id="2499c-120">Header</span></span>|<span data-ttu-id="2499c-121">值</span><span class="sxs-lookup"><span data-stu-id="2499c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2499c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2499c-122">Authorization</span></span>|<span data-ttu-id="2499c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2499c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2499c-124">接受</span><span class="sxs-lookup"><span data-stu-id="2499c-124">Accept</span></span>|<span data-ttu-id="2499c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2499c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2499c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2499c-126">Request body</span></span>
<span data-ttu-id="2499c-127">在请求正文中，提供 deviceConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2499c-127">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="2499c-128">下表显示创建 deviceConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2499c-128">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="2499c-129">属性</span><span class="sxs-lookup"><span data-stu-id="2499c-129">Property</span></span>|<span data-ttu-id="2499c-130">类型</span><span class="sxs-lookup"><span data-stu-id="2499c-130">Type</span></span>|<span data-ttu-id="2499c-131">说明</span><span class="sxs-lookup"><span data-stu-id="2499c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2499c-132">id</span><span class="sxs-lookup"><span data-stu-id="2499c-132">id</span></span>|<span data-ttu-id="2499c-133">String</span><span class="sxs-lookup"><span data-stu-id="2499c-133">String</span></span>|<span data-ttu-id="2499c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2499c-134">Key of the entity.</span></span>|
|<span data-ttu-id="2499c-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2499c-135">userDisplayName</span></span>|<span data-ttu-id="2499c-136">String</span><span class="sxs-lookup"><span data-stu-id="2499c-136">String</span></span>|<span data-ttu-id="2499c-137">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="2499c-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2499c-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="2499c-138">devicesCount</span></span>|<span data-ttu-id="2499c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2499c-139">Int32</span></span>|<span data-ttu-id="2499c-140">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="2499c-140">Devices count for that user.</span></span>|
|<span data-ttu-id="2499c-141">status</span><span class="sxs-lookup"><span data-stu-id="2499c-141">status</span></span>|[<span data-ttu-id="2499c-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2499c-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2499c-143">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2499c-143">Compliance status of the policy report.</span></span> <span data-ttu-id="2499c-144">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2499c-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2499c-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2499c-145">lastReportedDateTime</span></span>|<span data-ttu-id="2499c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2499c-146">DateTimeOffset</span></span>|<span data-ttu-id="2499c-147">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="2499c-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2499c-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2499c-148">userPrincipalName</span></span>|<span data-ttu-id="2499c-149">字符串</span><span class="sxs-lookup"><span data-stu-id="2499c-149">String</span></span>|<span data-ttu-id="2499c-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2499c-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2499c-151">响应</span><span class="sxs-lookup"><span data-stu-id="2499c-151">Response</span></span>
<span data-ttu-id="2499c-152">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2499c-152">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2499c-153">示例</span><span class="sxs-lookup"><span data-stu-id="2499c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2499c-154">请求</span><span class="sxs-lookup"><span data-stu-id="2499c-154">Request</span></span>
<span data-ttu-id="2499c-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2499c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2499c-156">响应</span><span class="sxs-lookup"><span data-stu-id="2499c-156">Response</span></span>
<span data-ttu-id="2499c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2499c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





