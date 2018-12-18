---
title: 创建 deviceConfigurationAssignment
description: 创建新的 deviceConfigurationAssignment 对象。
author: tfitzmac
ms.openlocfilehash: d278c04f0372869bf6b79e63a68d27766ef36485
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329104"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="3947e-103">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3947e-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="3947e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3947e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3947e-105">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3947e-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3947e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3947e-106">Prerequisites</span></span>
<span data-ttu-id="3947e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3947e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3947e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3947e-109">Permission type</span></span>|<span data-ttu-id="3947e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3947e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3947e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3947e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3947e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3947e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3947e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3947e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3947e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3947e-114">Not supported.</span></span>|
|<span data-ttu-id="3947e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3947e-115">Application</span></span>|<span data-ttu-id="3947e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3947e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3947e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3947e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3947e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3947e-118">Request headers</span></span>
|<span data-ttu-id="3947e-119">标头</span><span class="sxs-lookup"><span data-stu-id="3947e-119">Header</span></span>|<span data-ttu-id="3947e-120">值</span><span class="sxs-lookup"><span data-stu-id="3947e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3947e-121">授权</span><span class="sxs-lookup"><span data-stu-id="3947e-121">Authorization</span></span>|<span data-ttu-id="3947e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3947e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3947e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3947e-123">Accept</span></span>|<span data-ttu-id="3947e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3947e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3947e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3947e-125">Request body</span></span>
<span data-ttu-id="3947e-126">在请求正文中，提供 deviceConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3947e-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="3947e-127">下表显示创建 deviceConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3947e-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="3947e-128">属性</span><span class="sxs-lookup"><span data-stu-id="3947e-128">Property</span></span>|<span data-ttu-id="3947e-129">类型</span><span class="sxs-lookup"><span data-stu-id="3947e-129">Type</span></span>|<span data-ttu-id="3947e-130">说明</span><span class="sxs-lookup"><span data-stu-id="3947e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3947e-131">id</span><span class="sxs-lookup"><span data-stu-id="3947e-131">id</span></span>|<span data-ttu-id="3947e-132">String</span><span class="sxs-lookup"><span data-stu-id="3947e-132">String</span></span>|<span data-ttu-id="3947e-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="3947e-133">The key of the assignment.</span></span>|
|<span data-ttu-id="3947e-134">target</span><span class="sxs-lookup"><span data-stu-id="3947e-134">target</span></span>|[<span data-ttu-id="3947e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3947e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3947e-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="3947e-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="3947e-137">响应</span><span class="sxs-lookup"><span data-stu-id="3947e-137">Response</span></span>
<span data-ttu-id="3947e-138">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3947e-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3947e-139">示例</span><span class="sxs-lookup"><span data-stu-id="3947e-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="3947e-140">请求</span><span class="sxs-lookup"><span data-stu-id="3947e-140">Request</span></span>
<span data-ttu-id="3947e-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3947e-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3947e-142">响应</span><span class="sxs-lookup"><span data-stu-id="3947e-142">Response</span></span>
<span data-ttu-id="3947e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3947e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



