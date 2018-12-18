---
title: 列出 deviceCompliancePolicyAssignments
description: 列出 deviceCompliancePolicyAssignment 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: e1979293e28eb71f142f4631b636ae2f44994e80
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359092"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="eae8c-103">列出 deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="eae8c-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="eae8c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eae8c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eae8c-105">列出 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eae8c-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eae8c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="eae8c-106">Prerequisites</span></span>
<span data-ttu-id="eae8c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eae8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eae8c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eae8c-109">Permission type</span></span>|<span data-ttu-id="eae8c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eae8c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eae8c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eae8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eae8c-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eae8c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eae8c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eae8c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eae8c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eae8c-114">Not supported.</span></span>|
|<span data-ttu-id="eae8c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eae8c-115">Application</span></span>|<span data-ttu-id="eae8c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eae8c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eae8c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eae8c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="eae8c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eae8c-118">Request headers</span></span>
|<span data-ttu-id="eae8c-119">标头</span><span class="sxs-lookup"><span data-stu-id="eae8c-119">Header</span></span>|<span data-ttu-id="eae8c-120">值</span><span class="sxs-lookup"><span data-stu-id="eae8c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eae8c-121">授权</span><span class="sxs-lookup"><span data-stu-id="eae8c-121">Authorization</span></span>|<span data-ttu-id="eae8c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eae8c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eae8c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eae8c-123">Accept</span></span>|<span data-ttu-id="eae8c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eae8c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eae8c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eae8c-125">Request body</span></span>
<span data-ttu-id="eae8c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eae8c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eae8c-127">响应</span><span class="sxs-lookup"><span data-stu-id="eae8c-127">Response</span></span>
<span data-ttu-id="eae8c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eae8c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eae8c-129">示例</span><span class="sxs-lookup"><span data-stu-id="eae8c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="eae8c-130">请求</span><span class="sxs-lookup"><span data-stu-id="eae8c-130">Request</span></span>
<span data-ttu-id="eae8c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eae8c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="eae8c-132">响应</span><span class="sxs-lookup"><span data-stu-id="eae8c-132">Response</span></span>
<span data-ttu-id="eae8c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eae8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



