---
title: 更新 embeddedSIMActivationCodePoolAssignment
description: 更新 embeddedSIMActivationCodePoolAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60c73bfa768489b5fd78de77ad513e4c9cc398f1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943556"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="102b8-103">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="102b8-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="102b8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="102b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="102b8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="102b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="102b8-106">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="102b8-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="102b8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="102b8-107">Prerequisites</span></span>
<span data-ttu-id="102b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="102b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="102b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="102b8-110">Permission type</span></span>|<span data-ttu-id="102b8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="102b8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="102b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="102b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="102b8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="102b8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="102b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="102b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="102b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="102b8-115">Not supported.</span></span>|
|<span data-ttu-id="102b8-116">Application</span><span class="sxs-lookup"><span data-stu-id="102b8-116">Application</span></span>|<span data-ttu-id="102b8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="102b8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="102b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="102b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="102b8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="102b8-119">Request headers</span></span>
|<span data-ttu-id="102b8-120">标头</span><span class="sxs-lookup"><span data-stu-id="102b8-120">Header</span></span>|<span data-ttu-id="102b8-121">值</span><span class="sxs-lookup"><span data-stu-id="102b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="102b8-122">授权</span><span class="sxs-lookup"><span data-stu-id="102b8-122">Authorization</span></span>|<span data-ttu-id="102b8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="102b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="102b8-124">接受</span><span class="sxs-lookup"><span data-stu-id="102b8-124">Accept</span></span>|<span data-ttu-id="102b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="102b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="102b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="102b8-126">Request body</span></span>
<span data-ttu-id="102b8-127">在请求正文中，提供[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="102b8-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="102b8-128">下表显示创建[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="102b8-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="102b8-129">属性</span><span class="sxs-lookup"><span data-stu-id="102b8-129">Property</span></span>|<span data-ttu-id="102b8-130">类型</span><span class="sxs-lookup"><span data-stu-id="102b8-130">Type</span></span>|<span data-ttu-id="102b8-131">说明</span><span class="sxs-lookup"><span data-stu-id="102b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102b8-132">id</span><span class="sxs-lookup"><span data-stu-id="102b8-132">id</span></span>|<span data-ttu-id="102b8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="102b8-133">String</span></span>|<span data-ttu-id="102b8-134">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="102b8-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="102b8-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="102b8-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="102b8-136">target</span><span class="sxs-lookup"><span data-stu-id="102b8-136">target</span></span>|[<span data-ttu-id="102b8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="102b8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="102b8-138">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="102b8-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="102b8-139">响应</span><span class="sxs-lookup"><span data-stu-id="102b8-139">Response</span></span>
<span data-ttu-id="102b8-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="102b8-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="102b8-141">示例</span><span class="sxs-lookup"><span data-stu-id="102b8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="102b8-142">请求</span><span class="sxs-lookup"><span data-stu-id="102b8-142">Request</span></span>
<span data-ttu-id="102b8-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="102b8-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="102b8-144">响应</span><span class="sxs-lookup"><span data-stu-id="102b8-144">Response</span></span>
<span data-ttu-id="102b8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="102b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





