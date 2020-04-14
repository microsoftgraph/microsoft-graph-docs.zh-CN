---
title: 更新 deviceConfigurationAssignment
description: 更新 deviceConfigurationAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a7b4df7f80499812fde6d717fca1a383704ce98
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433582"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="8db3a-103">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8db3a-103">Update deviceConfigurationAssignment</span></span>

<span data-ttu-id="8db3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8db3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8db3a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8db3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8db3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8db3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8db3a-107">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8db3a-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8db3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8db3a-108">Prerequisites</span></span>
<span data-ttu-id="8db3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8db3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8db3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8db3a-111">Permission type</span></span>|<span data-ttu-id="8db3a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8db3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8db3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8db3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8db3a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8db3a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8db3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8db3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8db3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8db3a-116">Not supported.</span></span>|
|<span data-ttu-id="8db3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8db3a-117">Application</span></span>|<span data-ttu-id="8db3a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8db3a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8db3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8db3a-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8db3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8db3a-120">Request headers</span></span>
|<span data-ttu-id="8db3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="8db3a-121">Header</span></span>|<span data-ttu-id="8db3a-122">值</span><span class="sxs-lookup"><span data-stu-id="8db3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8db3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8db3a-123">Authorization</span></span>|<span data-ttu-id="8db3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8db3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8db3a-125">接受</span><span class="sxs-lookup"><span data-stu-id="8db3a-125">Accept</span></span>|<span data-ttu-id="8db3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8db3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8db3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8db3a-127">Request body</span></span>
<span data-ttu-id="8db3a-128">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8db3a-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="8db3a-129">下表显示创建 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8db3a-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="8db3a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8db3a-130">Property</span></span>|<span data-ttu-id="8db3a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8db3a-131">Type</span></span>|<span data-ttu-id="8db3a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8db3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8db3a-133">id</span><span class="sxs-lookup"><span data-stu-id="8db3a-133">id</span></span>|<span data-ttu-id="8db3a-134">String</span><span class="sxs-lookup"><span data-stu-id="8db3a-134">String</span></span>|<span data-ttu-id="8db3a-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="8db3a-135">The key of the assignment.</span></span>|
|<span data-ttu-id="8db3a-136">target</span><span class="sxs-lookup"><span data-stu-id="8db3a-136">target</span></span>|[<span data-ttu-id="8db3a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8db3a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8db3a-138">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="8db3a-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="8db3a-139">source</span><span class="sxs-lookup"><span data-stu-id="8db3a-139">source</span></span>|[<span data-ttu-id="8db3a-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8db3a-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8db3a-141">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="8db3a-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="8db3a-142">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8db3a-142">This property is read-only.</span></span> <span data-ttu-id="8db3a-143">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="8db3a-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8db3a-144">sourceId</span><span class="sxs-lookup"><span data-stu-id="8db3a-144">sourceId</span></span>|<span data-ttu-id="8db3a-145">String</span><span class="sxs-lookup"><span data-stu-id="8db3a-145">String</span></span>|<span data-ttu-id="8db3a-146">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="8db3a-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="8db3a-147">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8db3a-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="8db3a-148">响应</span><span class="sxs-lookup"><span data-stu-id="8db3a-148">Response</span></span>
<span data-ttu-id="8db3a-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8db3a-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8db3a-150">示例</span><span class="sxs-lookup"><span data-stu-id="8db3a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8db3a-151">请求</span><span class="sxs-lookup"><span data-stu-id="8db3a-151">Request</span></span>
<span data-ttu-id="8db3a-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8db3a-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="8db3a-153">响应</span><span class="sxs-lookup"><span data-stu-id="8db3a-153">Response</span></span>
<span data-ttu-id="8db3a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8db3a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



