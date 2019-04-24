---
title: 更新 deviceManagementIntentAssignment
description: 更新 deviceManagementIntentAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18552402a6a0531ee1c966f71bd519e4b9127d31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32508349"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="7fdbc-103">更新 deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="7fdbc-103">Update deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="7fdbc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fdbc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fdbc-106">更新[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-106">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fdbc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7fdbc-107">Prerequisites</span></span>
<span data-ttu-id="7fdbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fdbc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fdbc-110">Permission type</span></span>|<span data-ttu-id="7fdbc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7fdbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fdbc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fdbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fdbc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fdbc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7fdbc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fdbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fdbc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-115">Not supported.</span></span>|
|<span data-ttu-id="7fdbc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fdbc-116">Application</span></span>|<span data-ttu-id="7fdbc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fdbc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fdbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7fdbc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fdbc-119">Request headers</span></span>
|<span data-ttu-id="7fdbc-120">标头</span><span class="sxs-lookup"><span data-stu-id="7fdbc-120">Header</span></span>|<span data-ttu-id="7fdbc-121">值</span><span class="sxs-lookup"><span data-stu-id="7fdbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fdbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fdbc-122">Authorization</span></span>|<span data-ttu-id="7fdbc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fdbc-124">接受</span><span class="sxs-lookup"><span data-stu-id="7fdbc-124">Accept</span></span>|<span data-ttu-id="7fdbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fdbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fdbc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fdbc-126">Request body</span></span>
<span data-ttu-id="7fdbc-127">在请求正文中, 提供[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-127">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="7fdbc-128">下表显示创建[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-128">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="7fdbc-129">属性</span><span class="sxs-lookup"><span data-stu-id="7fdbc-129">Property</span></span>|<span data-ttu-id="7fdbc-130">类型</span><span class="sxs-lookup"><span data-stu-id="7fdbc-130">Type</span></span>|<span data-ttu-id="7fdbc-131">说明</span><span class="sxs-lookup"><span data-stu-id="7fdbc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fdbc-132">id</span><span class="sxs-lookup"><span data-stu-id="7fdbc-132">id</span></span>|<span data-ttu-id="7fdbc-133">String</span><span class="sxs-lookup"><span data-stu-id="7fdbc-133">String</span></span>|<span data-ttu-id="7fdbc-134">工作分配 ID</span><span class="sxs-lookup"><span data-stu-id="7fdbc-134">The assignment ID</span></span>|
|<span data-ttu-id="7fdbc-135">target</span><span class="sxs-lookup"><span data-stu-id="7fdbc-135">target</span></span>|[<span data-ttu-id="7fdbc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7fdbc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7fdbc-137">工作分配目标</span><span class="sxs-lookup"><span data-stu-id="7fdbc-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="7fdbc-138">响应</span><span class="sxs-lookup"><span data-stu-id="7fdbc-138">Response</span></span>
<span data-ttu-id="7fdbc-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fdbc-140">示例</span><span class="sxs-lookup"><span data-stu-id="7fdbc-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fdbc-141">请求</span><span class="sxs-lookup"><span data-stu-id="7fdbc-141">Request</span></span>
<span data-ttu-id="7fdbc-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7fdbc-143">响应</span><span class="sxs-lookup"><span data-stu-id="7fdbc-143">Response</span></span>
<span data-ttu-id="7fdbc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7fdbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





