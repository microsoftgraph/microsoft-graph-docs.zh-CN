---
title: 更新 rbacApplicationMultiple
description: 更新 rbacApplicationMultiple 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ff5e5cfff449c305c794024f7cedeaa031f358a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148468"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="87991-103">更新 rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="87991-103">Update rbacApplicationMultiple</span></span>

<span data-ttu-id="87991-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87991-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87991-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87991-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87991-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87991-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87991-107">更新 [rbacApplicationMultiple 对象](../resources/intune-rbac-rbacapplicationmultiple.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="87991-107">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87991-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="87991-108">Prerequisites</span></span>
<span data-ttu-id="87991-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87991-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="87991-111">Permission type</span></span>|<span data-ttu-id="87991-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87991-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87991-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87991-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87991-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87991-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="87991-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87991-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87991-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87991-116">Not supported.</span></span>|
|<span data-ttu-id="87991-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="87991-117">Application</span></span>|<span data-ttu-id="87991-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87991-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87991-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87991-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="87991-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="87991-120">Request headers</span></span>
|<span data-ttu-id="87991-121">标头</span><span class="sxs-lookup"><span data-stu-id="87991-121">Header</span></span>|<span data-ttu-id="87991-122">值</span><span class="sxs-lookup"><span data-stu-id="87991-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87991-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87991-123">Authorization</span></span>|<span data-ttu-id="87991-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87991-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87991-125">接受</span><span class="sxs-lookup"><span data-stu-id="87991-125">Accept</span></span>|<span data-ttu-id="87991-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87991-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87991-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="87991-127">Request body</span></span>
<span data-ttu-id="87991-128">在请求正文中，提供 [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87991-128">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="87991-129">下表显示创建 [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87991-129">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="87991-130">属性</span><span class="sxs-lookup"><span data-stu-id="87991-130">Property</span></span>|<span data-ttu-id="87991-131">类型</span><span class="sxs-lookup"><span data-stu-id="87991-131">Type</span></span>|<span data-ttu-id="87991-132">说明</span><span class="sxs-lookup"><span data-stu-id="87991-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87991-133">id</span><span class="sxs-lookup"><span data-stu-id="87991-133">id</span></span>|<span data-ttu-id="87991-134">String</span><span class="sxs-lookup"><span data-stu-id="87991-134">String</span></span>|<span data-ttu-id="87991-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="87991-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="87991-136">响应</span><span class="sxs-lookup"><span data-stu-id="87991-136">Response</span></span>
<span data-ttu-id="87991-137">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="87991-137">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87991-138">示例</span><span class="sxs-lookup"><span data-stu-id="87991-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="87991-139">请求</span><span class="sxs-lookup"><span data-stu-id="87991-139">Request</span></span>
<span data-ttu-id="87991-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87991-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="87991-141">响应</span><span class="sxs-lookup"><span data-stu-id="87991-141">Response</span></span>
<span data-ttu-id="87991-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87991-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```




