---
title: 创建 deviceManagementScriptAssignment
description: 创建新的 deviceManagementScriptAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fbb39816cc4a542c74fd166be431df2e71f7273
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611991"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="0c3eb-103">创建 deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="0c3eb-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="0c3eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c3eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c3eb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c3eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3eb-107">创建新的 [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c3eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c3eb-108">Prerequisites</span></span>
<span data-ttu-id="0c3eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c3eb-111">Permission type</span></span>|<span data-ttu-id="0c3eb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c3eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c3eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c3eb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3eb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c3eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c3eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-116">Not supported.</span></span>|
|<span data-ttu-id="0c3eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c3eb-117">Application</span></span>|<span data-ttu-id="0c3eb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3eb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c3eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c3eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0c3eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c3eb-120">Request headers</span></span>
|<span data-ttu-id="0c3eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="0c3eb-121">Header</span></span>|<span data-ttu-id="0c3eb-122">值</span><span class="sxs-lookup"><span data-stu-id="0c3eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c3eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c3eb-123">Authorization</span></span>|<span data-ttu-id="0c3eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c3eb-125">接受</span><span class="sxs-lookup"><span data-stu-id="0c3eb-125">Accept</span></span>|<span data-ttu-id="0c3eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c3eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c3eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c3eb-127">Request body</span></span>
<span data-ttu-id="0c3eb-128">在请求正文中，提供 deviceManagementScriptAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="0c3eb-129">下表显示创建 deviceManagementScriptAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="0c3eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="0c3eb-130">Property</span></span>|<span data-ttu-id="0c3eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="0c3eb-131">Type</span></span>|<span data-ttu-id="0c3eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="0c3eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3eb-133">id</span><span class="sxs-lookup"><span data-stu-id="0c3eb-133">id</span></span>|<span data-ttu-id="0c3eb-134">String</span><span class="sxs-lookup"><span data-stu-id="0c3eb-134">String</span></span>|<span data-ttu-id="0c3eb-135">设备管理脚本组分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="0c3eb-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-136">This property is read-only.</span></span>|
|<span data-ttu-id="0c3eb-137">target</span><span class="sxs-lookup"><span data-stu-id="0c3eb-137">target</span></span>|[<span data-ttu-id="0c3eb-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0c3eb-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0c3eb-139">我们将脚本定向到的 Azure Active Directory 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0c3eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="0c3eb-140">Response</span></span>
<span data-ttu-id="0c3eb-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c3eb-142">示例</span><span class="sxs-lookup"><span data-stu-id="0c3eb-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c3eb-143">请求</span><span class="sxs-lookup"><span data-stu-id="0c3eb-143">Request</span></span>
<span data-ttu-id="0c3eb-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="0c3eb-145">响应</span><span class="sxs-lookup"><span data-stu-id="0c3eb-145">Response</span></span>
<span data-ttu-id="0c3eb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c3eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




