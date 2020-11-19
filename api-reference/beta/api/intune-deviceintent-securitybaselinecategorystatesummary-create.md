---
title: 创建 securityBaselineCategoryStateSummary
description: 创建新的 securityBaselineCategoryStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83048a9fa97660cc02a6d9ee8bd58ca029da01e7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311096"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="f64af-103">创建 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="f64af-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="f64af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f64af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f64af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f64af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f64af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f64af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f64af-107">创建新的 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f64af-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f64af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f64af-108">Prerequisites</span></span>
<span data-ttu-id="f64af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f64af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f64af-111">Permission type</span></span>|<span data-ttu-id="f64af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f64af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f64af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f64af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f64af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f64af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f64af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f64af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f64af-116">Not supported.</span></span>|
|<span data-ttu-id="f64af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f64af-117">Application</span></span>|<span data-ttu-id="f64af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f64af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f64af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f64af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f64af-120">Request headers</span></span>
|<span data-ttu-id="f64af-121">标头</span><span class="sxs-lookup"><span data-stu-id="f64af-121">Header</span></span>|<span data-ttu-id="f64af-122">值</span><span class="sxs-lookup"><span data-stu-id="f64af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f64af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f64af-123">Authorization</span></span>|<span data-ttu-id="f64af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f64af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f64af-125">接受</span><span class="sxs-lookup"><span data-stu-id="f64af-125">Accept</span></span>|<span data-ttu-id="f64af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f64af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f64af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f64af-127">Request body</span></span>
<span data-ttu-id="f64af-128">在请求正文中，提供 securityBaselineCategoryStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f64af-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="f64af-129">下表显示创建 securityBaselineCategoryStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f64af-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="f64af-130">属性</span><span class="sxs-lookup"><span data-stu-id="f64af-130">Property</span></span>|<span data-ttu-id="f64af-131">类型</span><span class="sxs-lookup"><span data-stu-id="f64af-131">Type</span></span>|<span data-ttu-id="f64af-132">说明</span><span class="sxs-lookup"><span data-stu-id="f64af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f64af-133">id</span><span class="sxs-lookup"><span data-stu-id="f64af-133">id</span></span>|<span data-ttu-id="f64af-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f64af-134">String</span></span>|<span data-ttu-id="f64af-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f64af-135">Unique identifier of the entity.</span></span> <span data-ttu-id="f64af-136">继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f64af-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="f64af-137">secureCount</span></span>|<span data-ttu-id="f64af-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-138">Int32</span></span>|<span data-ttu-id="f64af-139">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="f64af-140">notSecureCount</span></span>|<span data-ttu-id="f64af-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-141">Int32</span></span>|<span data-ttu-id="f64af-142">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f64af-143">unknownCount</span></span>|<span data-ttu-id="f64af-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-144">Int32</span></span>|<span data-ttu-id="f64af-145">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="f64af-146">errorCount</span></span>|<span data-ttu-id="f64af-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-147">Int32</span></span>|<span data-ttu-id="f64af-148">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="f64af-149">conflictCount</span></span>|<span data-ttu-id="f64af-150">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-150">Int32</span></span>|<span data-ttu-id="f64af-151">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f64af-152">notApplicableCount</span></span>|<span data-ttu-id="f64af-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f64af-153">Int32</span></span>|<span data-ttu-id="f64af-154">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f64af-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="f64af-155">displayName</span><span class="sxs-lookup"><span data-stu-id="f64af-155">displayName</span></span>|<span data-ttu-id="f64af-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f64af-156">String</span></span>|<span data-ttu-id="f64af-157">类别名称</span><span class="sxs-lookup"><span data-stu-id="f64af-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="f64af-158">响应</span><span class="sxs-lookup"><span data-stu-id="f64af-158">Response</span></span>
<span data-ttu-id="f64af-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f64af-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64af-160">示例</span><span class="sxs-lookup"><span data-stu-id="f64af-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="f64af-161">请求</span><span class="sxs-lookup"><span data-stu-id="f64af-161">Request</span></span>
<span data-ttu-id="f64af-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f64af-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f64af-163">响应</span><span class="sxs-lookup"><span data-stu-id="f64af-163">Response</span></span>
<span data-ttu-id="f64af-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f64af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




