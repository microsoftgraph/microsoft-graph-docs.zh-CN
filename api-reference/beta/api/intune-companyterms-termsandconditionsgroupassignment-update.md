---
title: 更新 termsAndConditionsGroupAssignment
description: 更新 termsAndConditionsGroupAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea202d33028d9eff66e06030d3049f4d6fa7aef1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393751"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="40922-103">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="40922-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="40922-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="40922-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40922-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40922-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40922-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40922-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40922-107">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="40922-107">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40922-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40922-108">Prerequisites</span></span>
<span data-ttu-id="40922-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="40922-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40922-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40922-111">Permission type</span></span>|<span data-ttu-id="40922-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40922-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40922-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40922-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40922-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40922-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40922-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40922-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40922-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40922-116">Not supported.</span></span>|
|<span data-ttu-id="40922-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40922-117">Application</span></span>|<span data-ttu-id="40922-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="40922-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40922-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40922-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="40922-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40922-120">Request headers</span></span>
|<span data-ttu-id="40922-121">标头</span><span class="sxs-lookup"><span data-stu-id="40922-121">Header</span></span>|<span data-ttu-id="40922-122">值</span><span class="sxs-lookup"><span data-stu-id="40922-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40922-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40922-123">Authorization</span></span>|<span data-ttu-id="40922-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40922-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40922-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40922-125">Accept</span></span>|<span data-ttu-id="40922-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40922-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40922-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40922-127">Request body</span></span>
<span data-ttu-id="40922-128">在请求正文中，提供[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40922-128">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="40922-129">下表显示时创建[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40922-129">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="40922-130">属性</span><span class="sxs-lookup"><span data-stu-id="40922-130">Property</span></span>|<span data-ttu-id="40922-131">类型</span><span class="sxs-lookup"><span data-stu-id="40922-131">Type</span></span>|<span data-ttu-id="40922-132">说明</span><span class="sxs-lookup"><span data-stu-id="40922-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40922-133">id</span><span class="sxs-lookup"><span data-stu-id="40922-133">id</span></span>|<span data-ttu-id="40922-134">String</span><span class="sxs-lookup"><span data-stu-id="40922-134">String</span></span>|<span data-ttu-id="40922-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="40922-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="40922-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="40922-136">targetGroupId</span></span>|<span data-ttu-id="40922-137">String</span><span class="sxs-lookup"><span data-stu-id="40922-137">String</span></span>|<span data-ttu-id="40922-138">T&C 策略分配给组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="40922-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="40922-139">响应</span><span class="sxs-lookup"><span data-stu-id="40922-139">Response</span></span>
<span data-ttu-id="40922-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40922-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40922-141">示例</span><span class="sxs-lookup"><span data-stu-id="40922-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="40922-142">请求</span><span class="sxs-lookup"><span data-stu-id="40922-142">Request</span></span>
<span data-ttu-id="40922-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40922-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="40922-144">响应</span><span class="sxs-lookup"><span data-stu-id="40922-144">Response</span></span>
<span data-ttu-id="40922-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40922-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




