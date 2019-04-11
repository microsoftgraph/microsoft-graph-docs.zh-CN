---
title: 更新 securityBaselineState
description: 更新 securityBaselineState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad0bca78fdf54054b9319853123ab0e79321ed59
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791927"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="ebdb2-103">更新 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="ebdb2-103">Update securityBaselineState</span></span>

> <span data-ttu-id="ebdb2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebdb2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebdb2-106">更新[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebdb2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ebdb2-107">Prerequisites</span></span>
<span data-ttu-id="ebdb2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebdb2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebdb2-110">Permission type</span></span>|<span data-ttu-id="ebdb2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ebdb2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebdb2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebdb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebdb2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdb2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebdb2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebdb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebdb2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-115">Not supported.</span></span>|
|<span data-ttu-id="ebdb2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebdb2-116">Application</span></span>|<span data-ttu-id="ebdb2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebdb2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebdb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="ebdb2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebdb2-119">Request headers</span></span>
|<span data-ttu-id="ebdb2-120">标头</span><span class="sxs-lookup"><span data-stu-id="ebdb2-120">Header</span></span>|<span data-ttu-id="ebdb2-121">值</span><span class="sxs-lookup"><span data-stu-id="ebdb2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebdb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebdb2-122">Authorization</span></span>|<span data-ttu-id="ebdb2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebdb2-124">接受</span><span class="sxs-lookup"><span data-stu-id="ebdb2-124">Accept</span></span>|<span data-ttu-id="ebdb2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebdb2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebdb2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebdb2-126">Request body</span></span>
<span data-ttu-id="ebdb2-127">在请求正文中, 提供[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="ebdb2-128">下表显示创建[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="ebdb2-129">属性</span><span class="sxs-lookup"><span data-stu-id="ebdb2-129">Property</span></span>|<span data-ttu-id="ebdb2-130">类型</span><span class="sxs-lookup"><span data-stu-id="ebdb2-130">Type</span></span>|<span data-ttu-id="ebdb2-131">说明</span><span class="sxs-lookup"><span data-stu-id="ebdb2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebdb2-132">id</span><span class="sxs-lookup"><span data-stu-id="ebdb2-132">id</span></span>|<span data-ttu-id="ebdb2-133">String</span><span class="sxs-lookup"><span data-stu-id="ebdb2-133">String</span></span>|<span data-ttu-id="ebdb2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-134">Key of the entity.</span></span>|
|<span data-ttu-id="ebdb2-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="ebdb2-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="ebdb2-136">String</span><span class="sxs-lookup"><span data-stu-id="ebdb2-136">String</span></span>|<span data-ttu-id="ebdb2-137">安全基准模板 id</span><span class="sxs-lookup"><span data-stu-id="ebdb2-137">The security baseline template id</span></span>|
|<span data-ttu-id="ebdb2-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ebdb2-138">displayName</span></span>|<span data-ttu-id="ebdb2-139">String</span><span class="sxs-lookup"><span data-stu-id="ebdb2-139">String</span></span>|<span data-ttu-id="ebdb2-140">安全基准的显示名称</span><span class="sxs-lookup"><span data-stu-id="ebdb2-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="ebdb2-141">响应</span><span class="sxs-lookup"><span data-stu-id="ebdb2-141">Response</span></span>
<span data-ttu-id="ebdb2-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdb2-143">示例</span><span class="sxs-lookup"><span data-stu-id="ebdb2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebdb2-144">请求</span><span class="sxs-lookup"><span data-stu-id="ebdb2-144">Request</span></span>
<span data-ttu-id="ebdb2-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebdb2-146">响应</span><span class="sxs-lookup"><span data-stu-id="ebdb2-146">Response</span></span>
<span data-ttu-id="ebdb2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebdb2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



