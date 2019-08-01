---
title: 更新 termsAndConditionsAssignment
description: 更新 termsAndConditionsAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df64ab26d09093b9eebb08698a9cfed4cb9e86f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020393"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="3de3a-103">更新 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3de3a-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="3de3a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3de3a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de3a-105">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3de3a-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3de3a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3de3a-106">Prerequisites</span></span>
<span data-ttu-id="3de3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3de3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3de3a-109">Permission type</span></span>|<span data-ttu-id="3de3a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3de3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3de3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3de3a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de3a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3de3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3de3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3de3a-114">Not supported.</span></span>|
|<span data-ttu-id="3de3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3de3a-115">Application</span></span>|<span data-ttu-id="3de3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3de3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3de3a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3de3a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3de3a-118">Request headers</span></span>
|<span data-ttu-id="3de3a-119">标头</span><span class="sxs-lookup"><span data-stu-id="3de3a-119">Header</span></span>|<span data-ttu-id="3de3a-120">值</span><span class="sxs-lookup"><span data-stu-id="3de3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3de3a-121">Authorization</span></span>|<span data-ttu-id="3de3a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3de3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de3a-123">接受</span><span class="sxs-lookup"><span data-stu-id="3de3a-123">Accept</span></span>|<span data-ttu-id="3de3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3de3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de3a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3de3a-125">Request body</span></span>
<span data-ttu-id="3de3a-126">在请求正文中，提供 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3de3a-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="3de3a-127">下表显示创建 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3de3a-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="3de3a-128">属性</span><span class="sxs-lookup"><span data-stu-id="3de3a-128">Property</span></span>|<span data-ttu-id="3de3a-129">类型</span><span class="sxs-lookup"><span data-stu-id="3de3a-129">Type</span></span>|<span data-ttu-id="3de3a-130">说明</span><span class="sxs-lookup"><span data-stu-id="3de3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de3a-131">id</span><span class="sxs-lookup"><span data-stu-id="3de3a-131">id</span></span>|<span data-ttu-id="3de3a-132">String</span><span class="sxs-lookup"><span data-stu-id="3de3a-132">String</span></span>|<span data-ttu-id="3de3a-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3de3a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3de3a-134">target</span><span class="sxs-lookup"><span data-stu-id="3de3a-134">target</span></span>|[<span data-ttu-id="3de3a-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3de3a-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3de3a-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="3de3a-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="3de3a-137">响应</span><span class="sxs-lookup"><span data-stu-id="3de3a-137">Response</span></span>
<span data-ttu-id="3de3a-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3de3a-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de3a-139">示例</span><span class="sxs-lookup"><span data-stu-id="3de3a-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de3a-140">请求</span><span class="sxs-lookup"><span data-stu-id="3de3a-140">Request</span></span>
<span data-ttu-id="3de3a-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3de3a-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3de3a-142">响应</span><span class="sxs-lookup"><span data-stu-id="3de3a-142">Response</span></span>
<span data-ttu-id="3de3a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3de3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



