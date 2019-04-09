---
title: 更新 securityBaselineState
description: 更新 securityBaselineState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33f4a65937f8139aa7ebee483cad6e66f989caa0
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522844"
---
# <a name="update-securitybaselinestate"></a><span data-ttu-id="6a812-103">更新 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="6a812-103">Update securityBaselineState</span></span>

> <span data-ttu-id="6a812-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a812-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a812-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a812-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a812-106">更新[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a812-106">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a812-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a812-107">Prerequisites</span></span>
<span data-ttu-id="6a812-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6a812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a812-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a812-110">Permission type</span></span>|<span data-ttu-id="6a812-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a812-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a812-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a812-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a812-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a812-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a812-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a812-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a812-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a812-115">Not supported.</span></span>|
|<span data-ttu-id="6a812-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a812-116">Application</span></span>|<span data-ttu-id="6a812-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a812-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a812-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a812-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}
```

## <a name="request-headers"></a><span data-ttu-id="6a812-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a812-119">Request headers</span></span>
|<span data-ttu-id="6a812-120">标头</span><span class="sxs-lookup"><span data-stu-id="6a812-120">Header</span></span>|<span data-ttu-id="6a812-121">值</span><span class="sxs-lookup"><span data-stu-id="6a812-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a812-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a812-122">Authorization</span></span>|<span data-ttu-id="6a812-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a812-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a812-124">接受</span><span class="sxs-lookup"><span data-stu-id="6a812-124">Accept</span></span>|<span data-ttu-id="6a812-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a812-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a812-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a812-126">Request body</span></span>
<span data-ttu-id="6a812-127">在请求正文中, 提供[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a812-127">In the request body, supply a JSON representation for the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

<span data-ttu-id="6a812-128">下表显示创建[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a812-128">The following table shows the properties that are required when you create the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>

|<span data-ttu-id="6a812-129">属性</span><span class="sxs-lookup"><span data-stu-id="6a812-129">Property</span></span>|<span data-ttu-id="6a812-130">类型</span><span class="sxs-lookup"><span data-stu-id="6a812-130">Type</span></span>|<span data-ttu-id="6a812-131">说明</span><span class="sxs-lookup"><span data-stu-id="6a812-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a812-132">id</span><span class="sxs-lookup"><span data-stu-id="6a812-132">id</span></span>|<span data-ttu-id="6a812-133">String</span><span class="sxs-lookup"><span data-stu-id="6a812-133">String</span></span>|<span data-ttu-id="6a812-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6a812-134">Key of the entity.</span></span>|
|<span data-ttu-id="6a812-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="6a812-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="6a812-136">String</span><span class="sxs-lookup"><span data-stu-id="6a812-136">String</span></span>|<span data-ttu-id="6a812-137">安全基准模板 id</span><span class="sxs-lookup"><span data-stu-id="6a812-137">The security baseline template id</span></span>|
|<span data-ttu-id="6a812-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6a812-138">displayName</span></span>|<span data-ttu-id="6a812-139">String</span><span class="sxs-lookup"><span data-stu-id="6a812-139">String</span></span>|<span data-ttu-id="6a812-140">安全基准的显示名称</span><span class="sxs-lookup"><span data-stu-id="6a812-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="6a812-141">响应</span><span class="sxs-lookup"><span data-stu-id="6a812-141">Response</span></span>
<span data-ttu-id="6a812-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a812-142">If successful, this method returns a `200 OK` response code and an updated [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a812-143">示例</span><span class="sxs-lookup"><span data-stu-id="6a812-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a812-144">请求</span><span class="sxs-lookup"><span data-stu-id="6a812-144">Request</span></span>
<span data-ttu-id="6a812-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a812-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a812-146">响应</span><span class="sxs-lookup"><span data-stu-id="6a812-146">Response</span></span>
<span data-ttu-id="6a812-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a812-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



