---
title: 创建 groupPolicyConfiguration
description: 创建新的 groupPolicyConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 307c12d5b91759618c01f9fa219f50779394a0bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174711"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="2dca0-103">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dca0-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="2dca0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2dca0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dca0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dca0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dca0-106">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2dca0-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dca0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2dca0-107">Prerequisites</span></span>
<span data-ttu-id="2dca0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2dca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2dca0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2dca0-110">Permission type</span></span>|<span data-ttu-id="2dca0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2dca0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dca0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2dca0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2dca0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dca0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2dca0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2dca0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dca0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2dca0-115">Not supported.</span></span>|
|<span data-ttu-id="2dca0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2dca0-116">Application</span></span>|<span data-ttu-id="2dca0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2dca0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dca0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2dca0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2dca0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2dca0-119">Request headers</span></span>
|<span data-ttu-id="2dca0-120">标头</span><span class="sxs-lookup"><span data-stu-id="2dca0-120">Header</span></span>|<span data-ttu-id="2dca0-121">值</span><span class="sxs-lookup"><span data-stu-id="2dca0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dca0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dca0-122">Authorization</span></span>|<span data-ttu-id="2dca0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2dca0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dca0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2dca0-124">Accept</span></span>|<span data-ttu-id="2dca0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2dca0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dca0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2dca0-126">Request body</span></span>
<span data-ttu-id="2dca0-127">在请求正文中, 提供 groupPolicyConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dca0-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="2dca0-128">下表显示创建 groupPolicyConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2dca0-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="2dca0-129">属性</span><span class="sxs-lookup"><span data-stu-id="2dca0-129">Property</span></span>|<span data-ttu-id="2dca0-130">类型</span><span class="sxs-lookup"><span data-stu-id="2dca0-130">Type</span></span>|<span data-ttu-id="2dca0-131">说明</span><span class="sxs-lookup"><span data-stu-id="2dca0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dca0-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dca0-132">createdDateTime</span></span>|<span data-ttu-id="2dca0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dca0-133">DateTimeOffset</span></span>|<span data-ttu-id="2dca0-134">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2dca0-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="2dca0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2dca0-135">displayName</span></span>|<span data-ttu-id="2dca0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2dca0-136">String</span></span>|<span data-ttu-id="2dca0-137">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="2dca0-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="2dca0-138">说明</span><span class="sxs-lookup"><span data-stu-id="2dca0-138">description</span></span>|<span data-ttu-id="2dca0-139">字符串</span><span class="sxs-lookup"><span data-stu-id="2dca0-139">String</span></span>|<span data-ttu-id="2dca0-140">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="2dca0-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="2dca0-141">id</span><span class="sxs-lookup"><span data-stu-id="2dca0-141">id</span></span>|<span data-ttu-id="2dca0-142">String</span><span class="sxs-lookup"><span data-stu-id="2dca0-142">String</span></span>|<span data-ttu-id="2dca0-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2dca0-143">Key of the entity.</span></span>|
|<span data-ttu-id="2dca0-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dca0-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2dca0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dca0-145">DateTimeOffset</span></span>|<span data-ttu-id="2dca0-146">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2dca0-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2dca0-147">响应</span><span class="sxs-lookup"><span data-stu-id="2dca0-147">Response</span></span>
<span data-ttu-id="2dca0-148">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2dca0-148">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dca0-149">示例</span><span class="sxs-lookup"><span data-stu-id="2dca0-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dca0-150">请求</span><span class="sxs-lookup"><span data-stu-id="2dca0-150">Request</span></span>
<span data-ttu-id="2dca0-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2dca0-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2dca0-152">响应</span><span class="sxs-lookup"><span data-stu-id="2dca0-152">Response</span></span>
<span data-ttu-id="2dca0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2dca0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




