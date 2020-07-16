---
title: 获取 deviceCompliancePolicyAssignment
description: 读取 deviceCompliancePolicyAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3acc06ae3e73a360708955dde12fe4b081b25aa7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793036"
---
# <a name="get-devicecompliancepolicyassignment"></a><span data-ttu-id="29efb-103">获取 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="29efb-103">Get deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="29efb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29efb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29efb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29efb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29efb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29efb-107">读取 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29efb-107">Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29efb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29efb-108">Prerequisites</span></span>
<span data-ttu-id="29efb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29efb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29efb-111">Permission type</span></span>|<span data-ttu-id="29efb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29efb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29efb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29efb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29efb-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="29efb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="29efb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29efb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29efb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29efb-116">Not supported.</span></span>|
|<span data-ttu-id="29efb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29efb-117">Application</span></span>|<span data-ttu-id="29efb-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="29efb-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29efb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29efb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29efb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="29efb-120">Optional query parameters</span></span>
<span data-ttu-id="29efb-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="29efb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29efb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="29efb-122">Request headers</span></span>
|<span data-ttu-id="29efb-123">标头</span><span class="sxs-lookup"><span data-stu-id="29efb-123">Header</span></span>|<span data-ttu-id="29efb-124">值</span><span class="sxs-lookup"><span data-stu-id="29efb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29efb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="29efb-125">Authorization</span></span>|<span data-ttu-id="29efb-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29efb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29efb-127">接受</span><span class="sxs-lookup"><span data-stu-id="29efb-127">Accept</span></span>|<span data-ttu-id="29efb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29efb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29efb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="29efb-129">Request body</span></span>
<span data-ttu-id="29efb-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29efb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29efb-131">响应</span><span class="sxs-lookup"><span data-stu-id="29efb-131">Response</span></span>
<span data-ttu-id="29efb-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29efb-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29efb-133">示例</span><span class="sxs-lookup"><span data-stu-id="29efb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="29efb-134">请求</span><span class="sxs-lookup"><span data-stu-id="29efb-134">Request</span></span>
<span data-ttu-id="29efb-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29efb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="29efb-136">响应</span><span class="sxs-lookup"><span data-stu-id="29efb-136">Response</span></span>
<span data-ttu-id="29efb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29efb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
    "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```



