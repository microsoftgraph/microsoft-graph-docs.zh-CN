---
title: assign 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dfe23249462a1bd637995fcc1af42aff74c344cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807740"
---
# <a name="assign-action"></a><span data-ttu-id="21630-103">assign 操作</span><span class="sxs-lookup"><span data-stu-id="21630-103">assign action</span></span>

> <span data-ttu-id="21630-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21630-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21630-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21630-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21630-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21630-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21630-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21630-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21630-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="21630-108">Prerequisites</span></span>
<span data-ttu-id="21630-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="21630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21630-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21630-111">Permission type</span></span>|<span data-ttu-id="21630-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21630-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21630-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21630-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21630-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21630-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21630-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21630-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21630-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21630-116">Not supported.</span></span>|
|<span data-ttu-id="21630-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="21630-117">Application</span></span>|<span data-ttu-id="21630-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="21630-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21630-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21630-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="21630-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="21630-120">Request headers</span></span>
|<span data-ttu-id="21630-121">标头</span><span class="sxs-lookup"><span data-stu-id="21630-121">Header</span></span>|<span data-ttu-id="21630-122">值</span><span class="sxs-lookup"><span data-stu-id="21630-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21630-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21630-123">Authorization</span></span>|<span data-ttu-id="21630-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21630-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21630-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21630-125">Accept</span></span>|<span data-ttu-id="21630-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21630-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21630-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="21630-127">Request body</span></span>
<span data-ttu-id="21630-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21630-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="21630-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="21630-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="21630-130">属性</span><span class="sxs-lookup"><span data-stu-id="21630-130">Property</span></span>|<span data-ttu-id="21630-131">类型</span><span class="sxs-lookup"><span data-stu-id="21630-131">Type</span></span>|<span data-ttu-id="21630-132">说明</span><span class="sxs-lookup"><span data-stu-id="21630-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21630-133">assignments</span><span class="sxs-lookup"><span data-stu-id="21630-133">assignments</span></span>|<span data-ttu-id="21630-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21630-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="21630-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="21630-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="21630-136">响应</span><span class="sxs-lookup"><span data-stu-id="21630-136">Response</span></span>
<span data-ttu-id="21630-137">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="21630-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21630-138">示例</span><span class="sxs-lookup"><span data-stu-id="21630-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="21630-139">请求</span><span class="sxs-lookup"><span data-stu-id="21630-139">Request</span></span>
<span data-ttu-id="21630-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21630-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21630-141">响应</span><span class="sxs-lookup"><span data-stu-id="21630-141">Response</span></span>
<span data-ttu-id="21630-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21630-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





