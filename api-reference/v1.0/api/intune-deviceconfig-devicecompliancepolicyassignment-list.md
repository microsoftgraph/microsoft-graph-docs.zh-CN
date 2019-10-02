---
title: 列出 deviceCompliancePolicyAssignments
description: 列出 deviceCompliancePolicyAssignment 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4c561d9d200f3a420a4cb6cc6faaa3971dbfa54
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37369021"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="88633-103">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="88633-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="88633-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88633-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88633-105">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88633-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88633-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="88633-106">Prerequisites</span></span>
<span data-ttu-id="88633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88633-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88633-109">Permission type</span></span>|<span data-ttu-id="88633-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88633-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88633-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88633-111">Delegated (work or school account)</span></span>|<span data-ttu-id="88633-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88633-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="88633-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88633-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88633-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88633-114">Not supported.</span></span>|
|<span data-ttu-id="88633-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88633-115">Application</span></span>|<span data-ttu-id="88633-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88633-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88633-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88633-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="88633-118">请求头</span><span class="sxs-lookup"><span data-stu-id="88633-118">Request headers</span></span>
|<span data-ttu-id="88633-119">标头</span><span class="sxs-lookup"><span data-stu-id="88633-119">Header</span></span>|<span data-ttu-id="88633-120">值</span><span class="sxs-lookup"><span data-stu-id="88633-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88633-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88633-121">Authorization</span></span>|<span data-ttu-id="88633-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88633-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88633-123">接受</span><span class="sxs-lookup"><span data-stu-id="88633-123">Accept</span></span>|<span data-ttu-id="88633-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88633-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88633-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="88633-125">Request body</span></span>
<span data-ttu-id="88633-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88633-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88633-127">响应</span><span class="sxs-lookup"><span data-stu-id="88633-127">Response</span></span>
<span data-ttu-id="88633-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="88633-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88633-129">示例</span><span class="sxs-lookup"><span data-stu-id="88633-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="88633-130">请求</span><span class="sxs-lookup"><span data-stu-id="88633-130">Request</span></span>
<span data-ttu-id="88633-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88633-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="88633-132">响应</span><span class="sxs-lookup"><span data-stu-id="88633-132">Response</span></span>
<span data-ttu-id="88633-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88633-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




