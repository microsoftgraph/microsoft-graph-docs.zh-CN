---
title: 创建 securityBaselineState
description: 创建新的 securityBaselineState 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f481bc5a3fa5e58017a671fe2fed43baa4c30af1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522522"
---
# <a name="create-securitybaselinestate"></a><span data-ttu-id="4a7dc-103">创建 securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="4a7dc-103">Create securityBaselineState</span></span>

> <span data-ttu-id="4a7dc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a7dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a7dc-106">创建新的[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-106">Create a new [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a7dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a7dc-107">Prerequisites</span></span>
<span data-ttu-id="4a7dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a7dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a7dc-110">Permission type</span></span>|<span data-ttu-id="4a7dc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a7dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a7dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a7dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a7dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a7dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a7dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a7dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-115">Not supported.</span></span>|
|<span data-ttu-id="4a7dc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a7dc-116">Application</span></span>|<span data-ttu-id="4a7dc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a7dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a7dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="4a7dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a7dc-119">Request headers</span></span>
|<span data-ttu-id="4a7dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="4a7dc-120">Header</span></span>|<span data-ttu-id="4a7dc-121">值</span><span class="sxs-lookup"><span data-stu-id="4a7dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a7dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a7dc-122">Authorization</span></span>|<span data-ttu-id="4a7dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a7dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="4a7dc-124">Accept</span></span>|<span data-ttu-id="4a7dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a7dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a7dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a7dc-126">Request body</span></span>
<span data-ttu-id="4a7dc-127">在请求正文中, 提供 securityBaselineState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-127">In the request body, supply a JSON representation for the securityBaselineState object.</span></span>

<span data-ttu-id="4a7dc-128">下表显示创建 securityBaselineState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-128">The following table shows the properties that are required when you create the securityBaselineState.</span></span>

|<span data-ttu-id="4a7dc-129">属性</span><span class="sxs-lookup"><span data-stu-id="4a7dc-129">Property</span></span>|<span data-ttu-id="4a7dc-130">类型</span><span class="sxs-lookup"><span data-stu-id="4a7dc-130">Type</span></span>|<span data-ttu-id="4a7dc-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a7dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a7dc-132">id</span><span class="sxs-lookup"><span data-stu-id="4a7dc-132">id</span></span>|<span data-ttu-id="4a7dc-133">String</span><span class="sxs-lookup"><span data-stu-id="4a7dc-133">String</span></span>|<span data-ttu-id="4a7dc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-134">Key of the entity.</span></span>|
|<span data-ttu-id="4a7dc-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="4a7dc-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="4a7dc-136">String</span><span class="sxs-lookup"><span data-stu-id="4a7dc-136">String</span></span>|<span data-ttu-id="4a7dc-137">安全基准模板 id</span><span class="sxs-lookup"><span data-stu-id="4a7dc-137">The security baseline template id</span></span>|
|<span data-ttu-id="4a7dc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4a7dc-138">displayName</span></span>|<span data-ttu-id="4a7dc-139">String</span><span class="sxs-lookup"><span data-stu-id="4a7dc-139">String</span></span>|<span data-ttu-id="4a7dc-140">安全基准的显示名称</span><span class="sxs-lookup"><span data-stu-id="4a7dc-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="4a7dc-141">响应</span><span class="sxs-lookup"><span data-stu-id="4a7dc-141">Response</span></span>
<span data-ttu-id="4a7dc-142">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-142">If successful, this method returns a `201 Created` response code and a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a7dc-143">示例</span><span class="sxs-lookup"><span data-stu-id="4a7dc-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a7dc-144">请求</span><span class="sxs-lookup"><span data-stu-id="4a7dc-144">Request</span></span>
<span data-ttu-id="4a7dc-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4a7dc-146">响应</span><span class="sxs-lookup"><span data-stu-id="4a7dc-146">Response</span></span>
<span data-ttu-id="4a7dc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a7dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



