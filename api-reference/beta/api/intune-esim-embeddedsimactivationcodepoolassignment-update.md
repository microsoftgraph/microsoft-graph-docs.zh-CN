---
title: 更新 embeddedSIMActivationCodePoolAssignment
description: 更新 embeddedSIMActivationCodePoolAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8dc0a1f5452f300ac33c5d888494ce7524ce051a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452139"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="b9c76-103">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="b9c76-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="b9c76-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9c76-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9c76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9c76-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9c76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c76-107">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9c76-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c76-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9c76-108">Prerequisites</span></span>
<span data-ttu-id="b9c76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c76-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c76-111">Permission type</span></span>|<span data-ttu-id="b9c76-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9c76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c76-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9c76-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c76-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c76-116">Not supported.</span></span>|
|<span data-ttu-id="b9c76-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c76-117">Application</span></span>|<span data-ttu-id="b9c76-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c76-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c76-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9c76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9c76-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9c76-120">Request headers</span></span>
|<span data-ttu-id="b9c76-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9c76-121">Header</span></span>|<span data-ttu-id="b9c76-122">值</span><span class="sxs-lookup"><span data-stu-id="b9c76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c76-123">Authorization</span></span>|<span data-ttu-id="b9c76-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9c76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c76-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9c76-125">Accept</span></span>|<span data-ttu-id="b9c76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c76-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9c76-127">Request body</span></span>
<span data-ttu-id="b9c76-128">在请求正文中，提供[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9c76-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="b9c76-129">下表显示创建[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9c76-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="b9c76-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9c76-130">Property</span></span>|<span data-ttu-id="b9c76-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9c76-131">Type</span></span>|<span data-ttu-id="b9c76-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9c76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c76-133">id</span><span class="sxs-lookup"><span data-stu-id="b9c76-133">id</span></span>|<span data-ttu-id="b9c76-134">String</span><span class="sxs-lookup"><span data-stu-id="b9c76-134">String</span></span>|<span data-ttu-id="b9c76-135">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b9c76-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="b9c76-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="b9c76-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="b9c76-137">target</span><span class="sxs-lookup"><span data-stu-id="b9c76-137">target</span></span>|[<span data-ttu-id="b9c76-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b9c76-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b9c76-139">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="b9c76-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="b9c76-140">响应</span><span class="sxs-lookup"><span data-stu-id="b9c76-140">Response</span></span>
<span data-ttu-id="b9c76-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9c76-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c76-142">示例</span><span class="sxs-lookup"><span data-stu-id="b9c76-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c76-143">请求</span><span class="sxs-lookup"><span data-stu-id="b9c76-143">Request</span></span>
<span data-ttu-id="b9c76-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9c76-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b9c76-145">响应</span><span class="sxs-lookup"><span data-stu-id="b9c76-145">Response</span></span>
<span data-ttu-id="b9c76-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9c76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



