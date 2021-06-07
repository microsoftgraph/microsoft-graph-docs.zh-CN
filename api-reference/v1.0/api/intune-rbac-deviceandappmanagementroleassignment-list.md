---
title: 列出 deviceAndAppManagementRoleAssignments
description: 列出 deviceAndAppManagementRoleAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01a1c4c76a6340011437d3749abbdf8982d73b65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756230"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="5b3a9-103">列出 deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="5b3a9-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="5b3a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b3a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b3a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b3a9-106">列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b3a9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b3a9-107">Prerequisites</span></span>
<span data-ttu-id="5b3a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b3a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b3a9-110">Permission type</span></span>|<span data-ttu-id="5b3a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b3a9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b3a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b3a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b3a9-113">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b3a9-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5b3a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b3a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b3a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-115">Not supported.</span></span>|
|<span data-ttu-id="5b3a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b3a9-116">Application</span></span>|<span data-ttu-id="5b3a9-117">DeviceManagementRBAC.Read.All、DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b3a9-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b3a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b3a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="5b3a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b3a9-119">Request headers</span></span>
|<span data-ttu-id="5b3a9-120">标头</span><span class="sxs-lookup"><span data-stu-id="5b3a9-120">Header</span></span>|<span data-ttu-id="5b3a9-121">值</span><span class="sxs-lookup"><span data-stu-id="5b3a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b3a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b3a9-122">Authorization</span></span>|<span data-ttu-id="5b3a9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b3a9-124">接受</span><span class="sxs-lookup"><span data-stu-id="5b3a9-124">Accept</span></span>|<span data-ttu-id="5b3a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b3a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b3a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b3a9-126">Request body</span></span>
<span data-ttu-id="5b3a9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b3a9-128">响应</span><span class="sxs-lookup"><span data-stu-id="5b3a9-128">Response</span></span>
<span data-ttu-id="5b3a9-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b3a9-130">示例</span><span class="sxs-lookup"><span data-stu-id="5b3a9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b3a9-131">请求</span><span class="sxs-lookup"><span data-stu-id="5b3a9-131">Request</span></span>
<span data-ttu-id="5b3a9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="5b3a9-133">响应</span><span class="sxs-lookup"><span data-stu-id="5b3a9-133">Response</span></span>
<span data-ttu-id="5b3a9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b3a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
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




