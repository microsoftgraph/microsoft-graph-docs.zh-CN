---
title: 获取 roleScopeTagAutoAssignment
description: 读取 roleScopeTagAutoAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c6973fdc7913c7aee246fe277132ee825fd0039
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159267"
---
# <a name="get-rolescopetagautoassignment"></a><span data-ttu-id="9afba-103">获取 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="9afba-103">Get roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="9afba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9afba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9afba-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9afba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9afba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9afba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9afba-107">读取 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9afba-107">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9afba-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9afba-108">Prerequisites</span></span>
<span data-ttu-id="9afba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9afba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9afba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9afba-111">Permission type</span></span>|<span data-ttu-id="9afba-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9afba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9afba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9afba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9afba-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9afba-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9afba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9afba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9afba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9afba-116">Not supported.</span></span>|
|<span data-ttu-id="9afba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9afba-117">Application</span></span>|<span data-ttu-id="9afba-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9afba-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9afba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9afba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9afba-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9afba-120">Optional query parameters</span></span>
<span data-ttu-id="9afba-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9afba-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9afba-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9afba-122">Request headers</span></span>
|<span data-ttu-id="9afba-123">标头</span><span class="sxs-lookup"><span data-stu-id="9afba-123">Header</span></span>|<span data-ttu-id="9afba-124">值</span><span class="sxs-lookup"><span data-stu-id="9afba-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9afba-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9afba-125">Authorization</span></span>|<span data-ttu-id="9afba-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9afba-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9afba-127">接受</span><span class="sxs-lookup"><span data-stu-id="9afba-127">Accept</span></span>|<span data-ttu-id="9afba-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9afba-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9afba-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9afba-129">Request body</span></span>
<span data-ttu-id="9afba-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9afba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9afba-131">响应</span><span class="sxs-lookup"><span data-stu-id="9afba-131">Response</span></span>
<span data-ttu-id="9afba-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9afba-132">If successful, this method returns a `200 OK` response code and [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9afba-133">示例</span><span class="sxs-lookup"><span data-stu-id="9afba-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9afba-134">请求</span><span class="sxs-lookup"><span data-stu-id="9afba-134">Request</span></span>
<span data-ttu-id="9afba-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9afba-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

### <a name="response"></a><span data-ttu-id="9afba-136">响应</span><span class="sxs-lookup"><span data-stu-id="9afba-136">Response</span></span>
<span data-ttu-id="9afba-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9afba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 469

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
    "id": "256e6375-6375-256e-7563-6e2575636e25",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    }
  }
}
```




