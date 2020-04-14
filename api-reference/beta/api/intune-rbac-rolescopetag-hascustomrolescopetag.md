---
title: hasCustomRoleScopeTag 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a34f986559f7ba81465f51b0858577ee92a5c6da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437607"
---
# <a name="hascustomrolescopetag-function"></a><span data-ttu-id="a1703-103">hasCustomRoleScopeTag 函数</span><span class="sxs-lookup"><span data-stu-id="a1703-103">hasCustomRoleScopeTag function</span></span>

<span data-ttu-id="a1703-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1703-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1703-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1703-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1703-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1703-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1703-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1703-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1703-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1703-108">Prerequisites</span></span>
<span data-ttu-id="a1703-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1703-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1703-111">Permission type</span></span>|<span data-ttu-id="a1703-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1703-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1703-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1703-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1703-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1703-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a1703-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1703-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1703-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1703-116">Not supported.</span></span>|
|<span data-ttu-id="a1703-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1703-117">Application</span></span>|<span data-ttu-id="a1703-118">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1703-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1703-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1703-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/hasCustomRoleScopeTag
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/hasCustomRoleScopeTag
```

## <a name="request-headers"></a><span data-ttu-id="a1703-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1703-120">Request headers</span></span>
|<span data-ttu-id="a1703-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1703-121">Header</span></span>|<span data-ttu-id="a1703-122">值</span><span class="sxs-lookup"><span data-stu-id="a1703-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1703-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1703-123">Authorization</span></span>|<span data-ttu-id="a1703-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1703-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1703-125">接受</span><span class="sxs-lookup"><span data-stu-id="a1703-125">Accept</span></span>|<span data-ttu-id="a1703-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1703-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1703-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1703-127">Request body</span></span>
<span data-ttu-id="a1703-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1703-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1703-129">响应</span><span class="sxs-lookup"><span data-stu-id="a1703-129">Response</span></span>
<span data-ttu-id="a1703-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="a1703-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1703-131">示例</span><span class="sxs-lookup"><span data-stu-id="a1703-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1703-132">请求</span><span class="sxs-lookup"><span data-stu-id="a1703-132">Request</span></span>
<span data-ttu-id="a1703-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1703-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/hasCustomRoleScopeTag
```

### <a name="response"></a><span data-ttu-id="a1703-134">响应</span><span class="sxs-lookup"><span data-stu-id="a1703-134">Response</span></span>
<span data-ttu-id="a1703-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1703-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



