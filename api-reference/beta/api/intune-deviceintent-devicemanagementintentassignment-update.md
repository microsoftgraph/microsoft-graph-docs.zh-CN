---
title: 更新 deviceManagementIntentAssignment
description: 更新 deviceManagementIntentAssignment 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 862ecb3b706d486499a3bee8c0de14c92b7368e8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767454"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="42e80-103">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="42e80-103">Update deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="42e80-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42e80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42e80-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42e80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42e80-106">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="42e80-106">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42e80-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="42e80-107">Prerequisites</span></span>
<span data-ttu-id="42e80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42e80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42e80-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42e80-110">Permission type</span></span>|<span data-ttu-id="42e80-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42e80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42e80-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42e80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42e80-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e80-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42e80-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42e80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42e80-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42e80-115">Not supported.</span></span>|
|<span data-ttu-id="42e80-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="42e80-116">Application</span></span>|<span data-ttu-id="42e80-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e80-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42e80-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42e80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="42e80-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42e80-119">Request headers</span></span>
|<span data-ttu-id="42e80-120">标头</span><span class="sxs-lookup"><span data-stu-id="42e80-120">Header</span></span>|<span data-ttu-id="42e80-121">值</span><span class="sxs-lookup"><span data-stu-id="42e80-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42e80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42e80-122">Authorization</span></span>|<span data-ttu-id="42e80-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42e80-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42e80-124">接受</span><span class="sxs-lookup"><span data-stu-id="42e80-124">Accept</span></span>|<span data-ttu-id="42e80-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42e80-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42e80-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42e80-126">Request body</span></span>
<span data-ttu-id="42e80-127">在请求正文中，提供[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42e80-127">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="42e80-128">下表显示创建[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42e80-128">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="42e80-129">属性</span><span class="sxs-lookup"><span data-stu-id="42e80-129">Property</span></span>|<span data-ttu-id="42e80-130">类型</span><span class="sxs-lookup"><span data-stu-id="42e80-130">Type</span></span>|<span data-ttu-id="42e80-131">说明</span><span class="sxs-lookup"><span data-stu-id="42e80-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42e80-132">id</span><span class="sxs-lookup"><span data-stu-id="42e80-132">id</span></span>|<span data-ttu-id="42e80-133">String</span><span class="sxs-lookup"><span data-stu-id="42e80-133">String</span></span>|<span data-ttu-id="42e80-134">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="42e80-134">The assignment ID</span></span>|
|<span data-ttu-id="42e80-135">target</span><span class="sxs-lookup"><span data-stu-id="42e80-135">target</span></span>|[<span data-ttu-id="42e80-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42e80-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="42e80-137">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="42e80-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="42e80-138">响应</span><span class="sxs-lookup"><span data-stu-id="42e80-138">Response</span></span>
<span data-ttu-id="42e80-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42e80-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42e80-140">示例</span><span class="sxs-lookup"><span data-stu-id="42e80-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="42e80-141">请求</span><span class="sxs-lookup"><span data-stu-id="42e80-141">Request</span></span>
<span data-ttu-id="42e80-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42e80-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="42e80-143">响应</span><span class="sxs-lookup"><span data-stu-id="42e80-143">Response</span></span>
<span data-ttu-id="42e80-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42e80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




