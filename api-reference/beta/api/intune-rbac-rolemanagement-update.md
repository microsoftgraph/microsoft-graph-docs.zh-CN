---
title: 更新 roleManagement
description: 更新 roleManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 549d3ab5bc3e4d248ba81bf5c0059a6fcd0d5e90
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156672"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="405db-103">更新 roleManagement</span><span class="sxs-lookup"><span data-stu-id="405db-103">Update roleManagement</span></span>

<span data-ttu-id="405db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="405db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="405db-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="405db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="405db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="405db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="405db-107">更新 [roleManagement 对象](../resources/intune-rbac-rolemanagement.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="405db-107">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="405db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="405db-108">Prerequisites</span></span>
<span data-ttu-id="405db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="405db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="405db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="405db-111">Permission type</span></span>|<span data-ttu-id="405db-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="405db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="405db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="405db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="405db-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405db-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="405db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="405db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="405db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="405db-116">Not supported.</span></span>|
|<span data-ttu-id="405db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="405db-117">Application</span></span>|<span data-ttu-id="405db-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405db-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="405db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="405db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="405db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="405db-120">Request headers</span></span>
|<span data-ttu-id="405db-121">标头</span><span class="sxs-lookup"><span data-stu-id="405db-121">Header</span></span>|<span data-ttu-id="405db-122">值</span><span class="sxs-lookup"><span data-stu-id="405db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="405db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="405db-123">Authorization</span></span>|<span data-ttu-id="405db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="405db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="405db-125">接受</span><span class="sxs-lookup"><span data-stu-id="405db-125">Accept</span></span>|<span data-ttu-id="405db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="405db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="405db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="405db-127">Request body</span></span>
<span data-ttu-id="405db-128">在请求正文中，提供 [roleManagement](../resources/intune-rbac-rolemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="405db-128">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="405db-129">下表显示创建 [roleManagement 时所需的属性](../resources/intune-rbac-rolemanagement.md)。</span><span class="sxs-lookup"><span data-stu-id="405db-129">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="405db-130">属性</span><span class="sxs-lookup"><span data-stu-id="405db-130">Property</span></span>|<span data-ttu-id="405db-131">类型</span><span class="sxs-lookup"><span data-stu-id="405db-131">Type</span></span>|<span data-ttu-id="405db-132">说明</span><span class="sxs-lookup"><span data-stu-id="405db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="405db-133">id</span><span class="sxs-lookup"><span data-stu-id="405db-133">id</span></span>|<span data-ttu-id="405db-134">String</span><span class="sxs-lookup"><span data-stu-id="405db-134">String</span></span>|<span data-ttu-id="405db-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="405db-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="405db-136">响应</span><span class="sxs-lookup"><span data-stu-id="405db-136">Response</span></span>
<span data-ttu-id="405db-137">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [roleManagement](../resources/intune-rbac-rolemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="405db-137">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="405db-138">示例</span><span class="sxs-lookup"><span data-stu-id="405db-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="405db-139">请求</span><span class="sxs-lookup"><span data-stu-id="405db-139">Request</span></span>
<span data-ttu-id="405db-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="405db-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="405db-141">响应</span><span class="sxs-lookup"><span data-stu-id="405db-141">Response</span></span>
<span data-ttu-id="405db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="405db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```




