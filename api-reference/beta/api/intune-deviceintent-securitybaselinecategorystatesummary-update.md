---
title: 更新 securityBaselineCategoryStateSummary
description: 更新 securityBaselineCategoryStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09007fd08a9eddd5dbf74304e522fab00aa5ba2c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311033"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="2e293-103">更新 securityBaselineCategoryStateSummary</span><span class="sxs-lookup"><span data-stu-id="2e293-103">Update securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="2e293-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e293-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e293-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e293-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e293-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e293-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e293-107">更新 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e293-107">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e293-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e293-108">Prerequisites</span></span>
<span data-ttu-id="2e293-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e293-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e293-111">Permission type</span></span>|<span data-ttu-id="2e293-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e293-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e293-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e293-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e293-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e293-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e293-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e293-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e293-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e293-116">Not supported.</span></span>|
|<span data-ttu-id="2e293-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e293-117">Application</span></span>|<span data-ttu-id="2e293-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e293-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e293-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e293-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="2e293-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e293-120">Request headers</span></span>
|<span data-ttu-id="2e293-121">标头</span><span class="sxs-lookup"><span data-stu-id="2e293-121">Header</span></span>|<span data-ttu-id="2e293-122">值</span><span class="sxs-lookup"><span data-stu-id="2e293-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e293-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e293-123">Authorization</span></span>|<span data-ttu-id="2e293-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e293-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e293-125">接受</span><span class="sxs-lookup"><span data-stu-id="2e293-125">Accept</span></span>|<span data-ttu-id="2e293-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e293-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e293-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e293-127">Request body</span></span>
<span data-ttu-id="2e293-128">在请求正文中，提供 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e293-128">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="2e293-129">下表显示创建 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e293-129">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="2e293-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e293-130">Property</span></span>|<span data-ttu-id="2e293-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e293-131">Type</span></span>|<span data-ttu-id="2e293-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e293-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e293-133">id</span><span class="sxs-lookup"><span data-stu-id="2e293-133">id</span></span>|<span data-ttu-id="2e293-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2e293-134">String</span></span>|<span data-ttu-id="2e293-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2e293-135">Unique identifier of the entity.</span></span> <span data-ttu-id="2e293-136">继承自 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="2e293-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-137">secureCount</span><span class="sxs-lookup"><span data-stu-id="2e293-137">secureCount</span></span>|<span data-ttu-id="2e293-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-138">Int32</span></span>|<span data-ttu-id="2e293-139">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-140">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="2e293-140">notSecureCount</span></span>|<span data-ttu-id="2e293-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-141">Int32</span></span>|<span data-ttu-id="2e293-142">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="2e293-143">unknownCount</span></span>|<span data-ttu-id="2e293-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-144">Int32</span></span>|<span data-ttu-id="2e293-145">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="2e293-146">errorCount</span></span>|<span data-ttu-id="2e293-147">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-147">Int32</span></span>|<span data-ttu-id="2e293-148">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="2e293-149">conflictCount</span></span>|<span data-ttu-id="2e293-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-150">Int32</span></span>|<span data-ttu-id="2e293-151">继承自[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)的冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2e293-152">notApplicableCount</span></span>|<span data-ttu-id="2e293-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2e293-153">Int32</span></span>|<span data-ttu-id="2e293-154">从[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)继承的不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="2e293-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="2e293-155">displayName</span><span class="sxs-lookup"><span data-stu-id="2e293-155">displayName</span></span>|<span data-ttu-id="2e293-156">字符串</span><span class="sxs-lookup"><span data-stu-id="2e293-156">String</span></span>|<span data-ttu-id="2e293-157">类别名称</span><span class="sxs-lookup"><span data-stu-id="2e293-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="2e293-158">响应</span><span class="sxs-lookup"><span data-stu-id="2e293-158">Response</span></span>
<span data-ttu-id="2e293-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e293-159">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e293-160">示例</span><span class="sxs-lookup"><span data-stu-id="2e293-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e293-161">请求</span><span class="sxs-lookup"><span data-stu-id="2e293-161">Request</span></span>
<span data-ttu-id="2e293-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e293-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="2e293-163">响应</span><span class="sxs-lookup"><span data-stu-id="2e293-163">Response</span></span>
<span data-ttu-id="2e293-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e293-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




