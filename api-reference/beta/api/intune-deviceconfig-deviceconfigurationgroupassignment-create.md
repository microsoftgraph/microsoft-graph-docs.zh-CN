---
title: 创建 deviceConfigurationGroupAssignment
description: 创建新的 deviceConfigurationGroupAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66f0f1a2180e72ae2caad005157e4f75f5e4f81f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433405"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="80e88-103">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="80e88-103">Create deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="80e88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80e88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80e88-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80e88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80e88-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80e88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80e88-107">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80e88-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80e88-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="80e88-108">Prerequisites</span></span>
<span data-ttu-id="80e88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e88-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80e88-111">Permission type</span></span>|<span data-ttu-id="80e88-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80e88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80e88-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80e88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80e88-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e88-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80e88-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80e88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80e88-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80e88-116">Not supported.</span></span>|
|<span data-ttu-id="80e88-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80e88-117">Application</span></span>|<span data-ttu-id="80e88-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e88-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80e88-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80e88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="80e88-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80e88-120">Request headers</span></span>
|<span data-ttu-id="80e88-121">标头</span><span class="sxs-lookup"><span data-stu-id="80e88-121">Header</span></span>|<span data-ttu-id="80e88-122">值</span><span class="sxs-lookup"><span data-stu-id="80e88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80e88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80e88-123">Authorization</span></span>|<span data-ttu-id="80e88-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80e88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80e88-125">接受</span><span class="sxs-lookup"><span data-stu-id="80e88-125">Accept</span></span>|<span data-ttu-id="80e88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80e88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80e88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80e88-127">Request body</span></span>
<span data-ttu-id="80e88-128">在请求正文中，提供 deviceConfigurationGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80e88-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="80e88-129">下表显示创建 deviceConfigurationGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80e88-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="80e88-130">属性</span><span class="sxs-lookup"><span data-stu-id="80e88-130">Property</span></span>|<span data-ttu-id="80e88-131">类型</span><span class="sxs-lookup"><span data-stu-id="80e88-131">Type</span></span>|<span data-ttu-id="80e88-132">说明</span><span class="sxs-lookup"><span data-stu-id="80e88-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e88-133">id</span><span class="sxs-lookup"><span data-stu-id="80e88-133">id</span></span>|<span data-ttu-id="80e88-134">String</span><span class="sxs-lookup"><span data-stu-id="80e88-134">String</span></span>|<span data-ttu-id="80e88-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80e88-135">Key of the entity.</span></span>|
|<span data-ttu-id="80e88-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="80e88-136">targetGroupId</span></span>|<span data-ttu-id="80e88-137">String</span><span class="sxs-lookup"><span data-stu-id="80e88-137">String</span></span>|<span data-ttu-id="80e88-138">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="80e88-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="80e88-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="80e88-139">excludeGroup</span></span>|<span data-ttu-id="80e88-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="80e88-140">Boolean</span></span>|<span data-ttu-id="80e88-141">指示是否应排除此组。</span><span class="sxs-lookup"><span data-stu-id="80e88-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="80e88-142">应包含组的默认值</span><span class="sxs-lookup"><span data-stu-id="80e88-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="80e88-143">响应</span><span class="sxs-lookup"><span data-stu-id="80e88-143">Response</span></span>
<span data-ttu-id="80e88-144">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80e88-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80e88-145">示例</span><span class="sxs-lookup"><span data-stu-id="80e88-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="80e88-146">请求</span><span class="sxs-lookup"><span data-stu-id="80e88-146">Request</span></span>
<span data-ttu-id="80e88-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80e88-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="80e88-148">响应</span><span class="sxs-lookup"><span data-stu-id="80e88-148">Response</span></span>
<span data-ttu-id="80e88-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80e88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```



