---
title: 更新 groupPolicyConfiguration
description: 更新 groupPolicyConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6265e7b9382322a138c39f05f57daa4579452a82
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804483"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="a9096-103">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9096-103">Update groupPolicyConfiguration</span></span>

> <span data-ttu-id="a9096-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9096-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9096-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9096-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9096-106">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a9096-106">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9096-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9096-107">Prerequisites</span></span>
<span data-ttu-id="a9096-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9096-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9096-110">Permission type</span></span>|<span data-ttu-id="a9096-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9096-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9096-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9096-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9096-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9096-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9096-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9096-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9096-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9096-115">Not supported.</span></span>|
|<span data-ttu-id="a9096-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9096-116">Application</span></span>|<span data-ttu-id="a9096-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9096-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9096-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9096-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a9096-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9096-119">Request headers</span></span>
|<span data-ttu-id="a9096-120">标头</span><span class="sxs-lookup"><span data-stu-id="a9096-120">Header</span></span>|<span data-ttu-id="a9096-121">值</span><span class="sxs-lookup"><span data-stu-id="a9096-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9096-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9096-122">Authorization</span></span>|<span data-ttu-id="a9096-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9096-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9096-124">接受</span><span class="sxs-lookup"><span data-stu-id="a9096-124">Accept</span></span>|<span data-ttu-id="a9096-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9096-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9096-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9096-126">Request body</span></span>
<span data-ttu-id="a9096-127">在请求正文中，提供[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9096-127">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="a9096-128">下表显示创建[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9096-128">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="a9096-129">属性</span><span class="sxs-lookup"><span data-stu-id="a9096-129">Property</span></span>|<span data-ttu-id="a9096-130">类型</span><span class="sxs-lookup"><span data-stu-id="a9096-130">Type</span></span>|<span data-ttu-id="a9096-131">说明</span><span class="sxs-lookup"><span data-stu-id="a9096-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9096-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9096-132">createdDateTime</span></span>|<span data-ttu-id="a9096-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9096-133">DateTimeOffset</span></span>|<span data-ttu-id="a9096-134">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9096-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="a9096-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a9096-135">displayName</span></span>|<span data-ttu-id="a9096-136">String</span><span class="sxs-lookup"><span data-stu-id="a9096-136">String</span></span>|<span data-ttu-id="a9096-137">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="a9096-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="a9096-138">说明</span><span class="sxs-lookup"><span data-stu-id="a9096-138">description</span></span>|<span data-ttu-id="a9096-139">String</span><span class="sxs-lookup"><span data-stu-id="a9096-139">String</span></span>|<span data-ttu-id="a9096-140">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="a9096-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="a9096-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9096-141">roleScopeTagIds</span></span>|<span data-ttu-id="a9096-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a9096-142">String collection</span></span>|<span data-ttu-id="a9096-143">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="a9096-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="a9096-144">id</span><span class="sxs-lookup"><span data-stu-id="a9096-144">id</span></span>|<span data-ttu-id="a9096-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a9096-145">String</span></span>|<span data-ttu-id="a9096-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9096-146">Key of the entity.</span></span>|
|<span data-ttu-id="a9096-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9096-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a9096-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9096-148">DateTimeOffset</span></span>|<span data-ttu-id="a9096-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9096-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a9096-150">响应</span><span class="sxs-lookup"><span data-stu-id="a9096-150">Response</span></span>
<span data-ttu-id="a9096-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a9096-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9096-152">示例</span><span class="sxs-lookup"><span data-stu-id="a9096-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9096-153">请求</span><span class="sxs-lookup"><span data-stu-id="a9096-153">Request</span></span>
<span data-ttu-id="a9096-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9096-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a9096-155">响应</span><span class="sxs-lookup"><span data-stu-id="a9096-155">Response</span></span>
<span data-ttu-id="a9096-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9096-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




