---
title: 列出 deviceAndAppManagementRoleAssignments
description: 列出 deviceAndAppManagementRoleAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 132b30f251822e9403cad05651ad1eccfc875f51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980217"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="119cd-103">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="119cd-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="119cd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="119cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="119cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="119cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="119cd-106">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="119cd-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="119cd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="119cd-107">Prerequisites</span></span>
<span data-ttu-id="119cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="119cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="119cd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="119cd-110">Permission type</span></span>|<span data-ttu-id="119cd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="119cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="119cd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="119cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="119cd-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="119cd-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="119cd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="119cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="119cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="119cd-115">Not supported.</span></span>|
|<span data-ttu-id="119cd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="119cd-116">Application</span></span>|<span data-ttu-id="119cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="119cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="119cd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="119cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="119cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="119cd-119">Request headers</span></span>
|<span data-ttu-id="119cd-120">标头</span><span class="sxs-lookup"><span data-stu-id="119cd-120">Header</span></span>|<span data-ttu-id="119cd-121">值</span><span class="sxs-lookup"><span data-stu-id="119cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="119cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="119cd-122">Authorization</span></span>|<span data-ttu-id="119cd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="119cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="119cd-124">接受</span><span class="sxs-lookup"><span data-stu-id="119cd-124">Accept</span></span>|<span data-ttu-id="119cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="119cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="119cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="119cd-126">Request body</span></span>
<span data-ttu-id="119cd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="119cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="119cd-128">响应</span><span class="sxs-lookup"><span data-stu-id="119cd-128">Response</span></span>
<span data-ttu-id="119cd-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="119cd-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="119cd-130">示例</span><span class="sxs-lookup"><span data-stu-id="119cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="119cd-131">请求</span><span class="sxs-lookup"><span data-stu-id="119cd-131">Request</span></span>
<span data-ttu-id="119cd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="119cd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="119cd-133">响应</span><span class="sxs-lookup"><span data-stu-id="119cd-133">Response</span></span>
<span data-ttu-id="119cd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="119cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "members": [
        "Members value"
      ]
    }
  ]
}
```





