---
title: 创建 groupPolicyConfiguration
description: 创建新的 groupPolicyConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: faa91b75d086c8c6371b43e59e80700a3db74386
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685623"
---
# <a name="create-grouppolicyconfiguration"></a><span data-ttu-id="43162-103">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="43162-103">Create groupPolicyConfiguration</span></span>

<span data-ttu-id="43162-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43162-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43162-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43162-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43162-107">创建新的 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43162-107">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43162-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43162-108">Prerequisites</span></span>
<span data-ttu-id="43162-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43162-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43162-111">Permission type</span></span>|<span data-ttu-id="43162-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43162-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43162-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43162-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43162-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43162-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43162-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43162-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43162-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43162-116">Not supported.</span></span>|
|<span data-ttu-id="43162-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43162-117">Application</span></span>|<span data-ttu-id="43162-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43162-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43162-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43162-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43162-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43162-120">Request headers</span></span>
|<span data-ttu-id="43162-121">标头</span><span class="sxs-lookup"><span data-stu-id="43162-121">Header</span></span>|<span data-ttu-id="43162-122">值</span><span class="sxs-lookup"><span data-stu-id="43162-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43162-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43162-123">Authorization</span></span>|<span data-ttu-id="43162-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43162-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43162-125">接受</span><span class="sxs-lookup"><span data-stu-id="43162-125">Accept</span></span>|<span data-ttu-id="43162-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43162-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43162-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43162-127">Request body</span></span>
<span data-ttu-id="43162-128">在请求正文中，提供 groupPolicyConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43162-128">In the request body, supply a JSON representation for the groupPolicyConfiguration object.</span></span>

<span data-ttu-id="43162-129">下表显示创建 groupPolicyConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43162-129">The following table shows the properties that are required when you create the groupPolicyConfiguration.</span></span>

|<span data-ttu-id="43162-130">属性</span><span class="sxs-lookup"><span data-stu-id="43162-130">Property</span></span>|<span data-ttu-id="43162-131">类型</span><span class="sxs-lookup"><span data-stu-id="43162-131">Type</span></span>|<span data-ttu-id="43162-132">说明</span><span class="sxs-lookup"><span data-stu-id="43162-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43162-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43162-133">createdDateTime</span></span>|<span data-ttu-id="43162-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43162-134">DateTimeOffset</span></span>|<span data-ttu-id="43162-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43162-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="43162-136">displayName</span><span class="sxs-lookup"><span data-stu-id="43162-136">displayName</span></span>|<span data-ttu-id="43162-137">String</span><span class="sxs-lookup"><span data-stu-id="43162-137">String</span></span>|<span data-ttu-id="43162-138">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="43162-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="43162-139">说明</span><span class="sxs-lookup"><span data-stu-id="43162-139">description</span></span>|<span data-ttu-id="43162-140">String</span><span class="sxs-lookup"><span data-stu-id="43162-140">String</span></span>|<span data-ttu-id="43162-141">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="43162-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="43162-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43162-142">roleScopeTagIds</span></span>|<span data-ttu-id="43162-143">String collection</span><span class="sxs-lookup"><span data-stu-id="43162-143">String collection</span></span>|<span data-ttu-id="43162-144">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="43162-144">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="43162-145">id</span><span class="sxs-lookup"><span data-stu-id="43162-145">id</span></span>|<span data-ttu-id="43162-146">String</span><span class="sxs-lookup"><span data-stu-id="43162-146">String</span></span>|<span data-ttu-id="43162-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43162-147">Key of the entity.</span></span>|
|<span data-ttu-id="43162-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43162-148">lastModifiedDateTime</span></span>|<span data-ttu-id="43162-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43162-149">DateTimeOffset</span></span>|<span data-ttu-id="43162-150">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="43162-150">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="43162-151">响应</span><span class="sxs-lookup"><span data-stu-id="43162-151">Response</span></span>
<span data-ttu-id="43162-152">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43162-152">If successful, this method returns a `201 Created` response code and a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43162-153">示例</span><span class="sxs-lookup"><span data-stu-id="43162-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="43162-154">请求</span><span class="sxs-lookup"><span data-stu-id="43162-154">Request</span></span>
<span data-ttu-id="43162-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43162-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43162-156">响应</span><span class="sxs-lookup"><span data-stu-id="43162-156">Response</span></span>
<span data-ttu-id="43162-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





