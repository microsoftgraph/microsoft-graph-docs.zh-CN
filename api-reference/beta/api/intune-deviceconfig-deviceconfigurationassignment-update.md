---
title: 更新 deviceConfigurationAssignment
description: 更新 deviceConfigurationAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc10b0b2f0500095e2d14333cf296270ca1bec70
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174856"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="bc433-103">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="bc433-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="bc433-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc433-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc433-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc433-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc433-106">更新 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc433-106">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc433-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc433-107">Prerequisites</span></span>
<span data-ttu-id="bc433-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc433-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc433-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc433-110">Permission type</span></span>|<span data-ttu-id="bc433-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc433-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc433-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc433-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc433-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc433-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc433-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc433-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc433-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc433-115">Not supported.</span></span>|
|<span data-ttu-id="bc433-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc433-116">Application</span></span>|<span data-ttu-id="bc433-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc433-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc433-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc433-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bc433-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc433-119">Request headers</span></span>
|<span data-ttu-id="bc433-120">标头</span><span class="sxs-lookup"><span data-stu-id="bc433-120">Header</span></span>|<span data-ttu-id="bc433-121">值</span><span class="sxs-lookup"><span data-stu-id="bc433-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc433-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc433-122">Authorization</span></span>|<span data-ttu-id="bc433-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc433-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc433-124">接受</span><span class="sxs-lookup"><span data-stu-id="bc433-124">Accept</span></span>|<span data-ttu-id="bc433-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc433-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc433-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc433-126">Request body</span></span>
<span data-ttu-id="bc433-127">在请求正文中，提供 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc433-127">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="bc433-128">下表显示创建 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc433-128">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="bc433-129">属性</span><span class="sxs-lookup"><span data-stu-id="bc433-129">Property</span></span>|<span data-ttu-id="bc433-130">类型</span><span class="sxs-lookup"><span data-stu-id="bc433-130">Type</span></span>|<span data-ttu-id="bc433-131">说明</span><span class="sxs-lookup"><span data-stu-id="bc433-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc433-132">id</span><span class="sxs-lookup"><span data-stu-id="bc433-132">id</span></span>|<span data-ttu-id="bc433-133">String</span><span class="sxs-lookup"><span data-stu-id="bc433-133">String</span></span>|<span data-ttu-id="bc433-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="bc433-134">The key of the assignment.</span></span>|
|<span data-ttu-id="bc433-135">target</span><span class="sxs-lookup"><span data-stu-id="bc433-135">target</span></span>|[<span data-ttu-id="bc433-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bc433-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bc433-137">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="bc433-137">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="bc433-138">source</span><span class="sxs-lookup"><span data-stu-id="bc433-138">source</span></span>|[<span data-ttu-id="bc433-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="bc433-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="bc433-140">设备配置、direct 或包裹/policySet 的工作分配源。</span><span class="sxs-lookup"><span data-stu-id="bc433-140">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="bc433-141">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="bc433-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="bc433-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="bc433-142">sourceId</span></span>|<span data-ttu-id="bc433-143">String</span><span class="sxs-lookup"><span data-stu-id="bc433-143">String</span></span>|<span data-ttu-id="bc433-144">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="bc433-144">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="bc433-145">响应</span><span class="sxs-lookup"><span data-stu-id="bc433-145">Response</span></span>
<span data-ttu-id="bc433-146">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc433-146">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc433-147">示例</span><span class="sxs-lookup"><span data-stu-id="bc433-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc433-148">请求</span><span class="sxs-lookup"><span data-stu-id="bc433-148">Request</span></span>
<span data-ttu-id="bc433-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc433-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc433-150">响应</span><span class="sxs-lookup"><span data-stu-id="bc433-150">Response</span></span>
<span data-ttu-id="bc433-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc433-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




