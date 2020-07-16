---
title: 更新 termsAndConditionsAssignment
description: 更新 termsAndConditionsAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 794c73484141607f5ef5d6d9f1144ce8316c9cfc
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793155"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="7f62e-103">更新 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7f62e-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="7f62e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f62e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f62e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f62e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f62e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f62e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f62e-107">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7f62e-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f62e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f62e-108">Prerequisites</span></span>
<span data-ttu-id="7f62e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f62e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f62e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f62e-111">Permission type</span></span>|<span data-ttu-id="7f62e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f62e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f62e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f62e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f62e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f62e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f62e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f62e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f62e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f62e-116">Not supported.</span></span>|
|<span data-ttu-id="7f62e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f62e-117">Application</span></span>|<span data-ttu-id="7f62e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f62e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f62e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f62e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7f62e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f62e-120">Request headers</span></span>
|<span data-ttu-id="7f62e-121">标头</span><span class="sxs-lookup"><span data-stu-id="7f62e-121">Header</span></span>|<span data-ttu-id="7f62e-122">值</span><span class="sxs-lookup"><span data-stu-id="7f62e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f62e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f62e-123">Authorization</span></span>|<span data-ttu-id="7f62e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f62e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f62e-125">接受</span><span class="sxs-lookup"><span data-stu-id="7f62e-125">Accept</span></span>|<span data-ttu-id="7f62e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f62e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f62e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f62e-127">Request body</span></span>
<span data-ttu-id="7f62e-128">在请求正文中，提供 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f62e-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="7f62e-129">下表显示创建 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f62e-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="7f62e-130">属性</span><span class="sxs-lookup"><span data-stu-id="7f62e-130">Property</span></span>|<span data-ttu-id="7f62e-131">类型</span><span class="sxs-lookup"><span data-stu-id="7f62e-131">Type</span></span>|<span data-ttu-id="7f62e-132">说明</span><span class="sxs-lookup"><span data-stu-id="7f62e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f62e-133">id</span><span class="sxs-lookup"><span data-stu-id="7f62e-133">id</span></span>|<span data-ttu-id="7f62e-134">String</span><span class="sxs-lookup"><span data-stu-id="7f62e-134">String</span></span>|<span data-ttu-id="7f62e-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7f62e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7f62e-136">target</span><span class="sxs-lookup"><span data-stu-id="7f62e-136">target</span></span>|[<span data-ttu-id="7f62e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f62e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f62e-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="7f62e-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7f62e-139">响应</span><span class="sxs-lookup"><span data-stu-id="7f62e-139">Response</span></span>
<span data-ttu-id="7f62e-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f62e-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f62e-141">示例</span><span class="sxs-lookup"><span data-stu-id="7f62e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f62e-142">请求</span><span class="sxs-lookup"><span data-stu-id="7f62e-142">Request</span></span>
<span data-ttu-id="7f62e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f62e-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f62e-144">响应</span><span class="sxs-lookup"><span data-stu-id="7f62e-144">Response</span></span>
<span data-ttu-id="7f62e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f62e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



