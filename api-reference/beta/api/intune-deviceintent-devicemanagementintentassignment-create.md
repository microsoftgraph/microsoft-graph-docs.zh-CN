---
title: 创建 deviceManagementIntentAssignment
description: 创建新的 deviceManagementIntentAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91a23ab1d0c715f3b3cb28e4f6c84c1e3168270a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32508377"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="55872-103">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="55872-103">Create deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="55872-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55872-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55872-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55872-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55872-106">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55872-106">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55872-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="55872-107">Prerequisites</span></span>
<span data-ttu-id="55872-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55872-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="55872-110">Permission type</span></span>|<span data-ttu-id="55872-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55872-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55872-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55872-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55872-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55872-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55872-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55872-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55872-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="55872-115">Not supported.</span></span>|
|<span data-ttu-id="55872-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="55872-116">Application</span></span>|<span data-ttu-id="55872-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="55872-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55872-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55872-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="55872-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="55872-119">Request headers</span></span>
|<span data-ttu-id="55872-120">标头</span><span class="sxs-lookup"><span data-stu-id="55872-120">Header</span></span>|<span data-ttu-id="55872-121">值</span><span class="sxs-lookup"><span data-stu-id="55872-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55872-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55872-122">Authorization</span></span>|<span data-ttu-id="55872-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55872-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55872-124">接受</span><span class="sxs-lookup"><span data-stu-id="55872-124">Accept</span></span>|<span data-ttu-id="55872-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55872-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55872-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="55872-126">Request body</span></span>
<span data-ttu-id="55872-127">在请求正文中, 提供 deviceManagementIntentAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55872-127">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="55872-128">下表显示创建 deviceManagementIntentAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55872-128">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="55872-129">属性</span><span class="sxs-lookup"><span data-stu-id="55872-129">Property</span></span>|<span data-ttu-id="55872-130">类型</span><span class="sxs-lookup"><span data-stu-id="55872-130">Type</span></span>|<span data-ttu-id="55872-131">说明</span><span class="sxs-lookup"><span data-stu-id="55872-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55872-132">id</span><span class="sxs-lookup"><span data-stu-id="55872-132">id</span></span>|<span data-ttu-id="55872-133">String</span><span class="sxs-lookup"><span data-stu-id="55872-133">String</span></span>|<span data-ttu-id="55872-134">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="55872-134">The assignment ID</span></span>|
|<span data-ttu-id="55872-135">target</span><span class="sxs-lookup"><span data-stu-id="55872-135">target</span></span>|[<span data-ttu-id="55872-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="55872-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="55872-137">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="55872-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="55872-138">响应</span><span class="sxs-lookup"><span data-stu-id="55872-138">Response</span></span>
<span data-ttu-id="55872-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="55872-139">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55872-140">示例</span><span class="sxs-lookup"><span data-stu-id="55872-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="55872-141">请求</span><span class="sxs-lookup"><span data-stu-id="55872-141">Request</span></span>
<span data-ttu-id="55872-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55872-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="55872-143">响应</span><span class="sxs-lookup"><span data-stu-id="55872-143">Response</span></span>
<span data-ttu-id="55872-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55872-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





