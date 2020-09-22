---
title: 创建 securityBaselineCategoryStateSummary
description: 创建新的 securityBaselineCategoryStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b375538d5d5492e5f3c3942f44645ee12399b3af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088207"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="d52ea-103">创建 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="d52ea-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="d52ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d52ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d52ea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d52ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d52ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d52ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d52ea-107">创建新的 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d52ea-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d52ea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d52ea-108">Prerequisites</span></span>
<span data-ttu-id="d52ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d52ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d52ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d52ea-111">Permission type</span></span>|<span data-ttu-id="d52ea-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d52ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d52ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d52ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d52ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d52ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d52ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d52ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d52ea-116">Not supported.</span></span>|
|<span data-ttu-id="d52ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d52ea-117">Application</span></span>|<span data-ttu-id="d52ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d52ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d52ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d52ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d52ea-120">Request headers</span></span>
|<span data-ttu-id="d52ea-121">标头</span><span class="sxs-lookup"><span data-stu-id="d52ea-121">Header</span></span>|<span data-ttu-id="d52ea-122">值</span><span class="sxs-lookup"><span data-stu-id="d52ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d52ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d52ea-123">Authorization</span></span>|<span data-ttu-id="d52ea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d52ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d52ea-125">接受</span><span class="sxs-lookup"><span data-stu-id="d52ea-125">Accept</span></span>|<span data-ttu-id="d52ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d52ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d52ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d52ea-127">Request body</span></span>
<span data-ttu-id="d52ea-128">在请求正文中，提供 securityBaselineCategoryStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d52ea-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="d52ea-129">下表显示创建 securityBaselineCategoryStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d52ea-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="d52ea-130">属性</span><span class="sxs-lookup"><span data-stu-id="d52ea-130">Property</span></span>|<span data-ttu-id="d52ea-131">类型</span><span class="sxs-lookup"><span data-stu-id="d52ea-131">Type</span></span>|<span data-ttu-id="d52ea-132">说明</span><span class="sxs-lookup"><span data-stu-id="d52ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d52ea-133">id</span><span class="sxs-lookup"><span data-stu-id="d52ea-133">id</span></span>|<span data-ttu-id="d52ea-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d52ea-134">String</span></span>|<span data-ttu-id="d52ea-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d52ea-135">Unique identifier of the entity.</span></span> <span data-ttu-id="d52ea-136">继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d52ea-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-137">secureCount</span></span>|<span data-ttu-id="d52ea-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-138">Int32</span></span>|<span data-ttu-id="d52ea-139">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-140">notSecureCount</span></span>|<span data-ttu-id="d52ea-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-141">Int32</span></span>|<span data-ttu-id="d52ea-142">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-143">unknownCount</span></span>|<span data-ttu-id="d52ea-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-144">Int32</span></span>|<span data-ttu-id="d52ea-145">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-146">errorCount</span></span>|<span data-ttu-id="d52ea-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-147">Int32</span></span>|<span data-ttu-id="d52ea-148">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-149">conflictCount</span></span>|<span data-ttu-id="d52ea-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-150">Int32</span></span>|<span data-ttu-id="d52ea-151">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d52ea-152">notApplicableCount</span></span>|<span data-ttu-id="d52ea-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d52ea-153">Int32</span></span>|<span data-ttu-id="d52ea-154">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="d52ea-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="d52ea-155">displayName</span><span class="sxs-lookup"><span data-stu-id="d52ea-155">displayName</span></span>|<span data-ttu-id="d52ea-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d52ea-156">String</span></span>|<span data-ttu-id="d52ea-157">类别名称</span><span class="sxs-lookup"><span data-stu-id="d52ea-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="d52ea-158">响应</span><span class="sxs-lookup"><span data-stu-id="d52ea-158">Response</span></span>
<span data-ttu-id="d52ea-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d52ea-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d52ea-160">示例</span><span class="sxs-lookup"><span data-stu-id="d52ea-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="d52ea-161">请求</span><span class="sxs-lookup"><span data-stu-id="d52ea-161">Request</span></span>
<span data-ttu-id="d52ea-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d52ea-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d52ea-163">响应</span><span class="sxs-lookup"><span data-stu-id="d52ea-163">Response</span></span>
<span data-ttu-id="d52ea-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d52ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






