---
title: 获取 iosVppEBookAssignment
description: 读取 iosVppEBookAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6a235952ee32ea8db9dada6e05ea8b516f04490
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758419"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="54ac8-103">获取 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="54ac8-103">Get iosVppEBookAssignment</span></span>

<span data-ttu-id="54ac8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54ac8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54ac8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54ac8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54ac8-106">读取 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54ac8-106">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54ac8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="54ac8-107">Prerequisites</span></span>
<span data-ttu-id="54ac8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54ac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54ac8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="54ac8-110">Permission type</span></span>|<span data-ttu-id="54ac8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54ac8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54ac8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54ac8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54ac8-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ac8-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54ac8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54ac8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54ac8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="54ac8-115">Not supported.</span></span>|
|<span data-ttu-id="54ac8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="54ac8-116">Application</span></span>|<span data-ttu-id="54ac8-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ac8-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54ac8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54ac8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54ac8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54ac8-119">Optional query parameters</span></span>
<span data-ttu-id="54ac8-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54ac8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54ac8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="54ac8-121">Request headers</span></span>
|<span data-ttu-id="54ac8-122">标头</span><span class="sxs-lookup"><span data-stu-id="54ac8-122">Header</span></span>|<span data-ttu-id="54ac8-123">值</span><span class="sxs-lookup"><span data-stu-id="54ac8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54ac8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54ac8-124">Authorization</span></span>|<span data-ttu-id="54ac8-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="54ac8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54ac8-126">接受</span><span class="sxs-lookup"><span data-stu-id="54ac8-126">Accept</span></span>|<span data-ttu-id="54ac8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54ac8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54ac8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="54ac8-128">Request body</span></span>
<span data-ttu-id="54ac8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54ac8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54ac8-130">响应</span><span class="sxs-lookup"><span data-stu-id="54ac8-130">Response</span></span>
<span data-ttu-id="54ac8-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54ac8-131">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54ac8-132">示例</span><span class="sxs-lookup"><span data-stu-id="54ac8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="54ac8-133">请求</span><span class="sxs-lookup"><span data-stu-id="54ac8-133">Request</span></span>
<span data-ttu-id="54ac8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54ac8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="54ac8-135">响应</span><span class="sxs-lookup"><span data-stu-id="54ac8-135">Response</span></span>
<span data-ttu-id="54ac8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54ac8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
    "id": "48f05789-5789-48f0-8957-f0488957f048",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```




