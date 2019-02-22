---
title: 更新 groupPolicyConfiguration
description: 更新 groupPolicyConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 867d70f3978db683cb154b9e5405df08b315b4b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160030"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="24fc3-103">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="24fc3-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="24fc3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24fc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24fc3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24fc3-106">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24fc3-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24fc3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="24fc3-107">Prerequisites</span></span>
<span data-ttu-id="24fc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="24fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24fc3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="24fc3-110">Permission type</span></span>|<span data-ttu-id="24fc3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24fc3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24fc3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fc3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="24fc3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24fc3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24fc3-115">Not supported.</span></span>|
|<span data-ttu-id="24fc3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="24fc3-116">Application</span></span>|<span data-ttu-id="24fc3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="24fc3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24fc3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="24fc3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="24fc3-119">Request headers</span></span>
|<span data-ttu-id="24fc3-120">标头</span><span class="sxs-lookup"><span data-stu-id="24fc3-120">Header</span></span>|<span data-ttu-id="24fc3-121">值</span><span class="sxs-lookup"><span data-stu-id="24fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24fc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24fc3-122">Authorization</span></span>|<span data-ttu-id="24fc3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24fc3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="24fc3-124">Accept</span></span>|<span data-ttu-id="24fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24fc3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24fc3-126">Request body</span></span>
<span data-ttu-id="24fc3-127">在请求正文中, 提供[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24fc3-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="24fc3-128">下表显示创建[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24fc3-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="24fc3-129">属性</span><span class="sxs-lookup"><span data-stu-id="24fc3-129">Property</span></span>|<span data-ttu-id="24fc3-130">类型</span><span class="sxs-lookup"><span data-stu-id="24fc3-130">Type</span></span>|<span data-ttu-id="24fc3-131">说明</span><span class="sxs-lookup"><span data-stu-id="24fc3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24fc3-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24fc3-132">createdDateTime</span></span>|<span data-ttu-id="24fc3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24fc3-133">DateTimeOffset</span></span>|<span data-ttu-id="24fc3-134">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24fc3-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="24fc3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="24fc3-135">displayName</span></span>|<span data-ttu-id="24fc3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="24fc3-136">String</span></span>|<span data-ttu-id="24fc3-137">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="24fc3-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="24fc3-138">说明</span><span class="sxs-lookup"><span data-stu-id="24fc3-138">description</span></span>|<span data-ttu-id="24fc3-139">字符串</span><span class="sxs-lookup"><span data-stu-id="24fc3-139">String</span></span>|<span data-ttu-id="24fc3-140">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="24fc3-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="24fc3-141">id</span><span class="sxs-lookup"><span data-stu-id="24fc3-141">id</span></span>|<span data-ttu-id="24fc3-142">String</span><span class="sxs-lookup"><span data-stu-id="24fc3-142">String</span></span>|<span data-ttu-id="24fc3-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24fc3-143">Key of the entity.</span></span>|
|<span data-ttu-id="24fc3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24fc3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="24fc3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24fc3-145">DateTimeOffset</span></span>|<span data-ttu-id="24fc3-146">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24fc3-146">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="24fc3-147">响应</span><span class="sxs-lookup"><span data-stu-id="24fc3-147">Response</span></span>
<span data-ttu-id="24fc3-148">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24fc3-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fc3-149">示例</span><span class="sxs-lookup"><span data-stu-id="24fc3-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="24fc3-150">请求</span><span class="sxs-lookup"><span data-stu-id="24fc3-150">Request</span></span>
<span data-ttu-id="24fc3-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24fc3-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="24fc3-152">响应</span><span class="sxs-lookup"><span data-stu-id="24fc3-152">Response</span></span>
<span data-ttu-id="24fc3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24fc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




