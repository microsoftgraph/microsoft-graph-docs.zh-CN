---
title: 创建 deviceConfigurationAssignment
description: 创建新的 deviceConfigurationAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d81f8f5618b9582b40bfbccbb4c6c0fb50c2c11c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961559"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="65011-103">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="65011-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="65011-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="65011-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65011-105">创建新的 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65011-105">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65011-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="65011-106">Prerequisites</span></span>
<span data-ttu-id="65011-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="65011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65011-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65011-109">Permission type</span></span>|<span data-ttu-id="65011-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65011-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65011-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65011-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65011-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65011-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65011-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65011-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65011-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65011-114">Not supported.</span></span>|
|<span data-ttu-id="65011-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65011-115">Application</span></span>|<span data-ttu-id="65011-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65011-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65011-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65011-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="65011-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65011-118">Request headers</span></span>
|<span data-ttu-id="65011-119">标头</span><span class="sxs-lookup"><span data-stu-id="65011-119">Header</span></span>|<span data-ttu-id="65011-120">值</span><span class="sxs-lookup"><span data-stu-id="65011-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65011-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65011-121">Authorization</span></span>|<span data-ttu-id="65011-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65011-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65011-123">Accept</span><span class="sxs-lookup"><span data-stu-id="65011-123">Accept</span></span>|<span data-ttu-id="65011-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65011-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65011-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="65011-125">Request body</span></span>
<span data-ttu-id="65011-126">在请求正文中，提供 deviceConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65011-126">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="65011-127">下表显示创建 deviceConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65011-127">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="65011-128">属性</span><span class="sxs-lookup"><span data-stu-id="65011-128">Property</span></span>|<span data-ttu-id="65011-129">类型</span><span class="sxs-lookup"><span data-stu-id="65011-129">Type</span></span>|<span data-ttu-id="65011-130">说明</span><span class="sxs-lookup"><span data-stu-id="65011-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65011-131">id</span><span class="sxs-lookup"><span data-stu-id="65011-131">id</span></span>|<span data-ttu-id="65011-132">String</span><span class="sxs-lookup"><span data-stu-id="65011-132">String</span></span>|<span data-ttu-id="65011-133">分配的键。</span><span class="sxs-lookup"><span data-stu-id="65011-133">The key of the assignment.</span></span>|
|<span data-ttu-id="65011-134">target</span><span class="sxs-lookup"><span data-stu-id="65011-134">target</span></span>|[<span data-ttu-id="65011-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="65011-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="65011-136">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="65011-136">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="65011-137">响应</span><span class="sxs-lookup"><span data-stu-id="65011-137">Response</span></span>
<span data-ttu-id="65011-138">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65011-138">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65011-139">示例</span><span class="sxs-lookup"><span data-stu-id="65011-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="65011-140">请求</span><span class="sxs-lookup"><span data-stu-id="65011-140">Request</span></span>
<span data-ttu-id="65011-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65011-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65011-142">响应</span><span class="sxs-lookup"><span data-stu-id="65011-142">Response</span></span>
<span data-ttu-id="65011-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65011-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



