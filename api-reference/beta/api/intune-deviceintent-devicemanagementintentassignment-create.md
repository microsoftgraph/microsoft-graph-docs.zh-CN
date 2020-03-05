---
title: 创建 deviceManagementIntentAssignment
description: 创建新的 deviceManagementIntentAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 096d949bbef788e4a17eebed0cb1052460c4cc37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471118"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="6a6df-103">创建 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="6a6df-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="6a6df-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6a6df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a6df-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a6df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a6df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a6df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a6df-107">创建新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a6df-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a6df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a6df-108">Prerequisites</span></span>
<span data-ttu-id="6a6df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a6df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a6df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a6df-111">Permission type</span></span>|<span data-ttu-id="6a6df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a6df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a6df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a6df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a6df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a6df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a6df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a6df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a6df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a6df-116">Not supported.</span></span>|
|<span data-ttu-id="6a6df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a6df-117">Application</span></span>|<span data-ttu-id="6a6df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a6df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a6df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a6df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6a6df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a6df-120">Request headers</span></span>
|<span data-ttu-id="6a6df-121">标头</span><span class="sxs-lookup"><span data-stu-id="6a6df-121">Header</span></span>|<span data-ttu-id="6a6df-122">值</span><span class="sxs-lookup"><span data-stu-id="6a6df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a6df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a6df-123">Authorization</span></span>|<span data-ttu-id="6a6df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a6df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a6df-125">接受</span><span class="sxs-lookup"><span data-stu-id="6a6df-125">Accept</span></span>|<span data-ttu-id="6a6df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a6df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a6df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a6df-127">Request body</span></span>
<span data-ttu-id="6a6df-128">在请求正文中，提供 deviceManagementIntentAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a6df-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="6a6df-129">下表显示创建 deviceManagementIntentAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a6df-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="6a6df-130">属性</span><span class="sxs-lookup"><span data-stu-id="6a6df-130">Property</span></span>|<span data-ttu-id="6a6df-131">类型</span><span class="sxs-lookup"><span data-stu-id="6a6df-131">Type</span></span>|<span data-ttu-id="6a6df-132">说明</span><span class="sxs-lookup"><span data-stu-id="6a6df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a6df-133">id</span><span class="sxs-lookup"><span data-stu-id="6a6df-133">id</span></span>|<span data-ttu-id="6a6df-134">String</span><span class="sxs-lookup"><span data-stu-id="6a6df-134">String</span></span>|<span data-ttu-id="6a6df-135">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="6a6df-135">The assignment ID</span></span>|
|<span data-ttu-id="6a6df-136">target</span><span class="sxs-lookup"><span data-stu-id="6a6df-136">target</span></span>|[<span data-ttu-id="6a6df-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6a6df-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6a6df-138">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="6a6df-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="6a6df-139">响应</span><span class="sxs-lookup"><span data-stu-id="6a6df-139">Response</span></span>
<span data-ttu-id="6a6df-140">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a6df-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a6df-141">示例</span><span class="sxs-lookup"><span data-stu-id="6a6df-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a6df-142">请求</span><span class="sxs-lookup"><span data-stu-id="6a6df-142">Request</span></span>
<span data-ttu-id="6a6df-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a6df-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a6df-144">响应</span><span class="sxs-lookup"><span data-stu-id="6a6df-144">Response</span></span>
<span data-ttu-id="6a6df-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a6df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





