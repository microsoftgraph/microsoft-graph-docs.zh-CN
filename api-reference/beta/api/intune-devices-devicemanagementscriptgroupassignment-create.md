---
title: 创建 deviceManagementScriptGroupAssignment
description: 创建新的 deviceManagementScriptGroupAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff1384b470d723e083e7070c2892f164a9775020
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150455"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="0dbdb-103">创建 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="0dbdb-103">Create deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="0dbdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dbdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dbdb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dbdb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dbdb-107">创建新的 [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dbdb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0dbdb-108">Prerequisites</span></span>
<span data-ttu-id="0dbdb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dbdb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dbdb-111">Permission type</span></span>|<span data-ttu-id="0dbdb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0dbdb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dbdb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dbdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dbdb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbdb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0dbdb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dbdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dbdb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-116">Not supported.</span></span>|
|<span data-ttu-id="0dbdb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dbdb-117">Application</span></span>|<span data-ttu-id="0dbdb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbdb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dbdb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dbdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0dbdb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dbdb-120">Request headers</span></span>
|<span data-ttu-id="0dbdb-121">标头</span><span class="sxs-lookup"><span data-stu-id="0dbdb-121">Header</span></span>|<span data-ttu-id="0dbdb-122">值</span><span class="sxs-lookup"><span data-stu-id="0dbdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dbdb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dbdb-123">Authorization</span></span>|<span data-ttu-id="0dbdb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dbdb-125">接受</span><span class="sxs-lookup"><span data-stu-id="0dbdb-125">Accept</span></span>|<span data-ttu-id="0dbdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dbdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dbdb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dbdb-127">Request body</span></span>
<span data-ttu-id="0dbdb-128">在请求正文中，提供 deviceManagementScriptGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="0dbdb-129">下表显示创建 deviceManagementScriptGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="0dbdb-130">属性</span><span class="sxs-lookup"><span data-stu-id="0dbdb-130">Property</span></span>|<span data-ttu-id="0dbdb-131">类型</span><span class="sxs-lookup"><span data-stu-id="0dbdb-131">Type</span></span>|<span data-ttu-id="0dbdb-132">说明</span><span class="sxs-lookup"><span data-stu-id="0dbdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dbdb-133">id</span><span class="sxs-lookup"><span data-stu-id="0dbdb-133">id</span></span>|<span data-ttu-id="0dbdb-134">String</span><span class="sxs-lookup"><span data-stu-id="0dbdb-134">String</span></span>|<span data-ttu-id="0dbdb-135">设备管理脚本组分配实体的键。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="0dbdb-136">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-136">This property is read-only.</span></span>|
|<span data-ttu-id="0dbdb-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="0dbdb-137">targetGroupId</span></span>|<span data-ttu-id="0dbdb-138">String</span><span class="sxs-lookup"><span data-stu-id="0dbdb-138">String</span></span>|<span data-ttu-id="0dbdb-139">我们将脚本定向到的 Azure Active Directory 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="0dbdb-140">响应</span><span class="sxs-lookup"><span data-stu-id="0dbdb-140">Response</span></span>
<span data-ttu-id="0dbdb-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dbdb-142">示例</span><span class="sxs-lookup"><span data-stu-id="0dbdb-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dbdb-143">请求</span><span class="sxs-lookup"><span data-stu-id="0dbdb-143">Request</span></span>
<span data-ttu-id="0dbdb-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="0dbdb-145">响应</span><span class="sxs-lookup"><span data-stu-id="0dbdb-145">Response</span></span>
<span data-ttu-id="0dbdb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0dbdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




