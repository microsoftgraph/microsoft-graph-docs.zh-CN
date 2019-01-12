---
title: 创建 termsAndConditionsAssignment
description: 创建新的 termsAndConditionsAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 704aa0a3f86c3b65b3f2882af21010c46c02f1b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976133"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="39ec7-103">创建 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="39ec7-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="39ec7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39ec7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39ec7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39ec7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39ec7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39ec7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39ec7-107">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39ec7-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39ec7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="39ec7-108">Prerequisites</span></span>
<span data-ttu-id="39ec7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="39ec7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ec7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39ec7-111">Permission type</span></span>|<span data-ttu-id="39ec7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39ec7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39ec7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39ec7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39ec7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ec7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="39ec7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39ec7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39ec7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39ec7-116">Not supported.</span></span>|
|<span data-ttu-id="39ec7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39ec7-117">Application</span></span>|<span data-ttu-id="39ec7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="39ec7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39ec7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39ec7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="39ec7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="39ec7-120">Request headers</span></span>
|<span data-ttu-id="39ec7-121">标头</span><span class="sxs-lookup"><span data-stu-id="39ec7-121">Header</span></span>|<span data-ttu-id="39ec7-122">值</span><span class="sxs-lookup"><span data-stu-id="39ec7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39ec7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39ec7-123">Authorization</span></span>|<span data-ttu-id="39ec7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39ec7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39ec7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39ec7-125">Accept</span></span>|<span data-ttu-id="39ec7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39ec7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39ec7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39ec7-127">Request body</span></span>
<span data-ttu-id="39ec7-128">在请求正文中，提供 termsAndConditionsAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39ec7-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="39ec7-129">下表显示创建 termsAndConditionsAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="39ec7-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="39ec7-130">属性</span><span class="sxs-lookup"><span data-stu-id="39ec7-130">Property</span></span>|<span data-ttu-id="39ec7-131">类型</span><span class="sxs-lookup"><span data-stu-id="39ec7-131">Type</span></span>|<span data-ttu-id="39ec7-132">说明</span><span class="sxs-lookup"><span data-stu-id="39ec7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ec7-133">id</span><span class="sxs-lookup"><span data-stu-id="39ec7-133">id</span></span>|<span data-ttu-id="39ec7-134">String</span><span class="sxs-lookup"><span data-stu-id="39ec7-134">String</span></span>|<span data-ttu-id="39ec7-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="39ec7-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="39ec7-136">target</span><span class="sxs-lookup"><span data-stu-id="39ec7-136">target</span></span>|[<span data-ttu-id="39ec7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="39ec7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="39ec7-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="39ec7-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="39ec7-139">响应</span><span class="sxs-lookup"><span data-stu-id="39ec7-139">Response</span></span>
<span data-ttu-id="39ec7-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39ec7-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39ec7-141">示例</span><span class="sxs-lookup"><span data-stu-id="39ec7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="39ec7-142">请求</span><span class="sxs-lookup"><span data-stu-id="39ec7-142">Request</span></span>
<span data-ttu-id="39ec7-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39ec7-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39ec7-144">响应</span><span class="sxs-lookup"><span data-stu-id="39ec7-144">Response</span></span>
<span data-ttu-id="39ec7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39ec7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





