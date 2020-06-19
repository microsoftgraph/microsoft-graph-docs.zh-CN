---
title: 创建 deviceConfigurationAssignment
description: 创建新的 deviceConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b3406333441803bf7ac443ce8a4db1134f46bf5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793001"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="a57ca-103">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a57ca-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="a57ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a57ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a57ca-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a57ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a57ca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a57ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a57ca-107">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a57ca-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a57ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a57ca-108">Prerequisites</span></span>
<span data-ttu-id="a57ca-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a57ca-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a57ca-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a57ca-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a57ca-111">Permission type</span></span>|<span data-ttu-id="a57ca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a57ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a57ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a57ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a57ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a57ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a57ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a57ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a57ca-116">Not supported.</span></span>|
|<span data-ttu-id="a57ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a57ca-117">Application</span></span>|<span data-ttu-id="a57ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a57ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a57ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a57ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a57ca-120">Request headers</span></span>
|<span data-ttu-id="a57ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="a57ca-121">Header</span></span>|<span data-ttu-id="a57ca-122">值</span><span class="sxs-lookup"><span data-stu-id="a57ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a57ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a57ca-123">Authorization</span></span>|<span data-ttu-id="a57ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a57ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a57ca-125">接受</span><span class="sxs-lookup"><span data-stu-id="a57ca-125">Accept</span></span>|<span data-ttu-id="a57ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a57ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a57ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a57ca-127">Request body</span></span>
<span data-ttu-id="a57ca-128">在请求正文中，提供 deviceConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a57ca-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="a57ca-129">下表显示创建 deviceConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a57ca-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="a57ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="a57ca-130">Property</span></span>|<span data-ttu-id="a57ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="a57ca-131">Type</span></span>|<span data-ttu-id="a57ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="a57ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a57ca-133">id</span><span class="sxs-lookup"><span data-stu-id="a57ca-133">id</span></span>|<span data-ttu-id="a57ca-134">String</span><span class="sxs-lookup"><span data-stu-id="a57ca-134">String</span></span>|<span data-ttu-id="a57ca-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="a57ca-135">The key of the assignment.</span></span>|
|<span data-ttu-id="a57ca-136">target</span><span class="sxs-lookup"><span data-stu-id="a57ca-136">target</span></span>|[<span data-ttu-id="a57ca-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a57ca-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a57ca-138">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="a57ca-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="a57ca-139">source</span><span class="sxs-lookup"><span data-stu-id="a57ca-139">source</span></span>|[<span data-ttu-id="a57ca-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a57ca-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a57ca-141">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="a57ca-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="a57ca-142">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a57ca-142">This property is read-only.</span></span> <span data-ttu-id="a57ca-143">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="a57ca-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a57ca-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="a57ca-144">sourceId</span></span>|<span data-ttu-id="a57ca-145">String</span><span class="sxs-lookup"><span data-stu-id="a57ca-145">String</span></span>|<span data-ttu-id="a57ca-146">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="a57ca-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="a57ca-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a57ca-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="a57ca-148">响应</span><span class="sxs-lookup"><span data-stu-id="a57ca-148">Response</span></span>
<span data-ttu-id="a57ca-149">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a57ca-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a57ca-150">示例</span><span class="sxs-lookup"><span data-stu-id="a57ca-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a57ca-151">请求</span><span class="sxs-lookup"><span data-stu-id="a57ca-151">Request</span></span>
<span data-ttu-id="a57ca-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a57ca-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="a57ca-153">响应</span><span class="sxs-lookup"><span data-stu-id="a57ca-153">Response</span></span>
<span data-ttu-id="a57ca-154">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a57ca-154">Here is an example of the response.</span></span> <span data-ttu-id="a57ca-155">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a57ca-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a57ca-156">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a57ca-156">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



