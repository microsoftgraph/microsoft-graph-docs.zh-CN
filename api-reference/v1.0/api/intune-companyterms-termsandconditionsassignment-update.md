---
title: 更新 termsAndConditionsAssignment
description: 更新 termsAndConditionsAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: b55ec01c6bac55f9b1d72a5aad5f931bed6b6b2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301405"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="04a63-103">更新 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="04a63-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="04a63-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04a63-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04a63-105">更新 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04a63-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04a63-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="04a63-106">Prerequisites</span></span>
<span data-ttu-id="04a63-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="04a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04a63-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04a63-109">Permission type</span></span>|<span data-ttu-id="04a63-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04a63-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04a63-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04a63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04a63-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04a63-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04a63-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04a63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04a63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04a63-114">Not supported.</span></span>|
|<span data-ttu-id="04a63-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04a63-115">Application</span></span>|<span data-ttu-id="04a63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04a63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04a63-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04a63-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="04a63-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04a63-118">Request headers</span></span>
|<span data-ttu-id="04a63-119">标头</span><span class="sxs-lookup"><span data-stu-id="04a63-119">Header</span></span>|<span data-ttu-id="04a63-120">值</span><span class="sxs-lookup"><span data-stu-id="04a63-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04a63-121">授权</span><span class="sxs-lookup"><span data-stu-id="04a63-121">Authorization</span></span>|<span data-ttu-id="04a63-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04a63-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04a63-123">Accept</span><span class="sxs-lookup"><span data-stu-id="04a63-123">Accept</span></span>|<span data-ttu-id="04a63-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04a63-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04a63-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="04a63-125">Request body</span></span>
<span data-ttu-id="04a63-126">在请求正文中，提供 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04a63-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="04a63-127">下表显示创建 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04a63-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="04a63-128">属性</span><span class="sxs-lookup"><span data-stu-id="04a63-128">Property</span></span>|<span data-ttu-id="04a63-129">类型</span><span class="sxs-lookup"><span data-stu-id="04a63-129">Type</span></span>|<span data-ttu-id="04a63-130">说明</span><span class="sxs-lookup"><span data-stu-id="04a63-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a63-131">id</span><span class="sxs-lookup"><span data-stu-id="04a63-131">id</span></span>|<span data-ttu-id="04a63-132">String</span><span class="sxs-lookup"><span data-stu-id="04a63-132">String</span></span>|<span data-ttu-id="04a63-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="04a63-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="04a63-134">target</span><span class="sxs-lookup"><span data-stu-id="04a63-134">target</span></span>|[<span data-ttu-id="04a63-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04a63-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04a63-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="04a63-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="04a63-137">响应</span><span class="sxs-lookup"><span data-stu-id="04a63-137">Response</span></span>
<span data-ttu-id="04a63-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04a63-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04a63-139">示例</span><span class="sxs-lookup"><span data-stu-id="04a63-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="04a63-140">请求</span><span class="sxs-lookup"><span data-stu-id="04a63-140">Request</span></span>
<span data-ttu-id="04a63-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04a63-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04a63-142">响应</span><span class="sxs-lookup"><span data-stu-id="04a63-142">Response</span></span>
<span data-ttu-id="04a63-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04a63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



