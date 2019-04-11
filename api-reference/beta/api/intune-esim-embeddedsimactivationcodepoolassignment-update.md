---
title: 更新 embeddedSIMActivationCodePoolAssignment
description: 更新 embeddedSIMActivationCodePoolAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc2b5cbe9051e44ef68d62aa60fd67eb8b6a4597
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786978"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="9f447-103">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="9f447-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="9f447-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f447-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f447-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f447-106">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f447-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f447-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f447-107">Prerequisites</span></span>
<span data-ttu-id="9f447-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f447-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f447-110">Permission type</span></span>|<span data-ttu-id="9f447-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f447-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f447-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f447-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f447-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f447-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f447-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f447-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f447-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f447-115">Not supported.</span></span>|
|<span data-ttu-id="9f447-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f447-116">Application</span></span>|<span data-ttu-id="9f447-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f447-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f447-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f447-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9f447-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f447-119">Request headers</span></span>
|<span data-ttu-id="9f447-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f447-120">Header</span></span>|<span data-ttu-id="9f447-121">值</span><span class="sxs-lookup"><span data-stu-id="9f447-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f447-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f447-122">Authorization</span></span>|<span data-ttu-id="9f447-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f447-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f447-124">接受</span><span class="sxs-lookup"><span data-stu-id="9f447-124">Accept</span></span>|<span data-ttu-id="9f447-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f447-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f447-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f447-126">Request body</span></span>
<span data-ttu-id="9f447-127">在请求正文中, 提供[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f447-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="9f447-128">下表显示创建[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f447-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="9f447-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f447-129">Property</span></span>|<span data-ttu-id="9f447-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f447-130">Type</span></span>|<span data-ttu-id="9f447-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f447-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f447-132">id</span><span class="sxs-lookup"><span data-stu-id="9f447-132">id</span></span>|<span data-ttu-id="9f447-133">String</span><span class="sxs-lookup"><span data-stu-id="9f447-133">String</span></span>|<span data-ttu-id="9f447-134">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9f447-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="9f447-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="9f447-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9f447-136">target</span><span class="sxs-lookup"><span data-stu-id="9f447-136">target</span></span>|[<span data-ttu-id="9f447-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f447-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f447-138">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="9f447-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="9f447-139">响应</span><span class="sxs-lookup"><span data-stu-id="9f447-139">Response</span></span>
<span data-ttu-id="9f447-140">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9f447-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f447-141">示例</span><span class="sxs-lookup"><span data-stu-id="9f447-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f447-142">请求</span><span class="sxs-lookup"><span data-stu-id="9f447-142">Request</span></span>
<span data-ttu-id="9f447-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f447-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f447-144">响应</span><span class="sxs-lookup"><span data-stu-id="9f447-144">Response</span></span>
<span data-ttu-id="9f447-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f447-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





