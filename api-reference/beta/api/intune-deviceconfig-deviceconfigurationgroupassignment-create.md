---
title: 创建 deviceConfigurationGroupAssignment
description: 创建新的 deviceConfigurationGroupAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 686439ac3dceee93e9053490132d29b241cf49ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142292"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="9f772-103">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9f772-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="9f772-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f772-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f772-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f772-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f772-106">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f772-106">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f772-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f772-107">Prerequisites</span></span>
<span data-ttu-id="9f772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9f772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f772-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f772-110">Permission type</span></span>|<span data-ttu-id="9f772-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f772-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f772-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f772-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f772-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f772-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f772-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f772-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f772-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f772-115">Not supported.</span></span>|
|<span data-ttu-id="9f772-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f772-116">Application</span></span>|<span data-ttu-id="9f772-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f772-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f772-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f772-118">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9f772-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f772-119">Request headers</span></span>
|<span data-ttu-id="9f772-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f772-120">Header</span></span>|<span data-ttu-id="9f772-121">值</span><span class="sxs-lookup"><span data-stu-id="9f772-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f772-122">Authorization</span></span>|<span data-ttu-id="9f772-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f772-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f772-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f772-124">Accept</span></span>|<span data-ttu-id="9f772-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f772-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f772-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f772-126">Request body</span></span>
<span data-ttu-id="9f772-127">在请求正文中, 提供 deviceConfigurationGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f772-127">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="9f772-128">下表显示创建 deviceConfigurationGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f772-128">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="9f772-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f772-129">Property</span></span>|<span data-ttu-id="9f772-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f772-130">Type</span></span>|<span data-ttu-id="9f772-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f772-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f772-132">id</span><span class="sxs-lookup"><span data-stu-id="9f772-132">id</span></span>|<span data-ttu-id="9f772-133">String</span><span class="sxs-lookup"><span data-stu-id="9f772-133">String</span></span>|<span data-ttu-id="9f772-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f772-134">Key of the entity.</span></span>|
|<span data-ttu-id="9f772-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="9f772-135">targetGroupId</span></span>|<span data-ttu-id="9f772-136">字符串</span><span class="sxs-lookup"><span data-stu-id="9f772-136">String</span></span>|<span data-ttu-id="9f772-137">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="9f772-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="9f772-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="9f772-138">excludeGroup</span></span>|<span data-ttu-id="9f772-139">布尔</span><span class="sxs-lookup"><span data-stu-id="9f772-139">Boolean</span></span>|<span data-ttu-id="9f772-140">指示是否应排除此组。</span><span class="sxs-lookup"><span data-stu-id="9f772-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="9f772-141">应包含组的默认值</span><span class="sxs-lookup"><span data-stu-id="9f772-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="9f772-142">响应</span><span class="sxs-lookup"><span data-stu-id="9f772-142">Response</span></span>
<span data-ttu-id="9f772-143">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f772-143">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f772-144">示例</span><span class="sxs-lookup"><span data-stu-id="9f772-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f772-145">请求</span><span class="sxs-lookup"><span data-stu-id="9f772-145">Request</span></span>
<span data-ttu-id="9f772-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f772-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f772-147">响应</span><span class="sxs-lookup"><span data-stu-id="9f772-147">Response</span></span>
<span data-ttu-id="9f772-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f772-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




