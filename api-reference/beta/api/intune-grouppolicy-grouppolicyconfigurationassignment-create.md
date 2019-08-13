---
title: 创建 groupPolicyConfigurationAssignment
description: 创建新的 groupPolicyConfigurationAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb68222ef982dcac3ee94bac7a14fe2f4c0bbf5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355197"
---
# <a name="create-grouppolicyconfigurationassignment"></a><span data-ttu-id="331b1-103">创建 groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="331b1-103">Create groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="331b1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="331b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="331b1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="331b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="331b1-106">创建新的[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="331b1-106">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="331b1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="331b1-107">Prerequisites</span></span>
<span data-ttu-id="331b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="331b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="331b1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="331b1-110">Permission type</span></span>|<span data-ttu-id="331b1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="331b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="331b1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="331b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="331b1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="331b1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="331b1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="331b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="331b1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="331b1-115">Not supported.</span></span>|
|<span data-ttu-id="331b1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="331b1-116">Application</span></span>|<span data-ttu-id="331b1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="331b1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="331b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="331b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="331b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="331b1-119">Request headers</span></span>
|<span data-ttu-id="331b1-120">标头</span><span class="sxs-lookup"><span data-stu-id="331b1-120">Header</span></span>|<span data-ttu-id="331b1-121">值</span><span class="sxs-lookup"><span data-stu-id="331b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="331b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="331b1-122">Authorization</span></span>|<span data-ttu-id="331b1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="331b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="331b1-124">接受</span><span class="sxs-lookup"><span data-stu-id="331b1-124">Accept</span></span>|<span data-ttu-id="331b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="331b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="331b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="331b1-126">Request body</span></span>
<span data-ttu-id="331b1-127">在请求正文中, 提供 groupPolicyConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="331b1-127">In the request body, supply a JSON representation for the groupPolicyConfigurationAssignment object.</span></span>

<span data-ttu-id="331b1-128">下表显示创建 groupPolicyConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="331b1-128">The following table shows the properties that are required when you create the groupPolicyConfigurationAssignment.</span></span>

|<span data-ttu-id="331b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="331b1-129">Property</span></span>|<span data-ttu-id="331b1-130">类型</span><span class="sxs-lookup"><span data-stu-id="331b1-130">Type</span></span>|<span data-ttu-id="331b1-131">说明</span><span class="sxs-lookup"><span data-stu-id="331b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="331b1-132">id</span><span class="sxs-lookup"><span data-stu-id="331b1-132">id</span></span>|<span data-ttu-id="331b1-133">String</span><span class="sxs-lookup"><span data-stu-id="331b1-133">String</span></span>|<span data-ttu-id="331b1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="331b1-134">Key of the entity.</span></span>|
|<span data-ttu-id="331b1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="331b1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="331b1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="331b1-136">DateTimeOffset</span></span>|<span data-ttu-id="331b1-137">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="331b1-137">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="331b1-138">target</span><span class="sxs-lookup"><span data-stu-id="331b1-138">target</span></span>|[<span data-ttu-id="331b1-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="331b1-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="331b1-140">以组策略配置为目标的组的类型。</span><span class="sxs-lookup"><span data-stu-id="331b1-140">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="331b1-141">响应</span><span class="sxs-lookup"><span data-stu-id="331b1-141">Response</span></span>
<span data-ttu-id="331b1-142">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="331b1-142">If successful, this method returns a `201 Created` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="331b1-143">示例</span><span class="sxs-lookup"><span data-stu-id="331b1-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="331b1-144">请求</span><span class="sxs-lookup"><span data-stu-id="331b1-144">Request</span></span>
<span data-ttu-id="331b1-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="331b1-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="331b1-146">响应</span><span class="sxs-lookup"><span data-stu-id="331b1-146">Response</span></span>
<span data-ttu-id="331b1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="331b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






