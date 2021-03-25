---
title: 更新 securityBaselineStateSummary
description: 更新 securityBaselineStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de1db7428f19e07f6bf7d349b00d995d93d0a660
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154516"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="aaf28-103">更新 securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="aaf28-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="aaf28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaf28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaf28-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aaf28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf28-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aaf28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf28-107">更新 [securityBaselineStateSummary 对象](../resources/intune-deviceintent-securitybaselinestatesummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="aaf28-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaf28-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aaf28-108">Prerequisites</span></span>
<span data-ttu-id="aaf28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaf28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf28-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaf28-111">Permission type</span></span>|<span data-ttu-id="aaf28-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aaf28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaf28-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaf28-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf28-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaf28-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaf28-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aaf28-116">Not supported.</span></span>|
|<span data-ttu-id="aaf28-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaf28-117">Application</span></span>|<span data-ttu-id="aaf28-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf28-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaf28-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaf28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="aaf28-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aaf28-120">Request headers</span></span>
|<span data-ttu-id="aaf28-121">标头</span><span class="sxs-lookup"><span data-stu-id="aaf28-121">Header</span></span>|<span data-ttu-id="aaf28-122">值</span><span class="sxs-lookup"><span data-stu-id="aaf28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaf28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf28-123">Authorization</span></span>|<span data-ttu-id="aaf28-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aaf28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaf28-125">接受</span><span class="sxs-lookup"><span data-stu-id="aaf28-125">Accept</span></span>|<span data-ttu-id="aaf28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaf28-127">Request body</span></span>
<span data-ttu-id="aaf28-128">在请求正文中，提供 [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaf28-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="aaf28-129">下表显示创建 [securityBaselineStateSummary 时所需的属性](../resources/intune-deviceintent-securitybaselinestatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="aaf28-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="aaf28-130">属性</span><span class="sxs-lookup"><span data-stu-id="aaf28-130">Property</span></span>|<span data-ttu-id="aaf28-131">类型</span><span class="sxs-lookup"><span data-stu-id="aaf28-131">Type</span></span>|<span data-ttu-id="aaf28-132">说明</span><span class="sxs-lookup"><span data-stu-id="aaf28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf28-133">id</span><span class="sxs-lookup"><span data-stu-id="aaf28-133">id</span></span>|<span data-ttu-id="aaf28-134">String</span><span class="sxs-lookup"><span data-stu-id="aaf28-134">String</span></span>|<span data-ttu-id="aaf28-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aaf28-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="aaf28-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-136">secureCount</span></span>|<span data-ttu-id="aaf28-137">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-137">Int32</span></span>|<span data-ttu-id="aaf28-138">安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-138">Number of secure devices</span></span>|
|<span data-ttu-id="aaf28-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-139">notSecureCount</span></span>|<span data-ttu-id="aaf28-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-140">Int32</span></span>|<span data-ttu-id="aaf28-141">非安全设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-141">Number of not secure devices</span></span>|
|<span data-ttu-id="aaf28-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-142">unknownCount</span></span>|<span data-ttu-id="aaf28-143">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-143">Int32</span></span>|<span data-ttu-id="aaf28-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-144">Number of unknown devices</span></span>|
|<span data-ttu-id="aaf28-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-145">errorCount</span></span>|<span data-ttu-id="aaf28-146">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-146">Int32</span></span>|<span data-ttu-id="aaf28-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-147">Number of error devices</span></span>|
|<span data-ttu-id="aaf28-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-148">conflictCount</span></span>|<span data-ttu-id="aaf28-149">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-149">Int32</span></span>|<span data-ttu-id="aaf28-150">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-150">Number of conflict devices</span></span>|
|<span data-ttu-id="aaf28-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="aaf28-151">notApplicableCount</span></span>|<span data-ttu-id="aaf28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf28-152">Int32</span></span>|<span data-ttu-id="aaf28-153">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="aaf28-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="aaf28-154">响应</span><span class="sxs-lookup"><span data-stu-id="aaf28-154">Response</span></span>
<span data-ttu-id="aaf28-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaf28-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf28-156">示例</span><span class="sxs-lookup"><span data-stu-id="aaf28-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaf28-157">请求</span><span class="sxs-lookup"><span data-stu-id="aaf28-157">Request</span></span>
<span data-ttu-id="aaf28-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aaf28-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aaf28-159">响应</span><span class="sxs-lookup"><span data-stu-id="aaf28-159">Response</span></span>
<span data-ttu-id="aaf28-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aaf28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




