---
title: 更新 rbacApplicationMultiple
description: 更新 rbacApplicationMultiple 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0d835f328bf68efe09aa55f853a0e713b1e41c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940782"
---
# <a name="update-rbacapplicationmultiple"></a><span data-ttu-id="0475c-103">更新 rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="0475c-103">Update rbacApplicationMultiple</span></span>

> <span data-ttu-id="0475c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0475c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0475c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0475c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0475c-106">更新[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0475c-106">Update the properties of a [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0475c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0475c-107">Prerequisites</span></span>
<span data-ttu-id="0475c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0475c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0475c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0475c-110">Permission type</span></span>|<span data-ttu-id="0475c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0475c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0475c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0475c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0475c-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0475c-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0475c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0475c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0475c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0475c-115">Not supported.</span></span>|
|<span data-ttu-id="0475c-116">Application</span><span class="sxs-lookup"><span data-stu-id="0475c-116">Application</span></span>|<span data-ttu-id="0475c-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0475c-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0475c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0475c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="0475c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0475c-119">Request headers</span></span>
|<span data-ttu-id="0475c-120">标头</span><span class="sxs-lookup"><span data-stu-id="0475c-120">Header</span></span>|<span data-ttu-id="0475c-121">值</span><span class="sxs-lookup"><span data-stu-id="0475c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0475c-122">授权</span><span class="sxs-lookup"><span data-stu-id="0475c-122">Authorization</span></span>|<span data-ttu-id="0475c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0475c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0475c-124">接受</span><span class="sxs-lookup"><span data-stu-id="0475c-124">Accept</span></span>|<span data-ttu-id="0475c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0475c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0475c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0475c-126">Request body</span></span>
<span data-ttu-id="0475c-127">在请求正文中，提供[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0475c-127">In the request body, supply a JSON representation for the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object.</span></span>

<span data-ttu-id="0475c-128">下表显示创建[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0475c-128">The following table shows the properties that are required when you create the [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md).</span></span>

|<span data-ttu-id="0475c-129">属性</span><span class="sxs-lookup"><span data-stu-id="0475c-129">Property</span></span>|<span data-ttu-id="0475c-130">类型</span><span class="sxs-lookup"><span data-stu-id="0475c-130">Type</span></span>|<span data-ttu-id="0475c-131">说明</span><span class="sxs-lookup"><span data-stu-id="0475c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0475c-132">id</span><span class="sxs-lookup"><span data-stu-id="0475c-132">id</span></span>|<span data-ttu-id="0475c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0475c-133">String</span></span>|<span data-ttu-id="0475c-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0475c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0475c-135">响应</span><span class="sxs-lookup"><span data-stu-id="0475c-135">Response</span></span>
<span data-ttu-id="0475c-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0475c-136">If successful, this method returns a `200 OK` response code and an updated [rbacApplicationMultiple](../resources/intune-rbac-rbacapplicationmultiple.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0475c-137">示例</span><span class="sxs-lookup"><span data-stu-id="0475c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="0475c-138">请求</span><span class="sxs-lookup"><span data-stu-id="0475c-138">Request</span></span>
<span data-ttu-id="0475c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0475c-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a><span data-ttu-id="0475c-140">响应</span><span class="sxs-lookup"><span data-stu-id="0475c-140">Response</span></span>
<span data-ttu-id="0475c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0475c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```





