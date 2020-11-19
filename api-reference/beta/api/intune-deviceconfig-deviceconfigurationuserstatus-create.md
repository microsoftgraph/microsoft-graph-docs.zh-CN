---
title: 创建 deviceConfigurationUserStatus
description: 创建新的 deviceConfigurationUserStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abacfdab6ed7ca38ef608cd74733ca3494e24f69
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206460"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="12f17-103">创建 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="12f17-103">Create deviceConfigurationUserStatus</span></span>

<span data-ttu-id="12f17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12f17-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12f17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12f17-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12f17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12f17-107">创建新的 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12f17-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12f17-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12f17-108">Prerequisites</span></span>
<span data-ttu-id="12f17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12f17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12f17-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12f17-111">Permission type</span></span>|<span data-ttu-id="12f17-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12f17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12f17-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12f17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12f17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12f17-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12f17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12f17-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12f17-116">Not supported.</span></span>|
|<span data-ttu-id="12f17-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12f17-117">Application</span></span>|<span data-ttu-id="12f17-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12f17-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12f17-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12f17-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="12f17-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12f17-120">Request headers</span></span>
|<span data-ttu-id="12f17-121">标头</span><span class="sxs-lookup"><span data-stu-id="12f17-121">Header</span></span>|<span data-ttu-id="12f17-122">值</span><span class="sxs-lookup"><span data-stu-id="12f17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12f17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12f17-123">Authorization</span></span>|<span data-ttu-id="12f17-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12f17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12f17-125">接受</span><span class="sxs-lookup"><span data-stu-id="12f17-125">Accept</span></span>|<span data-ttu-id="12f17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12f17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12f17-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12f17-127">Request body</span></span>
<span data-ttu-id="12f17-128">在请求正文中，提供 deviceConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12f17-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="12f17-129">下表显示创建 deviceConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12f17-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="12f17-130">属性</span><span class="sxs-lookup"><span data-stu-id="12f17-130">Property</span></span>|<span data-ttu-id="12f17-131">类型</span><span class="sxs-lookup"><span data-stu-id="12f17-131">Type</span></span>|<span data-ttu-id="12f17-132">说明</span><span class="sxs-lookup"><span data-stu-id="12f17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f17-133">id</span><span class="sxs-lookup"><span data-stu-id="12f17-133">id</span></span>|<span data-ttu-id="12f17-134">String</span><span class="sxs-lookup"><span data-stu-id="12f17-134">String</span></span>|<span data-ttu-id="12f17-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12f17-135">Key of the entity.</span></span>|
|<span data-ttu-id="12f17-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="12f17-136">userDisplayName</span></span>|<span data-ttu-id="12f17-137">String</span><span class="sxs-lookup"><span data-stu-id="12f17-137">String</span></span>|<span data-ttu-id="12f17-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="12f17-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="12f17-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="12f17-139">devicesCount</span></span>|<span data-ttu-id="12f17-140">Int32</span><span class="sxs-lookup"><span data-stu-id="12f17-140">Int32</span></span>|<span data-ttu-id="12f17-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="12f17-141">Devices count for that user.</span></span>|
|<span data-ttu-id="12f17-142">status</span><span class="sxs-lookup"><span data-stu-id="12f17-142">status</span></span>|[<span data-ttu-id="12f17-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="12f17-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="12f17-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="12f17-144">Compliance status of the policy report.</span></span> <span data-ttu-id="12f17-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="12f17-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="12f17-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="12f17-146">lastReportedDateTime</span></span>|<span data-ttu-id="12f17-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f17-147">DateTimeOffset</span></span>|<span data-ttu-id="12f17-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="12f17-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="12f17-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12f17-149">userPrincipalName</span></span>|<span data-ttu-id="12f17-150">String</span><span class="sxs-lookup"><span data-stu-id="12f17-150">String</span></span>|<span data-ttu-id="12f17-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="12f17-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="12f17-152">响应</span><span class="sxs-lookup"><span data-stu-id="12f17-152">Response</span></span>
<span data-ttu-id="12f17-153">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12f17-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12f17-154">示例</span><span class="sxs-lookup"><span data-stu-id="12f17-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="12f17-155">请求</span><span class="sxs-lookup"><span data-stu-id="12f17-155">Request</span></span>
<span data-ttu-id="12f17-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12f17-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12f17-157">响应</span><span class="sxs-lookup"><span data-stu-id="12f17-157">Response</span></span>
<span data-ttu-id="12f17-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12f17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




