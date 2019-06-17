---
title: assign 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3708c956f447098a7aee694c52eb61372e9b1b14
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968467"
---
# <a name="assign-action"></a><span data-ttu-id="9f2ab-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="9f2ab-103">assign action</span></span>

> <span data-ttu-id="9f2ab-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f2ab-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f2ab-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9f2ab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f2ab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f2ab-107">Prerequisites</span></span>
<span data-ttu-id="9f2ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f2ab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f2ab-110">Permission type</span></span>|<span data-ttu-id="9f2ab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f2ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f2ab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f2ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f2ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f2ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f2ab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f2ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f2ab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-115">Not supported.</span></span>|
|<span data-ttu-id="9f2ab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f2ab-116">Application</span></span>|<span data-ttu-id="9f2ab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f2ab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f2ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9f2ab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f2ab-119">Request headers</span></span>
|<span data-ttu-id="9f2ab-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f2ab-120">Header</span></span>|<span data-ttu-id="9f2ab-121">值</span><span class="sxs-lookup"><span data-stu-id="9f2ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f2ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f2ab-122">Authorization</span></span>|<span data-ttu-id="9f2ab-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f2ab-124">接受</span><span class="sxs-lookup"><span data-stu-id="9f2ab-124">Accept</span></span>|<span data-ttu-id="9f2ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f2ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f2ab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f2ab-126">Request body</span></span>
<span data-ttu-id="9f2ab-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9f2ab-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9f2ab-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f2ab-129">Property</span></span>|<span data-ttu-id="9f2ab-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f2ab-130">Type</span></span>|<span data-ttu-id="9f2ab-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f2ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f2ab-132">assignments</span><span class="sxs-lookup"><span data-stu-id="9f2ab-132">assignments</span></span>|<span data-ttu-id="9f2ab-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9f2ab-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="9f2ab-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9f2ab-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9f2ab-135">响应</span><span class="sxs-lookup"><span data-stu-id="9f2ab-135">Response</span></span>
<span data-ttu-id="9f2ab-136">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f2ab-137">示例</span><span class="sxs-lookup"><span data-stu-id="9f2ab-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f2ab-138">请求</span><span class="sxs-lookup"><span data-stu-id="9f2ab-138">Request</span></span>
<span data-ttu-id="9f2ab-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f2ab-140">响应</span><span class="sxs-lookup"><span data-stu-id="9f2ab-140">Response</span></span>
<span data-ttu-id="9f2ab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f2ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





