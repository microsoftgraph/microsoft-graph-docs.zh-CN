---
title: 列出 deviceCompliancePolicyAssignments
description: 列出 deviceCompliancePolicyAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 047f8b3c6bb1fb5c4ca2113a72abcb32fad84130
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263957"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="a837f-103">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="a837f-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="a837f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a837f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a837f-105">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a837f-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a837f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a837f-106">Prerequisites</span></span>
<span data-ttu-id="a837f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a837f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a837f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a837f-109">Permission type</span></span>|<span data-ttu-id="a837f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a837f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a837f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a837f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a837f-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a837f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a837f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a837f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a837f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a837f-114">Not supported.</span></span>|
|<span data-ttu-id="a837f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a837f-115">Application</span></span>|<span data-ttu-id="a837f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a837f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a837f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a837f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a837f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a837f-118">Request headers</span></span>
|<span data-ttu-id="a837f-119">标头</span><span class="sxs-lookup"><span data-stu-id="a837f-119">Header</span></span>|<span data-ttu-id="a837f-120">值</span><span class="sxs-lookup"><span data-stu-id="a837f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a837f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a837f-121">Authorization</span></span>|<span data-ttu-id="a837f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a837f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a837f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a837f-123">Accept</span></span>|<span data-ttu-id="a837f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a837f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a837f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a837f-125">Request body</span></span>
<span data-ttu-id="a837f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a837f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a837f-127">响应</span><span class="sxs-lookup"><span data-stu-id="a837f-127">Response</span></span>
<span data-ttu-id="a837f-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a837f-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a837f-129">示例</span><span class="sxs-lookup"><span data-stu-id="a837f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a837f-130">请求</span><span class="sxs-lookup"><span data-stu-id="a837f-130">Request</span></span>
<span data-ttu-id="a837f-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a837f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="a837f-132">响应</span><span class="sxs-lookup"><span data-stu-id="a837f-132">Response</span></span>
<span data-ttu-id="a837f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a837f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



