---
title: 创建 deviceConfigurationAssignment
description: 创建新的 deviceConfigurationAssignment 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6dcac355c72e9326909091293af8759d0e8584c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400380"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="41bd6-103">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="41bd6-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="41bd6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="41bd6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="41bd6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41bd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41bd6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41bd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41bd6-107">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41bd6-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41bd6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41bd6-108">Prerequisites</span></span>
<span data-ttu-id="41bd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="41bd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="41bd6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41bd6-111">Permission type</span></span>|<span data-ttu-id="41bd6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41bd6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41bd6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41bd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41bd6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bd6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41bd6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41bd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41bd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41bd6-116">Not supported.</span></span>|
|<span data-ttu-id="41bd6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41bd6-117">Application</span></span>|<span data-ttu-id="41bd6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="41bd6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41bd6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41bd6-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="41bd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41bd6-120">Request headers</span></span>
|<span data-ttu-id="41bd6-121">标头</span><span class="sxs-lookup"><span data-stu-id="41bd6-121">Header</span></span>|<span data-ttu-id="41bd6-122">值</span><span class="sxs-lookup"><span data-stu-id="41bd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41bd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41bd6-123">Authorization</span></span>|<span data-ttu-id="41bd6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41bd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41bd6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41bd6-125">Accept</span></span>|<span data-ttu-id="41bd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41bd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41bd6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41bd6-127">Request body</span></span>
<span data-ttu-id="41bd6-128">在请求正文中，提供 deviceConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41bd6-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="41bd6-129">下表显示创建 deviceConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41bd6-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="41bd6-130">属性</span><span class="sxs-lookup"><span data-stu-id="41bd6-130">Property</span></span>|<span data-ttu-id="41bd6-131">类型</span><span class="sxs-lookup"><span data-stu-id="41bd6-131">Type</span></span>|<span data-ttu-id="41bd6-132">说明</span><span class="sxs-lookup"><span data-stu-id="41bd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41bd6-133">id</span><span class="sxs-lookup"><span data-stu-id="41bd6-133">id</span></span>|<span data-ttu-id="41bd6-134">String</span><span class="sxs-lookup"><span data-stu-id="41bd6-134">String</span></span>|<span data-ttu-id="41bd6-135">分配的键。</span><span class="sxs-lookup"><span data-stu-id="41bd6-135">The key of the assignment.</span></span>|
|<span data-ttu-id="41bd6-136">target</span><span class="sxs-lookup"><span data-stu-id="41bd6-136">target</span></span>|[<span data-ttu-id="41bd6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="41bd6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="41bd6-138">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="41bd6-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="41bd6-139">响应</span><span class="sxs-lookup"><span data-stu-id="41bd6-139">Response</span></span>
<span data-ttu-id="41bd6-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41bd6-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41bd6-141">示例</span><span class="sxs-lookup"><span data-stu-id="41bd6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="41bd6-142">请求</span><span class="sxs-lookup"><span data-stu-id="41bd6-142">Request</span></span>
<span data-ttu-id="41bd6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41bd6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="41bd6-144">响应</span><span class="sxs-lookup"><span data-stu-id="41bd6-144">Response</span></span>
<span data-ttu-id="41bd6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41bd6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




