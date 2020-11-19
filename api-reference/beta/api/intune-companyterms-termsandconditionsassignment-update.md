---
title: 更新 termsAndConditionsAssignment
description: 更新 termsAndConditionsAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 865dd4e6c9f17e4b683075d8dc8033141fa0b8c8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49243693"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="558d3-103">更新 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="558d3-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="558d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="558d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="558d3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="558d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="558d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="558d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="558d3-107">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="558d3-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="558d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="558d3-108">Prerequisites</span></span>
<span data-ttu-id="558d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="558d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="558d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="558d3-111">Permission type</span></span>|<span data-ttu-id="558d3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="558d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="558d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="558d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="558d3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="558d3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="558d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="558d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="558d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="558d3-116">Not supported.</span></span>|
|<span data-ttu-id="558d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="558d3-117">Application</span></span>|<span data-ttu-id="558d3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="558d3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="558d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="558d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="558d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="558d3-120">Request headers</span></span>
|<span data-ttu-id="558d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="558d3-121">Header</span></span>|<span data-ttu-id="558d3-122">值</span><span class="sxs-lookup"><span data-stu-id="558d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="558d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="558d3-123">Authorization</span></span>|<span data-ttu-id="558d3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="558d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="558d3-125">接受</span><span class="sxs-lookup"><span data-stu-id="558d3-125">Accept</span></span>|<span data-ttu-id="558d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="558d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="558d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="558d3-127">Request body</span></span>
<span data-ttu-id="558d3-128">在请求正文中，提供 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="558d3-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="558d3-129">下表显示创建 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="558d3-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="558d3-130">属性</span><span class="sxs-lookup"><span data-stu-id="558d3-130">Property</span></span>|<span data-ttu-id="558d3-131">类型</span><span class="sxs-lookup"><span data-stu-id="558d3-131">Type</span></span>|<span data-ttu-id="558d3-132">说明</span><span class="sxs-lookup"><span data-stu-id="558d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558d3-133">id</span><span class="sxs-lookup"><span data-stu-id="558d3-133">id</span></span>|<span data-ttu-id="558d3-134">String</span><span class="sxs-lookup"><span data-stu-id="558d3-134">String</span></span>|<span data-ttu-id="558d3-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="558d3-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="558d3-136">target</span><span class="sxs-lookup"><span data-stu-id="558d3-136">target</span></span>|[<span data-ttu-id="558d3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="558d3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="558d3-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="558d3-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="558d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="558d3-139">Response</span></span>
<span data-ttu-id="558d3-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="558d3-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="558d3-141">示例</span><span class="sxs-lookup"><span data-stu-id="558d3-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="558d3-142">请求</span><span class="sxs-lookup"><span data-stu-id="558d3-142">Request</span></span>
<span data-ttu-id="558d3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="558d3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="558d3-144">响应</span><span class="sxs-lookup"><span data-stu-id="558d3-144">Response</span></span>
<span data-ttu-id="558d3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="558d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




