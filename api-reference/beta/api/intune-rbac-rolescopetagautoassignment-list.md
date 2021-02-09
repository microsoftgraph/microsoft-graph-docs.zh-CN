---
title: 列出 roleScopeTagAutoAssignments
description: 列出 roleScopeTagAutoAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf86f41d33082dd7fa7faec4446b5b887d6a6aec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153731"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="02e2d-103">列出 roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="02e2d-103">List roleScopeTagAutoAssignments</span></span>

<span data-ttu-id="02e2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e2d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02e2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e2d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02e2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e2d-107">列出 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02e2d-107">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e2d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="02e2d-108">Prerequisites</span></span>
<span data-ttu-id="02e2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02e2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e2d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02e2d-111">Permission type</span></span>|<span data-ttu-id="02e2d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02e2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e2d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02e2d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02e2d-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e2d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="02e2d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02e2d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e2d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02e2d-116">Not supported.</span></span>|
|<span data-ttu-id="02e2d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02e2d-117">Application</span></span>|<span data-ttu-id="02e2d-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="02e2d-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e2d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02e2d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="02e2d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02e2d-120">Request headers</span></span>
|<span data-ttu-id="02e2d-121">标头</span><span class="sxs-lookup"><span data-stu-id="02e2d-121">Header</span></span>|<span data-ttu-id="02e2d-122">值</span><span class="sxs-lookup"><span data-stu-id="02e2d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02e2d-123">Authorization</span></span>|<span data-ttu-id="02e2d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02e2d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e2d-125">接受</span><span class="sxs-lookup"><span data-stu-id="02e2d-125">Accept</span></span>|<span data-ttu-id="02e2d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02e2d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e2d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="02e2d-127">Request body</span></span>
<span data-ttu-id="02e2d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02e2d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02e2d-129">响应</span><span class="sxs-lookup"><span data-stu-id="02e2d-129">Response</span></span>
<span data-ttu-id="02e2d-130">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="02e2d-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e2d-131">示例</span><span class="sxs-lookup"><span data-stu-id="02e2d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e2d-132">请求</span><span class="sxs-lookup"><span data-stu-id="02e2d-132">Request</span></span>
<span data-ttu-id="02e2d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02e2d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="02e2d-134">响应</span><span class="sxs-lookup"><span data-stu-id="02e2d-134">Response</span></span>
<span data-ttu-id="02e2d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02e2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 499

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




