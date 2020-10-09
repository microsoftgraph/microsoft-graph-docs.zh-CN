---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bba1f299aec5a896796c045067c3d6f8c5eaa425
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405048"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="deb42-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="deb42-103">Get deviceAppManagement</span></span>

<span data-ttu-id="deb42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="deb42-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="deb42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb42-106">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="deb42-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deb42-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="deb42-107">Prerequisites</span></span>

<span data-ttu-id="deb42-108">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="deb42-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="deb42-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deb42-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="deb42-110">请注意，相应的权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="deb42-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="deb42-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="deb42-111">Permission type</span></span>|<span data-ttu-id="deb42-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="deb42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb42-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deb42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="deb42-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="deb42-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="deb42-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deb42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb42-116">Not supported.</span></span>|
|<span data-ttu-id="deb42-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="deb42-117">Application</span></span>|<span data-ttu-id="deb42-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb42-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deb42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="deb42-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="deb42-120">Optional query parameters</span></span>
<span data-ttu-id="deb42-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="deb42-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deb42-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="deb42-122">Request headers</span></span>
|<span data-ttu-id="deb42-123">标头</span><span class="sxs-lookup"><span data-stu-id="deb42-123">Header</span></span>|<span data-ttu-id="deb42-124">值</span><span class="sxs-lookup"><span data-stu-id="deb42-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb42-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb42-125">Authorization</span></span>|<span data-ttu-id="deb42-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="deb42-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb42-127">接受</span><span class="sxs-lookup"><span data-stu-id="deb42-127">Accept</span></span>|<span data-ttu-id="deb42-128">application/json</span><span class="sxs-lookup"><span data-stu-id="deb42-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb42-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="deb42-129">Request body</span></span>
<span data-ttu-id="deb42-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="deb42-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deb42-131">响应</span><span class="sxs-lookup"><span data-stu-id="deb42-131">Response</span></span>
<span data-ttu-id="deb42-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deb42-132">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="deb42-133">示例请求</span><span class="sxs-lookup"><span data-stu-id="deb42-133">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="deb42-134">示例响应</span><span class="sxs-lookup"><span data-stu-id="deb42-134">Example response</span></span>
<span data-ttu-id="deb42-135">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="deb42-135">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="deb42-136">所有属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="deb42-136">All properties will be returned from an actual call.</span></span>

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