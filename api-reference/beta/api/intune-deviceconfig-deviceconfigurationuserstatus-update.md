---
title: 更新 deviceConfigurationUserStatus
description: 更新 deviceConfigurationUserStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4209bfc0192471761dc83c549e1be8bad1f266ed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442983"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="c0905-103">更新 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c0905-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="c0905-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c0905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0905-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0905-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0905-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0905-107">更新 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0905-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0905-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0905-108">Prerequisites</span></span>
<span data-ttu-id="c0905-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0905-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0905-111">Permission type</span></span>|<span data-ttu-id="c0905-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0905-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0905-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0905-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0905-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0905-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0905-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0905-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0905-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0905-116">Not supported.</span></span>|
|<span data-ttu-id="c0905-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0905-117">Application</span></span>|<span data-ttu-id="c0905-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0905-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0905-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0905-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c0905-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0905-120">Request headers</span></span>
|<span data-ttu-id="c0905-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0905-121">Header</span></span>|<span data-ttu-id="c0905-122">值</span><span class="sxs-lookup"><span data-stu-id="c0905-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0905-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0905-123">Authorization</span></span>|<span data-ttu-id="c0905-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0905-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0905-125">接受</span><span class="sxs-lookup"><span data-stu-id="c0905-125">Accept</span></span>|<span data-ttu-id="c0905-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0905-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0905-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0905-127">Request body</span></span>
<span data-ttu-id="c0905-128">在请求正文中，提供 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0905-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="c0905-129">下表显示创建 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0905-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="c0905-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0905-130">Property</span></span>|<span data-ttu-id="c0905-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0905-131">Type</span></span>|<span data-ttu-id="c0905-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0905-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0905-133">id</span><span class="sxs-lookup"><span data-stu-id="c0905-133">id</span></span>|<span data-ttu-id="c0905-134">String</span><span class="sxs-lookup"><span data-stu-id="c0905-134">String</span></span>|<span data-ttu-id="c0905-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0905-135">Key of the entity.</span></span>|
|<span data-ttu-id="c0905-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c0905-136">userDisplayName</span></span>|<span data-ttu-id="c0905-137">String</span><span class="sxs-lookup"><span data-stu-id="c0905-137">String</span></span>|<span data-ttu-id="c0905-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="c0905-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c0905-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c0905-139">devicesCount</span></span>|<span data-ttu-id="c0905-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c0905-140">Int32</span></span>|<span data-ttu-id="c0905-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="c0905-141">Devices count for that user.</span></span>|
|<span data-ttu-id="c0905-142">status</span><span class="sxs-lookup"><span data-stu-id="c0905-142">status</span></span>|[<span data-ttu-id="c0905-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c0905-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c0905-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="c0905-144">Compliance status of the policy report.</span></span> <span data-ttu-id="c0905-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="c0905-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c0905-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0905-146">lastReportedDateTime</span></span>|<span data-ttu-id="c0905-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0905-147">DateTimeOffset</span></span>|<span data-ttu-id="c0905-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="c0905-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c0905-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0905-149">userPrincipalName</span></span>|<span data-ttu-id="c0905-150">字符串</span><span class="sxs-lookup"><span data-stu-id="c0905-150">String</span></span>|<span data-ttu-id="c0905-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="c0905-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c0905-152">响应</span><span class="sxs-lookup"><span data-stu-id="c0905-152">Response</span></span>
<span data-ttu-id="c0905-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0905-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0905-154">示例</span><span class="sxs-lookup"><span data-stu-id="c0905-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0905-155">请求</span><span class="sxs-lookup"><span data-stu-id="c0905-155">Request</span></span>
<span data-ttu-id="c0905-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0905-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="c0905-157">响应</span><span class="sxs-lookup"><span data-stu-id="c0905-157">Response</span></span>
<span data-ttu-id="c0905-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0905-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





