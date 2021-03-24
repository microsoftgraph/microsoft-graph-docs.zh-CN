---
title: 更新 deviceConfigurationGroupAssignment
description: 更新 deviceConfigurationGroupAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd267a5a634797af0d773e749d1b222f604a1739
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137502"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="9eb7c-103">更新 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9eb7c-103">Update deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="9eb7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eb7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9eb7c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9eb7c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9eb7c-107">更新 [deviceConfigurationGroupAssignment 对象](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9eb7c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9eb7c-108">Prerequisites</span></span>
<span data-ttu-id="9eb7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eb7c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9eb7c-111">Permission type</span></span>|<span data-ttu-id="9eb7c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9eb7c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9eb7c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9eb7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9eb7c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eb7c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9eb7c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9eb7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9eb7c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-116">Not supported.</span></span>|
|<span data-ttu-id="9eb7c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9eb7c-117">Application</span></span>|<span data-ttu-id="9eb7c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eb7c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9eb7c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9eb7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9eb7c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9eb7c-120">Request headers</span></span>
|<span data-ttu-id="9eb7c-121">标头</span><span class="sxs-lookup"><span data-stu-id="9eb7c-121">Header</span></span>|<span data-ttu-id="9eb7c-122">值</span><span class="sxs-lookup"><span data-stu-id="9eb7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9eb7c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eb7c-123">Authorization</span></span>|<span data-ttu-id="9eb7c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9eb7c-125">接受</span><span class="sxs-lookup"><span data-stu-id="9eb7c-125">Accept</span></span>|<span data-ttu-id="9eb7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9eb7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eb7c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9eb7c-127">Request body</span></span>
<span data-ttu-id="9eb7c-128">在请求正文中，提供 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="9eb7c-129">下表显示创建 [deviceConfigurationGroupAssignment 时所需的属性](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="9eb7c-130">属性</span><span class="sxs-lookup"><span data-stu-id="9eb7c-130">Property</span></span>|<span data-ttu-id="9eb7c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9eb7c-131">Type</span></span>|<span data-ttu-id="9eb7c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9eb7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eb7c-133">id</span><span class="sxs-lookup"><span data-stu-id="9eb7c-133">id</span></span>|<span data-ttu-id="9eb7c-134">String</span><span class="sxs-lookup"><span data-stu-id="9eb7c-134">String</span></span>|<span data-ttu-id="9eb7c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-135">Key of the entity.</span></span>|
|<span data-ttu-id="9eb7c-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="9eb7c-136">targetGroupId</span></span>|<span data-ttu-id="9eb7c-137">String</span><span class="sxs-lookup"><span data-stu-id="9eb7c-137">String</span></span>|<span data-ttu-id="9eb7c-138">面向设备配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="9eb7c-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="9eb7c-139">excludeGroup</span></span>|<span data-ttu-id="9eb7c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb7c-140">Boolean</span></span>|<span data-ttu-id="9eb7c-141">指示是否应排除此组。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="9eb7c-142">应包含组的默认值</span><span class="sxs-lookup"><span data-stu-id="9eb7c-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="9eb7c-143">响应</span><span class="sxs-lookup"><span data-stu-id="9eb7c-143">Response</span></span>
<span data-ttu-id="9eb7c-144">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb7c-145">示例</span><span class="sxs-lookup"><span data-stu-id="9eb7c-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="9eb7c-146">请求</span><span class="sxs-lookup"><span data-stu-id="9eb7c-146">Request</span></span>
<span data-ttu-id="9eb7c-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="9eb7c-148">响应</span><span class="sxs-lookup"><span data-stu-id="9eb7c-148">Response</span></span>
<span data-ttu-id="9eb7c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9eb7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```




