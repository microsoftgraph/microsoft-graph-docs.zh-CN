---
title: 创建 embeddedSIMActivationCodePoolAssignment
description: 创建新的 embeddedSIMActivationCodePoolAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56f7f98ff0004ed08664b1635cc77436c69d1c7b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943584"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="ef251-103">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="ef251-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="ef251-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef251-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef251-106">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef251-106">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef251-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef251-107">Prerequisites</span></span>
<span data-ttu-id="ef251-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef251-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef251-110">Permission type</span></span>|<span data-ttu-id="ef251-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef251-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef251-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef251-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef251-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef251-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef251-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef251-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef251-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef251-115">Not supported.</span></span>|
|<span data-ttu-id="ef251-116">Application</span><span class="sxs-lookup"><span data-stu-id="ef251-116">Application</span></span>|<span data-ttu-id="ef251-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef251-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef251-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef251-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ef251-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef251-119">Request headers</span></span>
|<span data-ttu-id="ef251-120">标头</span><span class="sxs-lookup"><span data-stu-id="ef251-120">Header</span></span>|<span data-ttu-id="ef251-121">值</span><span class="sxs-lookup"><span data-stu-id="ef251-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef251-122">授权</span><span class="sxs-lookup"><span data-stu-id="ef251-122">Authorization</span></span>|<span data-ttu-id="ef251-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef251-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef251-124">接受</span><span class="sxs-lookup"><span data-stu-id="ef251-124">Accept</span></span>|<span data-ttu-id="ef251-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef251-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef251-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef251-126">Request body</span></span>
<span data-ttu-id="ef251-127">在请求正文中，提供 embeddedSIMActivationCodePoolAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef251-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="ef251-128">下表显示创建 embeddedSIMActivationCodePoolAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef251-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="ef251-129">属性</span><span class="sxs-lookup"><span data-stu-id="ef251-129">Property</span></span>|<span data-ttu-id="ef251-130">类型</span><span class="sxs-lookup"><span data-stu-id="ef251-130">Type</span></span>|<span data-ttu-id="ef251-131">说明</span><span class="sxs-lookup"><span data-stu-id="ef251-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef251-132">id</span><span class="sxs-lookup"><span data-stu-id="ef251-132">id</span></span>|<span data-ttu-id="ef251-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ef251-133">String</span></span>|<span data-ttu-id="ef251-134">嵌入的 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ef251-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="ef251-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="ef251-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="ef251-136">target</span><span class="sxs-lookup"><span data-stu-id="ef251-136">target</span></span>|[<span data-ttu-id="ef251-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef251-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ef251-138">嵌入的 SIM 激活代码池的目标组的类型。</span><span class="sxs-lookup"><span data-stu-id="ef251-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="ef251-139">响应</span><span class="sxs-lookup"><span data-stu-id="ef251-139">Response</span></span>
<span data-ttu-id="ef251-140">如果成功，此方法在响应`201 Created`正文中返回响应代码和[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ef251-140">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef251-141">示例</span><span class="sxs-lookup"><span data-stu-id="ef251-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef251-142">请求</span><span class="sxs-lookup"><span data-stu-id="ef251-142">Request</span></span>
<span data-ttu-id="ef251-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef251-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ef251-144">响应</span><span class="sxs-lookup"><span data-stu-id="ef251-144">Response</span></span>
<span data-ttu-id="ef251-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef251-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





