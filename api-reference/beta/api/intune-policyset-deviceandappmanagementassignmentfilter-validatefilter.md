---
title: validateFilter 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2315d4b42abd6289e77df767206197973e98fd3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160256"
---
# <a name="validatefilter-action"></a><span data-ttu-id="db08d-103">validateFilter 操作</span><span class="sxs-lookup"><span data-stu-id="db08d-103">validateFilter action</span></span>

<span data-ttu-id="db08d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db08d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db08d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db08d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db08d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db08d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db08d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="db08d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db08d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db08d-108">Prerequisites</span></span>
<span data-ttu-id="db08d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db08d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db08d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db08d-111">Permission type</span></span>|<span data-ttu-id="db08d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db08d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db08d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db08d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db08d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db08d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db08d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db08d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db08d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db08d-116">Not supported.</span></span>|
|<span data-ttu-id="db08d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db08d-117">Application</span></span>|<span data-ttu-id="db08d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db08d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db08d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db08d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/assignmentFilters/validateFilter
```

## <a name="request-headers"></a><span data-ttu-id="db08d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db08d-120">Request headers</span></span>
|<span data-ttu-id="db08d-121">标头</span><span class="sxs-lookup"><span data-stu-id="db08d-121">Header</span></span>|<span data-ttu-id="db08d-122">值</span><span class="sxs-lookup"><span data-stu-id="db08d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db08d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db08d-123">Authorization</span></span>|<span data-ttu-id="db08d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db08d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db08d-125">接受</span><span class="sxs-lookup"><span data-stu-id="db08d-125">Accept</span></span>|<span data-ttu-id="db08d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db08d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db08d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db08d-127">Request body</span></span>
<span data-ttu-id="db08d-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db08d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="db08d-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="db08d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="db08d-130">属性</span><span class="sxs-lookup"><span data-stu-id="db08d-130">Property</span></span>|<span data-ttu-id="db08d-131">类型</span><span class="sxs-lookup"><span data-stu-id="db08d-131">Type</span></span>|<span data-ttu-id="db08d-132">说明</span><span class="sxs-lookup"><span data-stu-id="db08d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db08d-133">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="db08d-133">deviceAndAppManagementAssignmentFilter</span></span>|[<span data-ttu-id="db08d-134">deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="db08d-134">deviceAndAppManagementAssignmentFilter</span></span>](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|<span data-ttu-id="db08d-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="db08d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="db08d-136">响应</span><span class="sxs-lookup"><span data-stu-id="db08d-136">Response</span></span>
<span data-ttu-id="db08d-137">如果成功，此操作在响应正文中返回响应代码和 `200 OK` [assignmentFilterValidationResult。](../resources/intune-policyset-assignmentfiltervalidationresult.md)</span><span class="sxs-lookup"><span data-stu-id="db08d-137">If successful, this action returns a `200 OK` response code and a [assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db08d-138">示例</span><span class="sxs-lookup"><span data-stu-id="db08d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="db08d-139">请求</span><span class="sxs-lookup"><span data-stu-id="db08d-139">Request</span></span>
<span data-ttu-id="db08d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db08d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/validateFilter

Content-type: application/json
Content-length: 520

{
  "deviceAndAppManagementAssignmentFilter": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
    "id": "819818db-18db-8198-db18-9881db189881",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "platform": "androidForWork",
    "rule": "Rule value",
    "roleScopeTags": [
      "Role Scope Tags value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="db08d-141">响应</span><span class="sxs-lookup"><span data-stu-id="db08d-141">Response</span></span>
<span data-ttu-id="db08d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db08d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterValidationResult",
    "isValidRule": true
  }
}
```




