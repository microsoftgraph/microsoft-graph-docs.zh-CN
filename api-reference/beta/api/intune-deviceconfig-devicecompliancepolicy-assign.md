---
title: assign 操作
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: ffac5ff9eb3cbc5ed3687954c7bbd518f340fda8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342880"
---
# <a name="assign-action"></a><span data-ttu-id="cf7c8-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="cf7c8-103">assign action</span></span>

> <span data-ttu-id="cf7c8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf7c8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf7c8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf7c8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf7c8-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf7c8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf7c8-108">Prerequisites</span></span>
<span data-ttu-id="cf7c8-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cf7c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf7c8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf7c8-111">Permission type</span></span>|<span data-ttu-id="cf7c8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf7c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf7c8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf7c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf7c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf7c8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf7c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-116">Not supported.</span></span>|
|<span data-ttu-id="cf7c8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf7c8-117">Application</span></span>|<span data-ttu-id="cf7c8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf7c8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf7c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="cf7c8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf7c8-120">Request headers</span></span>
|<span data-ttu-id="cf7c8-121">标头</span><span class="sxs-lookup"><span data-stu-id="cf7c8-121">Header</span></span>|<span data-ttu-id="cf7c8-122">值</span><span class="sxs-lookup"><span data-stu-id="cf7c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf7c8-123">授权</span><span class="sxs-lookup"><span data-stu-id="cf7c8-123">Authorization</span></span>|<span data-ttu-id="cf7c8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf7c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf7c8-125">Accept</span></span>|<span data-ttu-id="cf7c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf7c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf7c8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf7c8-127">Request body</span></span>
<span data-ttu-id="cf7c8-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cf7c8-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cf7c8-130">属性</span><span class="sxs-lookup"><span data-stu-id="cf7c8-130">Property</span></span>|<span data-ttu-id="cf7c8-131">类型</span><span class="sxs-lookup"><span data-stu-id="cf7c8-131">Type</span></span>|<span data-ttu-id="cf7c8-132">说明</span><span class="sxs-lookup"><span data-stu-id="cf7c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf7c8-133">assignments</span><span class="sxs-lookup"><span data-stu-id="cf7c8-133">assignments</span></span>|<span data-ttu-id="cf7c8-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cf7c8-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="cf7c8-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf7c8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cf7c8-136">响应</span><span class="sxs-lookup"><span data-stu-id="cf7c8-136">Response</span></span>
<span data-ttu-id="cf7c8-137">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7c8-138">示例</span><span class="sxs-lookup"><span data-stu-id="cf7c8-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf7c8-139">请求</span><span class="sxs-lookup"><span data-stu-id="cf7c8-139">Request</span></span>
<span data-ttu-id="cf7c8-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf7c8-141">响应</span><span class="sxs-lookup"><span data-stu-id="cf7c8-141">Response</span></span>
<span data-ttu-id="cf7c8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf7c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





