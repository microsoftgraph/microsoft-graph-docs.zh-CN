---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment
description: 更新 windowsDefenderApplicationControlSupplementalPolicyAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b8b88636cc7f47b1fca6a1dba59b42e0c8d6278
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938738"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="beb06-103">更新 windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="beb06-103">Update windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="beb06-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="beb06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beb06-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="beb06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb06-106">更新[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="beb06-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beb06-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="beb06-107">Prerequisites</span></span>
<span data-ttu-id="beb06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="beb06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="beb06-110">Permission type</span></span>|<span data-ttu-id="beb06-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="beb06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beb06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="beb06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="beb06-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb06-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="beb06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="beb06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beb06-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="beb06-115">Not supported.</span></span>|
|<span data-ttu-id="beb06-116">Application</span><span class="sxs-lookup"><span data-stu-id="beb06-116">Application</span></span>|<span data-ttu-id="beb06-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb06-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="beb06-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="beb06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="beb06-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="beb06-119">Request headers</span></span>
|<span data-ttu-id="beb06-120">标头</span><span class="sxs-lookup"><span data-stu-id="beb06-120">Header</span></span>|<span data-ttu-id="beb06-121">值</span><span class="sxs-lookup"><span data-stu-id="beb06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beb06-122">授权</span><span class="sxs-lookup"><span data-stu-id="beb06-122">Authorization</span></span>|<span data-ttu-id="beb06-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="beb06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beb06-124">接受</span><span class="sxs-lookup"><span data-stu-id="beb06-124">Accept</span></span>|<span data-ttu-id="beb06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="beb06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb06-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="beb06-126">Request body</span></span>
<span data-ttu-id="beb06-127">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="beb06-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

<span data-ttu-id="beb06-128">下表显示创建[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="beb06-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md).</span></span>

|<span data-ttu-id="beb06-129">属性</span><span class="sxs-lookup"><span data-stu-id="beb06-129">Property</span></span>|<span data-ttu-id="beb06-130">类型</span><span class="sxs-lookup"><span data-stu-id="beb06-130">Type</span></span>|<span data-ttu-id="beb06-131">说明</span><span class="sxs-lookup"><span data-stu-id="beb06-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb06-132">id</span><span class="sxs-lookup"><span data-stu-id="beb06-132">id</span></span>|<span data-ttu-id="beb06-133">字符串</span><span class="sxs-lookup"><span data-stu-id="beb06-133">String</span></span>|<span data-ttu-id="beb06-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="beb06-134">Key of the entity.</span></span>|
|<span data-ttu-id="beb06-135">target</span><span class="sxs-lookup"><span data-stu-id="beb06-135">target</span></span>|[<span data-ttu-id="beb06-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="beb06-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="beb06-137">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="beb06-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="beb06-138">响应</span><span class="sxs-lookup"><span data-stu-id="beb06-138">Response</span></span>
<span data-ttu-id="beb06-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="beb06-139">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb06-140">示例</span><span class="sxs-lookup"><span data-stu-id="beb06-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb06-141">请求</span><span class="sxs-lookup"><span data-stu-id="beb06-141">Request</span></span>
<span data-ttu-id="beb06-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="beb06-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
Content-type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="beb06-143">响应</span><span class="sxs-lookup"><span data-stu-id="beb06-143">Response</span></span>
<span data-ttu-id="beb06-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="beb06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





