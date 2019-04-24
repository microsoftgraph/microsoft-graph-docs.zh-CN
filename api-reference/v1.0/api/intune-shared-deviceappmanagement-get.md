---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 841282551258c23dc57e34c06e803d4184f86809
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463598"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="b92a4-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b92a4-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="b92a4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b92a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b92a4-105">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b92a4-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b92a4-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b92a4-106">Prerequisites</span></span>

<span data-ttu-id="b92a4-107">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="b92a4-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b92a4-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b92a4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b92a4-109">请注意, 相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="b92a4-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b92a4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b92a4-110">Permission type</span></span>|<span data-ttu-id="b92a4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b92a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b92a4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b92a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b92a4-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b92a4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="b92a4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b92a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b92a4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b92a4-115">Not supported.</span></span>|
|<span data-ttu-id="b92a4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b92a4-116">Application</span></span>|<span data-ttu-id="b92a4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b92a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b92a4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b92a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b92a4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b92a4-119">Optional query parameters</span></span>
<span data-ttu-id="b92a4-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b92a4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b92a4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b92a4-121">Request headers</span></span>
|<span data-ttu-id="b92a4-122">标头</span><span class="sxs-lookup"><span data-stu-id="b92a4-122">Header</span></span>|<span data-ttu-id="b92a4-123">值</span><span class="sxs-lookup"><span data-stu-id="b92a4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b92a4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b92a4-124">Authorization</span></span>|<span data-ttu-id="b92a4-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b92a4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b92a4-126">接受</span><span class="sxs-lookup"><span data-stu-id="b92a4-126">Accept</span></span>|<span data-ttu-id="b92a4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b92a4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b92a4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b92a4-128">Request body</span></span>
<span data-ttu-id="b92a4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b92a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b92a4-130">响应</span><span class="sxs-lookup"><span data-stu-id="b92a4-130">Response</span></span>
<span data-ttu-id="b92a4-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b92a4-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="b92a4-132">示例请求</span><span class="sxs-lookup"><span data-stu-id="b92a4-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="b92a4-133">响应示例</span><span class="sxs-lookup"><span data-stu-id="b92a4-133">Example response</span></span>
<span data-ttu-id="b92a4-134">为简洁起见, 可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b92a4-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b92a4-135">所有属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b92a4-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



