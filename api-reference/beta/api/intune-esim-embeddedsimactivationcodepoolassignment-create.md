---
title: 创建 embeddedSIMActivationCodePoolAssignment
description: 创建新的 embeddedSIMActivationCodePoolAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cda2263ff1df6232b70f0831ed2c02d7387d84fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126106"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="8385e-103">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="8385e-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="8385e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8385e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8385e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8385e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8385e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8385e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8385e-107">创建新的 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8385e-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8385e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8385e-108">Prerequisites</span></span>
<span data-ttu-id="8385e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8385e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8385e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8385e-111">Permission type</span></span>|<span data-ttu-id="8385e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8385e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8385e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8385e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8385e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8385e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8385e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8385e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8385e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8385e-116">Not supported.</span></span>|
|<span data-ttu-id="8385e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8385e-117">Application</span></span>|<span data-ttu-id="8385e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8385e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8385e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8385e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8385e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8385e-120">Request headers</span></span>
|<span data-ttu-id="8385e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8385e-121">Header</span></span>|<span data-ttu-id="8385e-122">值</span><span class="sxs-lookup"><span data-stu-id="8385e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8385e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8385e-123">Authorization</span></span>|<span data-ttu-id="8385e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8385e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8385e-125">接受</span><span class="sxs-lookup"><span data-stu-id="8385e-125">Accept</span></span>|<span data-ttu-id="8385e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8385e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8385e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8385e-127">Request body</span></span>
<span data-ttu-id="8385e-128">在请求正文中，提供 embeddedSIMActivationCodePoolAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8385e-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="8385e-129">下表显示创建 embeddedSIMActivationCodePoolAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8385e-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="8385e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8385e-130">Property</span></span>|<span data-ttu-id="8385e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8385e-131">Type</span></span>|<span data-ttu-id="8385e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8385e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8385e-133">id</span><span class="sxs-lookup"><span data-stu-id="8385e-133">id</span></span>|<span data-ttu-id="8385e-134">String</span><span class="sxs-lookup"><span data-stu-id="8385e-134">String</span></span>|<span data-ttu-id="8385e-135">嵌入式 SIM 卡激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8385e-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="8385e-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="8385e-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="8385e-137">target</span><span class="sxs-lookup"><span data-stu-id="8385e-137">target</span></span>|[<span data-ttu-id="8385e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8385e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8385e-139">嵌入式 SIM 卡激活代码池所面向的组类型。</span><span class="sxs-lookup"><span data-stu-id="8385e-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="8385e-140">响应</span><span class="sxs-lookup"><span data-stu-id="8385e-140">Response</span></span>
<span data-ttu-id="8385e-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8385e-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8385e-142">示例</span><span class="sxs-lookup"><span data-stu-id="8385e-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8385e-143">请求</span><span class="sxs-lookup"><span data-stu-id="8385e-143">Request</span></span>
<span data-ttu-id="8385e-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8385e-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 340

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="8385e-145">响应</span><span class="sxs-lookup"><span data-stu-id="8385e-145">Response</span></span>
<span data-ttu-id="8385e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8385e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




