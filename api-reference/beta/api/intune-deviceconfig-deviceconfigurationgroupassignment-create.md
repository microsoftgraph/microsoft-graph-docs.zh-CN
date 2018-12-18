---
title: 创建 deviceConfigurationGroupAssignment
description: 创建新的 deviceConfigurationGroupAssignment 对象。
author: tfitzmac
ms.openlocfilehash: c07356d3cf63699fda95e2be6fe361841e0b0d95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355102"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="44849-103">创建 deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="44849-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="44849-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44849-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44849-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44849-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44849-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44849-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44849-107">创建新的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44849-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44849-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44849-108">Prerequisites</span></span>
<span data-ttu-id="44849-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="44849-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44849-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44849-111">Permission type</span></span>|<span data-ttu-id="44849-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44849-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44849-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44849-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44849-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44849-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44849-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44849-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44849-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44849-116">Not supported.</span></span>|
|<span data-ttu-id="44849-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44849-117">Application</span></span>|<span data-ttu-id="44849-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="44849-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44849-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44849-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="44849-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="44849-120">Request headers</span></span>
|<span data-ttu-id="44849-121">标头</span><span class="sxs-lookup"><span data-stu-id="44849-121">Header</span></span>|<span data-ttu-id="44849-122">值</span><span class="sxs-lookup"><span data-stu-id="44849-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44849-123">授权</span><span class="sxs-lookup"><span data-stu-id="44849-123">Authorization</span></span>|<span data-ttu-id="44849-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44849-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44849-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44849-125">Accept</span></span>|<span data-ttu-id="44849-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44849-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44849-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44849-127">Request body</span></span>
<span data-ttu-id="44849-128">在请求正文中，提供 deviceConfigurationGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44849-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="44849-129">下表显示时创建 deviceConfigurationGroupAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44849-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="44849-130">属性</span><span class="sxs-lookup"><span data-stu-id="44849-130">Property</span></span>|<span data-ttu-id="44849-131">类型</span><span class="sxs-lookup"><span data-stu-id="44849-131">Type</span></span>|<span data-ttu-id="44849-132">说明</span><span class="sxs-lookup"><span data-stu-id="44849-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44849-133">id</span><span class="sxs-lookup"><span data-stu-id="44849-133">id</span></span>|<span data-ttu-id="44849-134">String</span><span class="sxs-lookup"><span data-stu-id="44849-134">String</span></span>|<span data-ttu-id="44849-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="44849-135">Key of the entity.</span></span>|
|<span data-ttu-id="44849-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="44849-136">targetGroupId</span></span>|<span data-ttu-id="44849-137">字符串</span><span class="sxs-lookup"><span data-stu-id="44849-137">String</span></span>|<span data-ttu-id="44849-138">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="44849-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="44849-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="44849-139">excludeGroup</span></span>|<span data-ttu-id="44849-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="44849-140">Boolean</span></span>|<span data-ttu-id="44849-141">指示此组是否应排除。</span><span class="sxs-lookup"><span data-stu-id="44849-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="44849-142">应包含的组的默认值</span><span class="sxs-lookup"><span data-stu-id="44849-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="44849-143">响应</span><span class="sxs-lookup"><span data-stu-id="44849-143">Response</span></span>
<span data-ttu-id="44849-144">如果成功，此方法返回`201 Created`响应代码和响应正文中的[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44849-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44849-145">示例</span><span class="sxs-lookup"><span data-stu-id="44849-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="44849-146">请求</span><span class="sxs-lookup"><span data-stu-id="44849-146">Request</span></span>
<span data-ttu-id="44849-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44849-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44849-148">响应</span><span class="sxs-lookup"><span data-stu-id="44849-148">Response</span></span>
<span data-ttu-id="44849-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44849-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





