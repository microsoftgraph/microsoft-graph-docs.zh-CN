---
title: 获取 deviceAndAppManagementAssignmentFilter
description: 读取 deviceAndAppManagementAssignmentFilter 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ef4d24ff9c6cf8a49e1647d2268a73eb76aa274
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791740"
---
# <a name="get-deviceandappmanagementassignmentfilter"></a><span data-ttu-id="1a86c-103">获取 deviceAndAppManagementAssignmentFilter</span><span class="sxs-lookup"><span data-stu-id="1a86c-103">Get deviceAndAppManagementAssignmentFilter</span></span>

<span data-ttu-id="1a86c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a86c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a86c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a86c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a86c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a86c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a86c-107">读取[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a86c-107">Read properties and relationships of the [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a86c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a86c-108">Prerequisites</span></span>
<span data-ttu-id="1a86c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1a86c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1a86c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a86c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a86c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a86c-111">Permission type</span></span>|<span data-ttu-id="1a86c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a86c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a86c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a86c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a86c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a86c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a86c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a86c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a86c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a86c-116">Not supported.</span></span>|
|<span data-ttu-id="1a86c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a86c-117">Application</span></span>|<span data-ttu-id="1a86c-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a86c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a86c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a86c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a86c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a86c-120">Optional query parameters</span></span>
<span data-ttu-id="1a86c-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a86c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a86c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a86c-122">Request headers</span></span>
|<span data-ttu-id="1a86c-123">标头</span><span class="sxs-lookup"><span data-stu-id="1a86c-123">Header</span></span>|<span data-ttu-id="1a86c-124">值</span><span class="sxs-lookup"><span data-stu-id="1a86c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a86c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a86c-125">Authorization</span></span>|<span data-ttu-id="1a86c-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a86c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a86c-127">接受</span><span class="sxs-lookup"><span data-stu-id="1a86c-127">Accept</span></span>|<span data-ttu-id="1a86c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1a86c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a86c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a86c-129">Request body</span></span>
<span data-ttu-id="1a86c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a86c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a86c-131">响应</span><span class="sxs-lookup"><span data-stu-id="1a86c-131">Response</span></span>
<span data-ttu-id="1a86c-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a86c-132">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a86c-133">示例</span><span class="sxs-lookup"><span data-stu-id="1a86c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a86c-134">请求</span><span class="sxs-lookup"><span data-stu-id="1a86c-134">Request</span></span>
<span data-ttu-id="1a86c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a86c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

### <a name="response"></a><span data-ttu-id="1a86c-136">响应</span><span class="sxs-lookup"><span data-stu-id="1a86c-136">Response</span></span>
<span data-ttu-id="1a86c-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1a86c-137">Here is an example of the response.</span></span> <span data-ttu-id="1a86c-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1a86c-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a86c-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1a86c-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 487

{
  "value": {
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



