---
title: 获取 roleScopeTagAutoAssignment
description: 读取 roleScopeTagAutoAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 676ce7d9707217c692b600467bd841941a927333
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791670"
---
# <a name="get-rolescopetagautoassignment"></a><span data-ttu-id="04075-103">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="04075-103">Get roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="04075-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04075-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04075-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04075-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04075-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04075-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04075-107">读取[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04075-107">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04075-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="04075-108">Prerequisites</span></span>
<span data-ttu-id="04075-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="04075-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="04075-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04075-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04075-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="04075-111">Permission type</span></span>|<span data-ttu-id="04075-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04075-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04075-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04075-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04075-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="04075-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="04075-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04075-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04075-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04075-116">Not supported.</span></span>|
|<span data-ttu-id="04075-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="04075-117">Application</span></span>|<span data-ttu-id="04075-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="04075-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04075-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04075-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04075-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="04075-120">Optional query parameters</span></span>
<span data-ttu-id="04075-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="04075-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04075-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="04075-122">Request headers</span></span>
|<span data-ttu-id="04075-123">标头</span><span class="sxs-lookup"><span data-stu-id="04075-123">Header</span></span>|<span data-ttu-id="04075-124">值</span><span class="sxs-lookup"><span data-stu-id="04075-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04075-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="04075-125">Authorization</span></span>|<span data-ttu-id="04075-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04075-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04075-127">接受</span><span class="sxs-lookup"><span data-stu-id="04075-127">Accept</span></span>|<span data-ttu-id="04075-128">application/json</span><span class="sxs-lookup"><span data-stu-id="04075-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04075-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="04075-129">Request body</span></span>
<span data-ttu-id="04075-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04075-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04075-131">响应</span><span class="sxs-lookup"><span data-stu-id="04075-131">Response</span></span>
<span data-ttu-id="04075-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04075-132">If successful, this method returns a `200 OK` response code and [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04075-133">示例</span><span class="sxs-lookup"><span data-stu-id="04075-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="04075-134">请求</span><span class="sxs-lookup"><span data-stu-id="04075-134">Request</span></span>
<span data-ttu-id="04075-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04075-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

### <a name="response"></a><span data-ttu-id="04075-136">响应</span><span class="sxs-lookup"><span data-stu-id="04075-136">Response</span></span>
<span data-ttu-id="04075-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="04075-137">Here is an example of the response.</span></span> <span data-ttu-id="04075-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="04075-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="04075-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="04075-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
    "id": "256e6375-6375-256e-7563-6e2575636e25",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```



