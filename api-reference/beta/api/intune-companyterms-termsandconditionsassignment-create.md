---
title: 创建 termsAndConditionsAssignment
description: 创建新的 termsAndConditionsAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 329bd5b227600dff42c96d54a6a0497f8b978af3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760107"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="f5d6a-103">创建 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f5d6a-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="f5d6a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5d6a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5d6a-106">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5d6a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5d6a-107">Prerequisites</span></span>
<span data-ttu-id="f5d6a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5d6a-110">Permission type</span></span>|<span data-ttu-id="f5d6a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5d6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5d6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5d6a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5d6a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f5d6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5d6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-115">Not supported.</span></span>|
|<span data-ttu-id="f5d6a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5d6a-116">Application</span></span>|<span data-ttu-id="f5d6a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5d6a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5d6a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5d6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f5d6a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5d6a-119">Request headers</span></span>
|<span data-ttu-id="f5d6a-120">标头</span><span class="sxs-lookup"><span data-stu-id="f5d6a-120">Header</span></span>|<span data-ttu-id="f5d6a-121">值</span><span class="sxs-lookup"><span data-stu-id="f5d6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5d6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5d6a-122">Authorization</span></span>|<span data-ttu-id="f5d6a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5d6a-124">接受</span><span class="sxs-lookup"><span data-stu-id="f5d6a-124">Accept</span></span>|<span data-ttu-id="f5d6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5d6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5d6a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5d6a-126">Request body</span></span>
<span data-ttu-id="f5d6a-127">在请求正文中，提供 termsAndConditionsAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="f5d6a-128">下表显示创建 termsAndConditionsAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="f5d6a-129">属性</span><span class="sxs-lookup"><span data-stu-id="f5d6a-129">Property</span></span>|<span data-ttu-id="f5d6a-130">类型</span><span class="sxs-lookup"><span data-stu-id="f5d6a-130">Type</span></span>|<span data-ttu-id="f5d6a-131">说明</span><span class="sxs-lookup"><span data-stu-id="f5d6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5d6a-132">id</span><span class="sxs-lookup"><span data-stu-id="f5d6a-132">id</span></span>|<span data-ttu-id="f5d6a-133">String</span><span class="sxs-lookup"><span data-stu-id="f5d6a-133">String</span></span>|<span data-ttu-id="f5d6a-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f5d6a-135">target</span><span class="sxs-lookup"><span data-stu-id="f5d6a-135">target</span></span>|[<span data-ttu-id="f5d6a-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f5d6a-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f5d6a-137">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="f5d6a-138">响应</span><span class="sxs-lookup"><span data-stu-id="f5d6a-138">Response</span></span>
<span data-ttu-id="f5d6a-139">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5d6a-140">示例</span><span class="sxs-lookup"><span data-stu-id="f5d6a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5d6a-141">请求</span><span class="sxs-lookup"><span data-stu-id="f5d6a-141">Request</span></span>
<span data-ttu-id="f5d6a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="f5d6a-143">响应</span><span class="sxs-lookup"><span data-stu-id="f5d6a-143">Response</span></span>
<span data-ttu-id="f5d6a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5d6a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




