---
title: 创建 managedDeviceMobileAppConfigurationAssignment
description: 创建新的 managedDeviceMobileAppConfigurationAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc6286af6fe2c05fad3752fc626dd3e279058179
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754257"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="0c22c-103">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0c22c-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

<span data-ttu-id="0c22c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c22c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c22c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c22c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c22c-106">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c22c-106">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c22c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c22c-107">Prerequisites</span></span>
<span data-ttu-id="0c22c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c22c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c22c-110">Permission type</span></span>|<span data-ttu-id="0c22c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c22c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c22c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c22c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c22c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c22c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c22c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c22c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c22c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c22c-115">Not supported.</span></span>|
|<span data-ttu-id="0c22c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c22c-116">Application</span></span>|<span data-ttu-id="0c22c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c22c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c22c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c22c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0c22c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c22c-119">Request headers</span></span>
|<span data-ttu-id="0c22c-120">标头</span><span class="sxs-lookup"><span data-stu-id="0c22c-120">Header</span></span>|<span data-ttu-id="0c22c-121">值</span><span class="sxs-lookup"><span data-stu-id="0c22c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c22c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c22c-122">Authorization</span></span>|<span data-ttu-id="0c22c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c22c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c22c-124">接受</span><span class="sxs-lookup"><span data-stu-id="0c22c-124">Accept</span></span>|<span data-ttu-id="0c22c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c22c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c22c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c22c-126">Request body</span></span>
<span data-ttu-id="0c22c-127">在请求正文中，提供 managedDeviceMobileAppConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c22c-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="0c22c-128">下表显示创建 managedDeviceMobileAppConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c22c-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="0c22c-129">属性</span><span class="sxs-lookup"><span data-stu-id="0c22c-129">Property</span></span>|<span data-ttu-id="0c22c-130">类型</span><span class="sxs-lookup"><span data-stu-id="0c22c-130">Type</span></span>|<span data-ttu-id="0c22c-131">说明</span><span class="sxs-lookup"><span data-stu-id="0c22c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c22c-132">id</span><span class="sxs-lookup"><span data-stu-id="0c22c-132">id</span></span>|<span data-ttu-id="0c22c-133">String</span><span class="sxs-lookup"><span data-stu-id="0c22c-133">String</span></span>|<span data-ttu-id="0c22c-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0c22c-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0c22c-135">target</span><span class="sxs-lookup"><span data-stu-id="0c22c-135">target</span></span>|[<span data-ttu-id="0c22c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0c22c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0c22c-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="0c22c-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="0c22c-138">响应</span><span class="sxs-lookup"><span data-stu-id="0c22c-138">Response</span></span>
<span data-ttu-id="0c22c-139">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c22c-139">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c22c-140">示例</span><span class="sxs-lookup"><span data-stu-id="0c22c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c22c-141">请求</span><span class="sxs-lookup"><span data-stu-id="0c22c-141">Request</span></span>
<span data-ttu-id="0c22c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c22c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="0c22c-143">响应</span><span class="sxs-lookup"><span data-stu-id="0c22c-143">Response</span></span>
<span data-ttu-id="0c22c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c22c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
```




