---
title: 创建 deviceCompliancePolicyAssignment
description: 创建新的 deviceCompliancePolicyAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 541d4af1f1daab4efce46088561128e219068b2f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980942"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="1a4ba-103">创建 deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="1a4ba-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="1a4ba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a4ba-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a4ba-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a4ba-107">创建新的 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1a4ba-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a4ba-108">Prerequisites</span></span>
<span data-ttu-id="1a4ba-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1a4ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a4ba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a4ba-111">Permission type</span></span>|<span data-ttu-id="1a4ba-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a4ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a4ba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a4ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a4ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a4ba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a4ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-116">Not supported.</span></span>|
|<span data-ttu-id="1a4ba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a4ba-117">Application</span></span>|<span data-ttu-id="1a4ba-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a4ba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a4ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1a4ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a4ba-120">Request headers</span></span>
|<span data-ttu-id="1a4ba-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a4ba-121">Header</span></span>|<span data-ttu-id="1a4ba-122">值</span><span class="sxs-lookup"><span data-stu-id="1a4ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a4ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a4ba-123">Authorization</span></span>|<span data-ttu-id="1a4ba-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a4ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a4ba-125">Accept</span></span>|<span data-ttu-id="1a4ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a4ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a4ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a4ba-127">Request body</span></span>
<span data-ttu-id="1a4ba-128">在请求正文中，提供 deviceCompliancePolicyAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="1a4ba-129">下表显示创建 deviceCompliancePolicyAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="1a4ba-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a4ba-130">Property</span></span>|<span data-ttu-id="1a4ba-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a4ba-131">Type</span></span>|<span data-ttu-id="1a4ba-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a4ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a4ba-133">id</span><span class="sxs-lookup"><span data-stu-id="1a4ba-133">id</span></span>|<span data-ttu-id="1a4ba-134">String</span><span class="sxs-lookup"><span data-stu-id="1a4ba-134">String</span></span>|<span data-ttu-id="1a4ba-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-135">Key of the entity.</span></span>|
|<span data-ttu-id="1a4ba-136">target</span><span class="sxs-lookup"><span data-stu-id="1a4ba-136">target</span></span>|[<span data-ttu-id="1a4ba-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1a4ba-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1a4ba-138">符合性策略分配目标。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="1a4ba-139">响应</span><span class="sxs-lookup"><span data-stu-id="1a4ba-139">Response</span></span>
<span data-ttu-id="1a4ba-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a4ba-141">示例</span><span class="sxs-lookup"><span data-stu-id="1a4ba-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1a4ba-142">请求</span><span class="sxs-lookup"><span data-stu-id="1a4ba-142">Request</span></span>
<span data-ttu-id="1a4ba-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1a4ba-144">响应</span><span class="sxs-lookup"><span data-stu-id="1a4ba-144">Response</span></span>
<span data-ttu-id="1a4ba-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a4ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





