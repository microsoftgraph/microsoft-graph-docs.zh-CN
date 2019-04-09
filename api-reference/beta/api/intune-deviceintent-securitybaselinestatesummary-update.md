---
title: 更新 securityBaselineStateSummary
description: 更新 securityBaselineStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cfd2f6eafd638822b5bd66887ab36d3bf95a88d
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523621"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="16446-103">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="16446-103">Update securityBaselineStateSummary</span></span>

> <span data-ttu-id="16446-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16446-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16446-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16446-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16446-106">更新[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16446-106">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16446-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="16446-107">Prerequisites</span></span>
<span data-ttu-id="16446-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16446-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16446-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16446-110">Permission type</span></span>|<span data-ttu-id="16446-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16446-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16446-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16446-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16446-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16446-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16446-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16446-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16446-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16446-115">Not supported.</span></span>|
|<span data-ttu-id="16446-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16446-116">Application</span></span>|<span data-ttu-id="16446-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="16446-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16446-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16446-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="16446-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="16446-119">Request headers</span></span>
|<span data-ttu-id="16446-120">标头</span><span class="sxs-lookup"><span data-stu-id="16446-120">Header</span></span>|<span data-ttu-id="16446-121">值</span><span class="sxs-lookup"><span data-stu-id="16446-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16446-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16446-122">Authorization</span></span>|<span data-ttu-id="16446-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16446-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16446-124">接受</span><span class="sxs-lookup"><span data-stu-id="16446-124">Accept</span></span>|<span data-ttu-id="16446-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16446-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16446-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16446-126">Request body</span></span>
<span data-ttu-id="16446-127">在请求正文中, 提供[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16446-127">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="16446-128">下表显示创建[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16446-128">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="16446-129">属性</span><span class="sxs-lookup"><span data-stu-id="16446-129">Property</span></span>|<span data-ttu-id="16446-130">类型</span><span class="sxs-lookup"><span data-stu-id="16446-130">Type</span></span>|<span data-ttu-id="16446-131">说明</span><span class="sxs-lookup"><span data-stu-id="16446-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16446-132">id</span><span class="sxs-lookup"><span data-stu-id="16446-132">id</span></span>|<span data-ttu-id="16446-133">String</span><span class="sxs-lookup"><span data-stu-id="16446-133">String</span></span>|<span data-ttu-id="16446-134">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="16446-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="16446-135">secureCount</span><span class="sxs-lookup"><span data-stu-id="16446-135">secureCount</span></span>|<span data-ttu-id="16446-136">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-136">Int32</span></span>|<span data-ttu-id="16446-137">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-137">Number of secure devices</span></span>|
|<span data-ttu-id="16446-138">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="16446-138">notSecureCount</span></span>|<span data-ttu-id="16446-139">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-139">Int32</span></span>|<span data-ttu-id="16446-140">不安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-140">Number of not secure devices</span></span>|
|<span data-ttu-id="16446-141">unknownCount</span><span class="sxs-lookup"><span data-stu-id="16446-141">unknownCount</span></span>|<span data-ttu-id="16446-142">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-142">Int32</span></span>|<span data-ttu-id="16446-143">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-143">Number of unknown devices</span></span>|
|<span data-ttu-id="16446-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="16446-144">errorCount</span></span>|<span data-ttu-id="16446-145">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-145">Int32</span></span>|<span data-ttu-id="16446-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-146">Number of error devices</span></span>|
|<span data-ttu-id="16446-147">conflictCount</span><span class="sxs-lookup"><span data-stu-id="16446-147">conflictCount</span></span>|<span data-ttu-id="16446-148">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-148">Int32</span></span>|<span data-ttu-id="16446-149">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-149">Number of conflict devices</span></span>|
|<span data-ttu-id="16446-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="16446-150">notApplicableCount</span></span>|<span data-ttu-id="16446-151">Int32</span><span class="sxs-lookup"><span data-stu-id="16446-151">Int32</span></span>|<span data-ttu-id="16446-152">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="16446-152">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="16446-153">响应</span><span class="sxs-lookup"><span data-stu-id="16446-153">Response</span></span>
<span data-ttu-id="16446-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16446-154">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16446-155">示例</span><span class="sxs-lookup"><span data-stu-id="16446-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="16446-156">请求</span><span class="sxs-lookup"><span data-stu-id="16446-156">Request</span></span>
<span data-ttu-id="16446-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16446-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16446-158">响应</span><span class="sxs-lookup"><span data-stu-id="16446-158">Response</span></span>
<span data-ttu-id="16446-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16446-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







