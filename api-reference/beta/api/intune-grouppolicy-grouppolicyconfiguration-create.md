---
title: 创建 groupPolicyConfiguration
description: 创建新的 groupPolicyConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1a41f844c0a2773de968be985abbe8bf812c7a5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804497"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="48292-103">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="48292-103">Create groupPolicyConfiguration</span></span>

> <span data-ttu-id="48292-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="48292-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48292-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48292-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48292-106">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48292-106">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48292-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="48292-107">Prerequisites</span></span>
<span data-ttu-id="48292-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48292-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="48292-110">Permission type</span></span>|<span data-ttu-id="48292-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48292-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48292-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48292-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48292-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48292-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48292-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48292-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48292-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="48292-115">Not supported.</span></span>|
|<span data-ttu-id="48292-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="48292-116">Application</span></span>|<span data-ttu-id="48292-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48292-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48292-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48292-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48292-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="48292-119">Request headers</span></span>
|<span data-ttu-id="48292-120">标头</span><span class="sxs-lookup"><span data-stu-id="48292-120">Header</span></span>|<span data-ttu-id="48292-121">值</span><span class="sxs-lookup"><span data-stu-id="48292-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48292-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48292-122">Authorization</span></span>|<span data-ttu-id="48292-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48292-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48292-124">接受</span><span class="sxs-lookup"><span data-stu-id="48292-124">Accept</span></span>|<span data-ttu-id="48292-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48292-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48292-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="48292-126">Request body</span></span>
<span data-ttu-id="48292-127">在请求正文中，提供 groupPolicyConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48292-127">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="48292-128">下表显示创建 groupPolicyConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48292-128">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="48292-129">属性</span><span class="sxs-lookup"><span data-stu-id="48292-129">Property</span></span>|<span data-ttu-id="48292-130">类型</span><span class="sxs-lookup"><span data-stu-id="48292-130">Type</span></span>|<span data-ttu-id="48292-131">说明</span><span class="sxs-lookup"><span data-stu-id="48292-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48292-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48292-132">createdDateTime</span></span>|<span data-ttu-id="48292-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48292-133">DateTimeOffset</span></span>|<span data-ttu-id="48292-134">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48292-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="48292-135">displayName</span><span class="sxs-lookup"><span data-stu-id="48292-135">displayName</span></span>|<span data-ttu-id="48292-136">String</span><span class="sxs-lookup"><span data-stu-id="48292-136">String</span></span>|<span data-ttu-id="48292-137">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="48292-137">User provided name for the resource object.</span></span>|
|<span data-ttu-id="48292-138">说明</span><span class="sxs-lookup"><span data-stu-id="48292-138">description</span></span>|<span data-ttu-id="48292-139">String</span><span class="sxs-lookup"><span data-stu-id="48292-139">String</span></span>|<span data-ttu-id="48292-140">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="48292-140">User provided description for the resource object.</span></span>|
|<span data-ttu-id="48292-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48292-141">roleScopeTagIds</span></span>|<span data-ttu-id="48292-142">String collection</span><span class="sxs-lookup"><span data-stu-id="48292-142">String collection</span></span>|<span data-ttu-id="48292-143">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="48292-143">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="48292-144">id</span><span class="sxs-lookup"><span data-stu-id="48292-144">id</span></span>|<span data-ttu-id="48292-145">字符串</span><span class="sxs-lookup"><span data-stu-id="48292-145">String</span></span>|<span data-ttu-id="48292-146">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48292-146">Key of the entity.</span></span>|
|<span data-ttu-id="48292-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48292-147">lastModifiedDateTime</span></span>|<span data-ttu-id="48292-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48292-148">DateTimeOffset</span></span>|<span data-ttu-id="48292-149">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48292-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="48292-150">响应</span><span class="sxs-lookup"><span data-stu-id="48292-150">Response</span></span>
<span data-ttu-id="48292-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48292-151">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48292-152">示例</span><span class="sxs-lookup"><span data-stu-id="48292-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="48292-153">请求</span><span class="sxs-lookup"><span data-stu-id="48292-153">Request</span></span>
<span data-ttu-id="48292-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48292-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations
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

### <a name="response"></a><span data-ttu-id="48292-155">响应</span><span class="sxs-lookup"><span data-stu-id="48292-155">Response</span></span>
<span data-ttu-id="48292-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




