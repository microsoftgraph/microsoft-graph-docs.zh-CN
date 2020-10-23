---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 652858135557e7121386c723f44e275e6f7c1198
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732676"
---
# <a name="assign-action"></a><span data-ttu-id="66d45-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="66d45-103">assign action</span></span>

<span data-ttu-id="66d45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66d45-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66d45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d45-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66d45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d45-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66d45-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66d45-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="66d45-108">Prerequisites</span></span>
<span data-ttu-id="66d45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66d45-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="66d45-111">Permission type</span></span>|<span data-ttu-id="66d45-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66d45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66d45-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66d45-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="66d45-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="66d45-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="66d45-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d45-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66d45-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66d45-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66d45-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="66d45-117">Not supported.</span></span>|
|<span data-ttu-id="66d45-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="66d45-118">Application</span></span>||
| <span data-ttu-id="66d45-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="66d45-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="66d45-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d45-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66d45-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66d45-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="66d45-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="66d45-122">Request headers</span></span>
|<span data-ttu-id="66d45-123">标头</span><span class="sxs-lookup"><span data-stu-id="66d45-123">Header</span></span>|<span data-ttu-id="66d45-124">值</span><span class="sxs-lookup"><span data-stu-id="66d45-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66d45-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d45-125">Authorization</span></span>|<span data-ttu-id="66d45-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66d45-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66d45-127">接受</span><span class="sxs-lookup"><span data-stu-id="66d45-127">Accept</span></span>|<span data-ttu-id="66d45-128">application/json</span><span class="sxs-lookup"><span data-stu-id="66d45-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d45-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="66d45-129">Request body</span></span>
<span data-ttu-id="66d45-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66d45-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66d45-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="66d45-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66d45-132">属性</span><span class="sxs-lookup"><span data-stu-id="66d45-132">Property</span></span>|<span data-ttu-id="66d45-133">类型</span><span class="sxs-lookup"><span data-stu-id="66d45-133">Type</span></span>|<span data-ttu-id="66d45-134">说明</span><span class="sxs-lookup"><span data-stu-id="66d45-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d45-135">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="66d45-135">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="66d45-136">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66d45-136">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="66d45-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66d45-137">Not yet documented</span></span>|
|<span data-ttu-id="66d45-138">assignments</span><span class="sxs-lookup"><span data-stu-id="66d45-138">assignments</span></span>|<span data-ttu-id="66d45-139">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66d45-139">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66d45-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="66d45-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66d45-141">响应</span><span class="sxs-lookup"><span data-stu-id="66d45-141">Response</span></span>
<span data-ttu-id="66d45-142">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="66d45-142">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d45-143">示例</span><span class="sxs-lookup"><span data-stu-id="66d45-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="66d45-144">请求</span><span class="sxs-lookup"><span data-stu-id="66d45-144">Request</span></span>
<span data-ttu-id="66d45-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66d45-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 617

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66d45-146">响应</span><span class="sxs-lookup"><span data-stu-id="66d45-146">Response</span></span>
<span data-ttu-id="66d45-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66d45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```








