---
title: 更新 termsAndConditionsGroupAssignment
description: 更新 termsAndConditionsGroupAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 650477e810035039cdc9513ac41a387539fb761c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804016"
---
# <a name="update-termsandconditionsgroupassignment"></a><span data-ttu-id="d238b-103">更新 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d238b-103">Update termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="d238b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d238b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d238b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d238b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d238b-106">更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d238b-106">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d238b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d238b-107">Prerequisites</span></span>
<span data-ttu-id="d238b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d238b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d238b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d238b-110">Permission type</span></span>|<span data-ttu-id="d238b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d238b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d238b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d238b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d238b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d238b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d238b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d238b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d238b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d238b-115">Not supported.</span></span>|
|<span data-ttu-id="d238b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d238b-116">Application</span></span>|<span data-ttu-id="d238b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d238b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d238b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d238b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d238b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d238b-119">Request headers</span></span>
|<span data-ttu-id="d238b-120">标头</span><span class="sxs-lookup"><span data-stu-id="d238b-120">Header</span></span>|<span data-ttu-id="d238b-121">值</span><span class="sxs-lookup"><span data-stu-id="d238b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d238b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d238b-122">Authorization</span></span>|<span data-ttu-id="d238b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d238b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d238b-124">接受</span><span class="sxs-lookup"><span data-stu-id="d238b-124">Accept</span></span>|<span data-ttu-id="d238b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d238b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d238b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d238b-126">Request body</span></span>
<span data-ttu-id="d238b-127">在请求正文中, 提供[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d238b-127">In the request body, supply a JSON representation for the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

<span data-ttu-id="d238b-128">下表显示创建[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d238b-128">The following table shows the properties that are required when you create the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>

|<span data-ttu-id="d238b-129">属性</span><span class="sxs-lookup"><span data-stu-id="d238b-129">Property</span></span>|<span data-ttu-id="d238b-130">类型</span><span class="sxs-lookup"><span data-stu-id="d238b-130">Type</span></span>|<span data-ttu-id="d238b-131">说明</span><span class="sxs-lookup"><span data-stu-id="d238b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d238b-132">id</span><span class="sxs-lookup"><span data-stu-id="d238b-132">id</span></span>|<span data-ttu-id="d238b-133">String</span><span class="sxs-lookup"><span data-stu-id="d238b-133">String</span></span>|<span data-ttu-id="d238b-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d238b-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d238b-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d238b-135">targetGroupId</span></span>|<span data-ttu-id="d238b-136">String</span><span class="sxs-lookup"><span data-stu-id="d238b-136">String</span></span>|<span data-ttu-id="d238b-137">向其分配 T&C 策略的组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d238b-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d238b-138">响应</span><span class="sxs-lookup"><span data-stu-id="d238b-138">Response</span></span>
<span data-ttu-id="d238b-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d238b-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d238b-140">示例</span><span class="sxs-lookup"><span data-stu-id="d238b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d238b-141">请求</span><span class="sxs-lookup"><span data-stu-id="d238b-141">Request</span></span>
<span data-ttu-id="d238b-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d238b-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="d238b-143">响应</span><span class="sxs-lookup"><span data-stu-id="d238b-143">Response</span></span>
<span data-ttu-id="d238b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d238b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





