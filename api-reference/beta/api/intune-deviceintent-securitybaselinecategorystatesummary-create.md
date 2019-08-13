---
title: 创建 securityBaselineCategoryStateSummary
description: 创建新的 securityBaselineCategoryStateSummary 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42c21f7584e0f747d2f18203cb10ac6577ee984d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343060"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="c1b9e-103">创建 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="c1b9e-103">Create securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="c1b9e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1b9e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1b9e-106">创建新的[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-106">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1b9e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1b9e-107">Prerequisites</span></span>
<span data-ttu-id="c1b9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1b9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1b9e-110">Permission type</span></span>|<span data-ttu-id="c1b9e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1b9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1b9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1b9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1b9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1b9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1b9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-115">Not supported.</span></span>|
|<span data-ttu-id="c1b9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1b9e-116">Application</span></span>|<span data-ttu-id="c1b9e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1b9e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1b9e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1b9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c1b9e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1b9e-119">Request headers</span></span>
|<span data-ttu-id="c1b9e-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1b9e-120">Header</span></span>|<span data-ttu-id="c1b9e-121">值</span><span class="sxs-lookup"><span data-stu-id="c1b9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1b9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1b9e-122">Authorization</span></span>|<span data-ttu-id="c1b9e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1b9e-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1b9e-124">Accept</span></span>|<span data-ttu-id="c1b9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1b9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1b9e-126">Request body</span></span>
<span data-ttu-id="c1b9e-127">在请求正文中, 提供 securityBaselineCategoryStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-127">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="c1b9e-128">下表显示创建 securityBaselineCategoryStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-128">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="c1b9e-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1b9e-129">Property</span></span>|<span data-ttu-id="c1b9e-130">类型</span><span class="sxs-lookup"><span data-stu-id="c1b9e-130">Type</span></span>|<span data-ttu-id="c1b9e-131">说明</span><span class="sxs-lookup"><span data-stu-id="c1b9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1b9e-132">id</span><span class="sxs-lookup"><span data-stu-id="c1b9e-132">id</span></span>|<span data-ttu-id="c1b9e-133">String</span><span class="sxs-lookup"><span data-stu-id="c1b9e-133">String</span></span>|<span data-ttu-id="c1b9e-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-134">Unique identifier of the entity.</span></span> <span data-ttu-id="c1b9e-135">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="c1b9e-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-136">secureCount</span></span>|<span data-ttu-id="c1b9e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-137">Int32</span></span>|<span data-ttu-id="c1b9e-138">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-139">notSecureCount</span></span>|<span data-ttu-id="c1b9e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-140">Int32</span></span>|<span data-ttu-id="c1b9e-141">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-142">unknownCount</span></span>|<span data-ttu-id="c1b9e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-143">Int32</span></span>|<span data-ttu-id="c1b9e-144">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-145">errorCount</span></span>|<span data-ttu-id="c1b9e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-146">Int32</span></span>|<span data-ttu-id="c1b9e-147">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-148">conflictCount</span></span>|<span data-ttu-id="c1b9e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-149">Int32</span></span>|<span data-ttu-id="c1b9e-150">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c1b9e-151">notApplicableCount</span></span>|<span data-ttu-id="c1b9e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b9e-152">Int32</span></span>|<span data-ttu-id="c1b9e-153">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c1b9e-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="c1b9e-154">displayName</span><span class="sxs-lookup"><span data-stu-id="c1b9e-154">displayName</span></span>|<span data-ttu-id="c1b9e-155">String</span><span class="sxs-lookup"><span data-stu-id="c1b9e-155">String</span></span>|<span data-ttu-id="c1b9e-156">类别名称</span><span class="sxs-lookup"><span data-stu-id="c1b9e-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="c1b9e-157">响应</span><span class="sxs-lookup"><span data-stu-id="c1b9e-157">Response</span></span>
<span data-ttu-id="c1b9e-158">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-158">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1b9e-159">示例</span><span class="sxs-lookup"><span data-stu-id="c1b9e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1b9e-160">请求</span><span class="sxs-lookup"><span data-stu-id="c1b9e-160">Request</span></span>
<span data-ttu-id="c1b9e-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c1b9e-162">响应</span><span class="sxs-lookup"><span data-stu-id="c1b9e-162">Response</span></span>
<span data-ttu-id="c1b9e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1b9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```






