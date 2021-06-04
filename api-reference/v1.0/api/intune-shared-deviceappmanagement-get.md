---
title: 获取 deviceAppManagement
description: 读取 deviceAppManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bba1f299aec5a896796c045067c3d6f8c5eaa425
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732355"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="b07a8-103">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="b07a8-103">Get deviceAppManagement</span></span>

<span data-ttu-id="b07a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b07a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b07a8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b07a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07a8-106">读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b07a8-106">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b07a8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b07a8-107">Prerequisites</span></span>

<span data-ttu-id="b07a8-108">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="b07a8-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b07a8-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b07a8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b07a8-110">请注意，相应的权限因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="b07a8-110">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b07a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b07a8-111">Permission type</span></span>|<span data-ttu-id="b07a8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b07a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b07a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b07a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b07a8-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b07a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="b07a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b07a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b07a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b07a8-116">Not supported.</span></span>|
|<span data-ttu-id="b07a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b07a8-117">Application</span></span>|<span data-ttu-id="b07a8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b07a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b07a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b07a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b07a8-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b07a8-120">Optional query parameters</span></span>
<span data-ttu-id="b07a8-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b07a8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b07a8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b07a8-122">Request headers</span></span>
|<span data-ttu-id="b07a8-123">标头</span><span class="sxs-lookup"><span data-stu-id="b07a8-123">Header</span></span>|<span data-ttu-id="b07a8-124">值</span><span class="sxs-lookup"><span data-stu-id="b07a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b07a8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b07a8-125">Authorization</span></span>|<span data-ttu-id="b07a8-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b07a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b07a8-127">接受</span><span class="sxs-lookup"><span data-stu-id="b07a8-127">Accept</span></span>|<span data-ttu-id="b07a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b07a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b07a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b07a8-129">Request body</span></span>
<span data-ttu-id="b07a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b07a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b07a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="b07a8-131">Response</span></span>
<span data-ttu-id="b07a8-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b07a8-132">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="b07a8-133">示例请求</span><span class="sxs-lookup"><span data-stu-id="b07a8-133">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="b07a8-134">示例响应</span><span class="sxs-lookup"><span data-stu-id="b07a8-134">Example response</span></span>
<span data-ttu-id="b07a8-135">为简洁起见，可能会截断此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b07a8-135">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b07a8-136">所有属性都将从实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="b07a8-136">All properties will be returned from an actual call.</span></span>

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