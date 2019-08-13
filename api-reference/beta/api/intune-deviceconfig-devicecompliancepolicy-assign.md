---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c05a30474b3c184f98f427db0eafb7523dc94764
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340217"
---
# <a name="assign-action"></a><span data-ttu-id="a1100-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="a1100-103">assign action</span></span>

> <span data-ttu-id="a1100-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1100-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1100-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1100-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1100-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1100-107">Prerequisites</span></span>
<span data-ttu-id="a1100-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1100-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1100-110">Permission type</span></span>|<span data-ttu-id="a1100-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1100-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1100-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1100-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1100-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1100-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1100-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1100-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1100-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1100-115">Not supported.</span></span>|
|<span data-ttu-id="a1100-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1100-116">Application</span></span>|<span data-ttu-id="a1100-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1100-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1100-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1100-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a1100-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1100-119">Request headers</span></span>
|<span data-ttu-id="a1100-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1100-120">Header</span></span>|<span data-ttu-id="a1100-121">值</span><span class="sxs-lookup"><span data-stu-id="a1100-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1100-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1100-122">Authorization</span></span>|<span data-ttu-id="a1100-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1100-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1100-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1100-124">Accept</span></span>|<span data-ttu-id="a1100-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1100-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1100-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1100-126">Request body</span></span>
<span data-ttu-id="a1100-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1100-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a1100-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a1100-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a1100-129">属性</span><span class="sxs-lookup"><span data-stu-id="a1100-129">Property</span></span>|<span data-ttu-id="a1100-130">类型</span><span class="sxs-lookup"><span data-stu-id="a1100-130">Type</span></span>|<span data-ttu-id="a1100-131">说明</span><span class="sxs-lookup"><span data-stu-id="a1100-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1100-132">assignments</span><span class="sxs-lookup"><span data-stu-id="a1100-132">assignments</span></span>|<span data-ttu-id="a1100-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a1100-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="a1100-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1100-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1100-135">响应</span><span class="sxs-lookup"><span data-stu-id="a1100-135">Response</span></span>
<span data-ttu-id="a1100-136">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a1100-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1100-137">示例</span><span class="sxs-lookup"><span data-stu-id="a1100-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1100-138">请求</span><span class="sxs-lookup"><span data-stu-id="a1100-138">Request</span></span>
<span data-ttu-id="a1100-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1100-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a1100-140">响应</span><span class="sxs-lookup"><span data-stu-id="a1100-140">Response</span></span>
<span data-ttu-id="a1100-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1100-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






