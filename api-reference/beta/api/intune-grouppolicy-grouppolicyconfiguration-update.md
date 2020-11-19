---
title: 更新 groupPolicyConfiguration
description: 更新 groupPolicyConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0156d4b84d4e4b2f5b0e144414c79a7ec0bbe884
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49227915"
---
# <a name="update-grouppolicyconfiguration"></a><span data-ttu-id="9c0fe-103">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c0fe-103">Update groupPolicyConfiguration</span></span>

<span data-ttu-id="9c0fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c0fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c0fe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c0fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c0fe-107">更新 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-107">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c0fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c0fe-108">Prerequisites</span></span>
<span data-ttu-id="9c0fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c0fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c0fe-111">Permission type</span></span>|<span data-ttu-id="9c0fe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c0fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c0fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c0fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c0fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c0fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c0fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-116">Not supported.</span></span>|
|<span data-ttu-id="9c0fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c0fe-117">Application</span></span>|<span data-ttu-id="9c0fe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c0fe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c0fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c0fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9c0fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c0fe-120">Request headers</span></span>
|<span data-ttu-id="9c0fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c0fe-121">Header</span></span>|<span data-ttu-id="9c0fe-122">值</span><span class="sxs-lookup"><span data-stu-id="9c0fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c0fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c0fe-123">Authorization</span></span>|<span data-ttu-id="9c0fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c0fe-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c0fe-125">Accept</span></span>|<span data-ttu-id="9c0fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c0fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c0fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c0fe-127">Request body</span></span>
<span data-ttu-id="9c0fe-128">在请求正文中，提供 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-128">In the request body, supply a JSON representation for the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

<span data-ttu-id="9c0fe-129">下表显示创建 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-129">The following table shows the properties that are required when you create the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>

|<span data-ttu-id="9c0fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c0fe-130">Property</span></span>|<span data-ttu-id="9c0fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c0fe-131">Type</span></span>|<span data-ttu-id="9c0fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c0fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c0fe-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c0fe-133">createdDateTime</span></span>|<span data-ttu-id="9c0fe-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c0fe-134">DateTimeOffset</span></span>|<span data-ttu-id="9c0fe-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="9c0fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9c0fe-136">displayName</span></span>|<span data-ttu-id="9c0fe-137">String</span><span class="sxs-lookup"><span data-stu-id="9c0fe-137">String</span></span>|<span data-ttu-id="9c0fe-138">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="9c0fe-139">description</span><span class="sxs-lookup"><span data-stu-id="9c0fe-139">description</span></span>|<span data-ttu-id="9c0fe-140">String</span><span class="sxs-lookup"><span data-stu-id="9c0fe-140">String</span></span>|<span data-ttu-id="9c0fe-141">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="9c0fe-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c0fe-142">roleScopeTagIds</span></span>|<span data-ttu-id="9c0fe-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="9c0fe-143">String collection</span></span>|<span data-ttu-id="9c0fe-144">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="9c0fe-145">id</span><span class="sxs-lookup"><span data-stu-id="9c0fe-145">id</span></span>|<span data-ttu-id="9c0fe-146">String</span><span class="sxs-lookup"><span data-stu-id="9c0fe-146">String</span></span>|<span data-ttu-id="9c0fe-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-147">Key of the entity.</span></span>|
|<span data-ttu-id="9c0fe-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c0fe-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9c0fe-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c0fe-149">DateTimeOffset</span></span>|<span data-ttu-id="9c0fe-150">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="9c0fe-151">响应</span><span class="sxs-lookup"><span data-stu-id="9c0fe-151">Response</span></span>
<span data-ttu-id="9c0fe-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c0fe-153">示例</span><span class="sxs-lookup"><span data-stu-id="9c0fe-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c0fe-154">请求</span><span class="sxs-lookup"><span data-stu-id="9c0fe-154">Request</span></span>
<span data-ttu-id="9c0fe-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c0fe-156">响应</span><span class="sxs-lookup"><span data-stu-id="9c0fe-156">Response</span></span>
<span data-ttu-id="9c0fe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c0fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




