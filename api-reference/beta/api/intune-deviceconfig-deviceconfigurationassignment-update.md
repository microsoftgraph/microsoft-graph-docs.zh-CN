---
title: 更新 deviceConfigurationAssignment
description: 更新 deviceConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b982b5007e9c9805914726476f76f9b770fa4920
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792973"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="ff179-103">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ff179-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="ff179-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff179-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff179-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff179-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff179-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff179-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff179-107">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff179-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff179-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff179-108">Prerequisites</span></span>
<span data-ttu-id="ff179-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ff179-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ff179-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff179-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff179-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff179-111">Permission type</span></span>|<span data-ttu-id="ff179-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff179-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff179-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff179-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff179-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff179-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff179-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff179-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff179-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff179-116">Not supported.</span></span>|
|<span data-ttu-id="ff179-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff179-117">Application</span></span>|<span data-ttu-id="ff179-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff179-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff179-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff179-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ff179-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff179-120">Request headers</span></span>
|<span data-ttu-id="ff179-121">标头</span><span class="sxs-lookup"><span data-stu-id="ff179-121">Header</span></span>|<span data-ttu-id="ff179-122">值</span><span class="sxs-lookup"><span data-stu-id="ff179-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff179-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff179-123">Authorization</span></span>|<span data-ttu-id="ff179-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff179-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff179-125">接受</span><span class="sxs-lookup"><span data-stu-id="ff179-125">Accept</span></span>|<span data-ttu-id="ff179-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff179-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff179-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff179-127">Request body</span></span>
<span data-ttu-id="ff179-128">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff179-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="ff179-129">下表显示创建 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff179-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="ff179-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff179-130">Property</span></span>|<span data-ttu-id="ff179-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff179-131">Type</span></span>|<span data-ttu-id="ff179-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff179-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff179-133">id</span><span class="sxs-lookup"><span data-stu-id="ff179-133">id</span></span>|<span data-ttu-id="ff179-134">String</span><span class="sxs-lookup"><span data-stu-id="ff179-134">String</span></span>|<span data-ttu-id="ff179-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="ff179-135">The key of the assignment.</span></span>|
|<span data-ttu-id="ff179-136">target</span><span class="sxs-lookup"><span data-stu-id="ff179-136">target</span></span>|[<span data-ttu-id="ff179-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff179-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff179-138">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="ff179-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="ff179-139">source</span><span class="sxs-lookup"><span data-stu-id="ff179-139">source</span></span>|[<span data-ttu-id="ff179-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="ff179-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="ff179-141">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="ff179-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="ff179-142">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ff179-142">This property is read-only.</span></span> <span data-ttu-id="ff179-143">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="ff179-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="ff179-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="ff179-144">sourceId</span></span>|<span data-ttu-id="ff179-145">String</span><span class="sxs-lookup"><span data-stu-id="ff179-145">String</span></span>|<span data-ttu-id="ff179-146">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="ff179-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="ff179-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ff179-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="ff179-148">响应</span><span class="sxs-lookup"><span data-stu-id="ff179-148">Response</span></span>
<span data-ttu-id="ff179-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff179-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff179-150">示例</span><span class="sxs-lookup"><span data-stu-id="ff179-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff179-151">请求</span><span class="sxs-lookup"><span data-stu-id="ff179-151">Request</span></span>
<span data-ttu-id="ff179-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff179-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
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

### <a name="response"></a><span data-ttu-id="ff179-153">响应</span><span class="sxs-lookup"><span data-stu-id="ff179-153">Response</span></span>
<span data-ttu-id="ff179-154">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ff179-154">Here is an example of the response.</span></span> <span data-ttu-id="ff179-155">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ff179-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ff179-156">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ff179-156">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



