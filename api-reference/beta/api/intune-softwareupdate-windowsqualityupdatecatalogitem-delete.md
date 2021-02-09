---
title: 删除 windowsQualityUpdateCatalogItem
description: 删除 windowsQualityUpdateCatalogItem。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e20f01d403dda049a4f22e069cacb3bd7ef83f6c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160211"
---
# <a name="delete-windowsqualityupdatecatalogitem"></a><span data-ttu-id="d9b0e-103">删除 windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="d9b0e-103">Delete windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="d9b0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9b0e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9b0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b0e-107">删除 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-107">Deletes a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9b0e-108">Prerequisites</span></span>
<span data-ttu-id="d9b0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9b0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9b0e-111">Permission type</span></span>|<span data-ttu-id="d9b0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9b0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9b0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9b0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9b0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9b0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-116">Not supported.</span></span>|
|<span data-ttu-id="d9b0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9b0e-117">Application</span></span>|<span data-ttu-id="d9b0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9b0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9b0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d9b0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9b0e-120">Request headers</span></span>
|<span data-ttu-id="d9b0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="d9b0e-121">Header</span></span>|<span data-ttu-id="d9b0e-122">值</span><span class="sxs-lookup"><span data-stu-id="d9b0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9b0e-123">Authorization</span></span>|<span data-ttu-id="d9b0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="d9b0e-125">Accept</span></span>|<span data-ttu-id="d9b0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9b0e-127">Request body</span></span>
<span data-ttu-id="d9b0e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9b0e-129">响应</span><span class="sxs-lookup"><span data-stu-id="d9b0e-129">Response</span></span>
<span data-ttu-id="d9b0e-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9b0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="d9b0e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9b0e-132">请求</span><span class="sxs-lookup"><span data-stu-id="d9b0e-132">Request</span></span>
<span data-ttu-id="d9b0e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

### <a name="response"></a><span data-ttu-id="d9b0e-134">响应</span><span class="sxs-lookup"><span data-stu-id="d9b0e-134">Response</span></span>
<span data-ttu-id="d9b0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9b0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




