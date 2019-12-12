---
title: 更新 roleManagement
description: 更新 roleManagement 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2451397f5bde92f949174edef67c311ff1d966c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955173"
---
# <a name="update-rolemanagement"></a><span data-ttu-id="c1476-103">更新 roleManagement</span><span class="sxs-lookup"><span data-stu-id="c1476-103">Update roleManagement</span></span>

> <span data-ttu-id="c1476-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c1476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1476-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1476-106">更新[roleManagement](../resources/intune-rbac-rolemanagement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1476-106">Update the properties of a [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1476-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1476-107">Prerequisites</span></span>
<span data-ttu-id="c1476-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1476-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1476-110">Permission type</span></span>|<span data-ttu-id="c1476-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1476-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1476-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1476-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1476-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1476-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c1476-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1476-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1476-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1476-115">Not supported.</span></span>|
|<span data-ttu-id="c1476-116">Application</span><span class="sxs-lookup"><span data-stu-id="c1476-116">Application</span></span>|<span data-ttu-id="c1476-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1476-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1476-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1476-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a><span data-ttu-id="c1476-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1476-119">Request headers</span></span>
|<span data-ttu-id="c1476-120">标头</span><span class="sxs-lookup"><span data-stu-id="c1476-120">Header</span></span>|<span data-ttu-id="c1476-121">值</span><span class="sxs-lookup"><span data-stu-id="c1476-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1476-122">授权</span><span class="sxs-lookup"><span data-stu-id="c1476-122">Authorization</span></span>|<span data-ttu-id="c1476-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1476-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1476-124">接受</span><span class="sxs-lookup"><span data-stu-id="c1476-124">Accept</span></span>|<span data-ttu-id="c1476-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1476-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1476-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1476-126">Request body</span></span>
<span data-ttu-id="c1476-127">在请求正文中，提供[roleManagement](../resources/intune-rbac-rolemanagement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1476-127">In the request body, supply a JSON representation for the [roleManagement](../resources/intune-rbac-rolemanagement.md) object.</span></span>

<span data-ttu-id="c1476-128">下表显示创建[roleManagement](../resources/intune-rbac-rolemanagement.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c1476-128">The following table shows the properties that are required when you create the [roleManagement](../resources/intune-rbac-rolemanagement.md).</span></span>

|<span data-ttu-id="c1476-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1476-129">Property</span></span>|<span data-ttu-id="c1476-130">类型</span><span class="sxs-lookup"><span data-stu-id="c1476-130">Type</span></span>|<span data-ttu-id="c1476-131">说明</span><span class="sxs-lookup"><span data-stu-id="c1476-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1476-132">id</span><span class="sxs-lookup"><span data-stu-id="c1476-132">id</span></span>|<span data-ttu-id="c1476-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c1476-133">String</span></span>|<span data-ttu-id="c1476-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c1476-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c1476-135">响应</span><span class="sxs-lookup"><span data-stu-id="c1476-135">Response</span></span>
<span data-ttu-id="c1476-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[roleManagement](../resources/intune-rbac-rolemanagement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1476-136">If successful, this method returns a `200 OK` response code and an updated [roleManagement](../resources/intune-rbac-rolemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1476-137">示例</span><span class="sxs-lookup"><span data-stu-id="c1476-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1476-138">请求</span><span class="sxs-lookup"><span data-stu-id="c1476-138">Request</span></span>
<span data-ttu-id="c1476-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1476-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a><span data-ttu-id="c1476-140">响应</span><span class="sxs-lookup"><span data-stu-id="c1476-140">Response</span></span>
<span data-ttu-id="c1476-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1476-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```





