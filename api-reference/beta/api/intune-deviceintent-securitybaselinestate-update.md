---
title: 更新 securityBaselineState
description: 更新 securityBaselineState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad0bca78fdf54054b9319853123ab0e79321ed59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466173"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="28d73-103">更新 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="28d73-103">Update securityBaselineState</span></span>

> <span data-ttu-id="28d73-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28d73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28d73-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28d73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28d73-106">更新[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28d73-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28d73-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="28d73-107">Prerequisites</span></span>
<span data-ttu-id="28d73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28d73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d73-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28d73-110">Permission type</span></span>|<span data-ttu-id="28d73-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="28d73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28d73-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28d73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28d73-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d73-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28d73-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28d73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28d73-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28d73-115">Not supported.</span></span>|
|<span data-ttu-id="28d73-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28d73-116">Application</span></span>|<span data-ttu-id="28d73-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="28d73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28d73-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28d73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="28d73-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28d73-119">Request headers</span></span>
|<span data-ttu-id="28d73-120">标头</span><span class="sxs-lookup"><span data-stu-id="28d73-120">Header</span></span>|<span data-ttu-id="28d73-121">值</span><span class="sxs-lookup"><span data-stu-id="28d73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28d73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28d73-122">Authorization</span></span>|<span data-ttu-id="28d73-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="28d73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28d73-124">接受</span><span class="sxs-lookup"><span data-stu-id="28d73-124">Accept</span></span>|<span data-ttu-id="28d73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28d73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d73-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28d73-126">Request body</span></span>
<span data-ttu-id="28d73-127">在请求正文中, 提供[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28d73-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="28d73-128">下表显示创建[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28d73-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="28d73-129">属性</span><span class="sxs-lookup"><span data-stu-id="28d73-129">Property</span></span>|<span data-ttu-id="28d73-130">类型</span><span class="sxs-lookup"><span data-stu-id="28d73-130">Type</span></span>|<span data-ttu-id="28d73-131">说明</span><span class="sxs-lookup"><span data-stu-id="28d73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28d73-132">id</span><span class="sxs-lookup"><span data-stu-id="28d73-132">id</span></span>|<span data-ttu-id="28d73-133">String</span><span class="sxs-lookup"><span data-stu-id="28d73-133">String</span></span>|<span data-ttu-id="28d73-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="28d73-134">Key of the entity.</span></span>|
|<span data-ttu-id="28d73-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="28d73-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="28d73-136">字符串</span><span class="sxs-lookup"><span data-stu-id="28d73-136">String</span></span>|<span data-ttu-id="28d73-137">安全基准模板 id</span><span class="sxs-lookup"><span data-stu-id="28d73-137">The security baseline template id</span></span>|
|<span data-ttu-id="28d73-138">displayName</span><span class="sxs-lookup"><span data-stu-id="28d73-138">displayName</span></span>|<span data-ttu-id="28d73-139">String</span><span class="sxs-lookup"><span data-stu-id="28d73-139">String</span></span>|<span data-ttu-id="28d73-140">安全基准的显示名称</span><span class="sxs-lookup"><span data-stu-id="28d73-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="28d73-141">响应</span><span class="sxs-lookup"><span data-stu-id="28d73-141">Response</span></span>
<span data-ttu-id="28d73-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28d73-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d73-143">示例</span><span class="sxs-lookup"><span data-stu-id="28d73-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="28d73-144">请求</span><span class="sxs-lookup"><span data-stu-id="28d73-144">Request</span></span>
<span data-ttu-id="28d73-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="28d73-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="28d73-146">响应</span><span class="sxs-lookup"><span data-stu-id="28d73-146">Response</span></span>
<span data-ttu-id="28d73-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28d73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



