---
title: 更新 embeddedSIMActivationCodePoolAssignment
description: 更新 embeddedSIMActivationCodePoolAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87d2b3470107b1c517f29af4704b8038d85a7f54
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420792"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="bfa63-103">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="bfa63-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="bfa63-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bfa63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bfa63-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bfa63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfa63-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bfa63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa63-107">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bfa63-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfa63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bfa63-108">Prerequisites</span></span>
<span data-ttu-id="bfa63-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bfa63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bfa63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfa63-111">Permission type</span></span>|<span data-ttu-id="bfa63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bfa63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfa63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfa63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfa63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfa63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfa63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfa63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfa63-116">Not supported.</span></span>|
|<span data-ttu-id="bfa63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfa63-117">Application</span></span>|<span data-ttu-id="bfa63-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfa63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfa63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfa63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bfa63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfa63-120">Request headers</span></span>
|<span data-ttu-id="bfa63-121">标头</span><span class="sxs-lookup"><span data-stu-id="bfa63-121">Header</span></span>|<span data-ttu-id="bfa63-122">值</span><span class="sxs-lookup"><span data-stu-id="bfa63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfa63-123">授权</span><span class="sxs-lookup"><span data-stu-id="bfa63-123">Authorization</span></span>|<span data-ttu-id="bfa63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bfa63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfa63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bfa63-125">Accept</span></span>|<span data-ttu-id="bfa63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfa63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfa63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfa63-127">Request body</span></span>
<span data-ttu-id="bfa63-128">在请求正文中，提供[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfa63-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="bfa63-129">下表显示时创建[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfa63-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="bfa63-130">属性</span><span class="sxs-lookup"><span data-stu-id="bfa63-130">Property</span></span>|<span data-ttu-id="bfa63-131">类型</span><span class="sxs-lookup"><span data-stu-id="bfa63-131">Type</span></span>|<span data-ttu-id="bfa63-132">说明</span><span class="sxs-lookup"><span data-stu-id="bfa63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa63-133">id</span><span class="sxs-lookup"><span data-stu-id="bfa63-133">id</span></span>|<span data-ttu-id="bfa63-134">String</span><span class="sxs-lookup"><span data-stu-id="bfa63-134">String</span></span>|<span data-ttu-id="bfa63-135">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bfa63-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="bfa63-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="bfa63-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="bfa63-137">target</span><span class="sxs-lookup"><span data-stu-id="bfa63-137">target</span></span>|[<span data-ttu-id="bfa63-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bfa63-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bfa63-139">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="bfa63-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="bfa63-140">响应</span><span class="sxs-lookup"><span data-stu-id="bfa63-140">Response</span></span>
<span data-ttu-id="bfa63-141">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfa63-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfa63-142">示例</span><span class="sxs-lookup"><span data-stu-id="bfa63-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfa63-143">请求</span><span class="sxs-lookup"><span data-stu-id="bfa63-143">Request</span></span>
<span data-ttu-id="bfa63-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfa63-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bfa63-145">响应</span><span class="sxs-lookup"><span data-stu-id="bfa63-145">Response</span></span>
<span data-ttu-id="bfa63-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfa63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




