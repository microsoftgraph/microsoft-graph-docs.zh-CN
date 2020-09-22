---
title: 更新 securityBaselineStateSummary
description: 更新 securityBaselineStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 479d79c0dc0129c1389d9410dbed32314685117b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068733"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="8f858-103">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="8f858-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="8f858-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f858-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f858-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f858-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f858-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f858-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f858-107">更新 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8f858-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f858-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f858-108">Prerequisites</span></span>
<span data-ttu-id="8f858-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f858-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f858-111">Permission type</span></span>|<span data-ttu-id="8f858-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f858-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f858-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f858-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f858-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f858-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f858-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f858-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f858-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f858-116">Not supported.</span></span>|
|<span data-ttu-id="8f858-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f858-117">Application</span></span>|<span data-ttu-id="8f858-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f858-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f858-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f858-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8f858-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f858-120">Request headers</span></span>
|<span data-ttu-id="8f858-121">标头</span><span class="sxs-lookup"><span data-stu-id="8f858-121">Header</span></span>|<span data-ttu-id="8f858-122">值</span><span class="sxs-lookup"><span data-stu-id="8f858-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f858-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f858-123">Authorization</span></span>|<span data-ttu-id="8f858-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f858-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f858-125">接受</span><span class="sxs-lookup"><span data-stu-id="8f858-125">Accept</span></span>|<span data-ttu-id="8f858-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f858-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f858-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f858-127">Request body</span></span>
<span data-ttu-id="8f858-128">在请求正文中，提供 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f858-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="8f858-129">下表显示创建 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f858-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="8f858-130">属性</span><span class="sxs-lookup"><span data-stu-id="8f858-130">Property</span></span>|<span data-ttu-id="8f858-131">类型</span><span class="sxs-lookup"><span data-stu-id="8f858-131">Type</span></span>|<span data-ttu-id="8f858-132">说明</span><span class="sxs-lookup"><span data-stu-id="8f858-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f858-133">id</span><span class="sxs-lookup"><span data-stu-id="8f858-133">id</span></span>|<span data-ttu-id="8f858-134">String</span><span class="sxs-lookup"><span data-stu-id="8f858-134">String</span></span>|<span data-ttu-id="8f858-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f858-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="8f858-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="8f858-136">secureCount</span></span>|<span data-ttu-id="8f858-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-137">Int32</span></span>|<span data-ttu-id="8f858-138">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-138">Number of secure devices</span></span>|
|<span data-ttu-id="8f858-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="8f858-139">notSecureCount</span></span>|<span data-ttu-id="8f858-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-140">Int32</span></span>|<span data-ttu-id="8f858-141">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-141">Number of not secure devices</span></span>|
|<span data-ttu-id="8f858-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="8f858-142">unknownCount</span></span>|<span data-ttu-id="8f858-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-143">Int32</span></span>|<span data-ttu-id="8f858-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-144">Number of unknown devices</span></span>|
|<span data-ttu-id="8f858-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="8f858-145">errorCount</span></span>|<span data-ttu-id="8f858-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-146">Int32</span></span>|<span data-ttu-id="8f858-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-147">Number of error devices</span></span>|
|<span data-ttu-id="8f858-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="8f858-148">conflictCount</span></span>|<span data-ttu-id="8f858-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-149">Int32</span></span>|<span data-ttu-id="8f858-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-150">Number of conflict devices</span></span>|
|<span data-ttu-id="8f858-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8f858-151">notApplicableCount</span></span>|<span data-ttu-id="8f858-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8f858-152">Int32</span></span>|<span data-ttu-id="8f858-153">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="8f858-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="8f858-154">响应</span><span class="sxs-lookup"><span data-stu-id="8f858-154">Response</span></span>
<span data-ttu-id="8f858-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f858-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f858-156">示例</span><span class="sxs-lookup"><span data-stu-id="8f858-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f858-157">请求</span><span class="sxs-lookup"><span data-stu-id="8f858-157">Request</span></span>
<span data-ttu-id="8f858-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f858-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="8f858-159">响应</span><span class="sxs-lookup"><span data-stu-id="8f858-159">Response</span></span>
<span data-ttu-id="8f858-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f858-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```






