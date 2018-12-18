---
title: 创建 deviceManagementScriptAssignment
description: 创建新的 deviceManagementScriptAssignment 对象。
author: tfitzmac
ms.openlocfilehash: c0ef551c7f049e05dc13fd0371734206514fc534
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363758"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="40d6c-103">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="40d6c-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="40d6c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="40d6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40d6c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40d6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40d6c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="40d6c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40d6c-107">创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40d6c-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40d6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40d6c-108">Prerequisites</span></span>
<span data-ttu-id="40d6c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="40d6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40d6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40d6c-111">Permission type</span></span>|<span data-ttu-id="40d6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40d6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40d6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40d6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40d6c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40d6c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40d6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40d6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40d6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40d6c-116">Not supported.</span></span>|
|<span data-ttu-id="40d6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40d6c-117">Application</span></span>|<span data-ttu-id="40d6c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="40d6c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40d6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40d6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="40d6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40d6c-120">Request headers</span></span>
|<span data-ttu-id="40d6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="40d6c-121">Header</span></span>|<span data-ttu-id="40d6c-122">值</span><span class="sxs-lookup"><span data-stu-id="40d6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40d6c-123">授权</span><span class="sxs-lookup"><span data-stu-id="40d6c-123">Authorization</span></span>|<span data-ttu-id="40d6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40d6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40d6c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40d6c-125">Accept</span></span>|<span data-ttu-id="40d6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40d6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40d6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40d6c-127">Request body</span></span>
<span data-ttu-id="40d6c-128">在请求正文中，提供 deviceManagementScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40d6c-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="40d6c-129">下表显示时创建 deviceManagementScriptAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40d6c-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="40d6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="40d6c-130">Property</span></span>|<span data-ttu-id="40d6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="40d6c-131">Type</span></span>|<span data-ttu-id="40d6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="40d6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40d6c-133">id</span><span class="sxs-lookup"><span data-stu-id="40d6c-133">id</span></span>|<span data-ttu-id="40d6c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="40d6c-134">String</span></span>|<span data-ttu-id="40d6c-135">设备管理脚本组工作分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="40d6c-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="40d6c-136">target</span><span class="sxs-lookup"><span data-stu-id="40d6c-136">target</span></span>|[<span data-ttu-id="40d6c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="40d6c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="40d6c-138">Azure Active Directory 组的 Id 目标脚本。</span><span class="sxs-lookup"><span data-stu-id="40d6c-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="40d6c-139">响应</span><span class="sxs-lookup"><span data-stu-id="40d6c-139">Response</span></span>
<span data-ttu-id="40d6c-140">如果成功，此方法返回`201 Created`响应代码和响应正文中的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40d6c-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40d6c-141">示例</span><span class="sxs-lookup"><span data-stu-id="40d6c-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="40d6c-142">请求</span><span class="sxs-lookup"><span data-stu-id="40d6c-142">Request</span></span>
<span data-ttu-id="40d6c-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40d6c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="40d6c-144">响应</span><span class="sxs-lookup"><span data-stu-id="40d6c-144">Response</span></span>
<span data-ttu-id="40d6c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40d6c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





