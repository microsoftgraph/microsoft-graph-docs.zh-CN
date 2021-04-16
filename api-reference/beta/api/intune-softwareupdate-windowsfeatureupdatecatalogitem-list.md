---
title: 列出 windowsFeatureUpdateCatalogItems
description: 列出 windowsFeatureUpdateCatalogItem 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e23993ccedff32e9ce50e4fa210468296bca1061
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866900"
---
# <a name="list-windowsfeatureupdatecatalogitems"></a><span data-ttu-id="c89f2-103">列出 windowsFeatureUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="c89f2-103">List windowsFeatureUpdateCatalogItems</span></span>

<span data-ttu-id="c89f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c89f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c89f2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c89f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c89f2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c89f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89f2-107">列出 [windowsFeatureUpdateCatalogItem 对象的属性和](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c89f2-107">List properties and relationships of the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c89f2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c89f2-108">Prerequisites</span></span>
<span data-ttu-id="c89f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c89f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89f2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c89f2-111">Permission type</span></span>|<span data-ttu-id="c89f2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c89f2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c89f2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c89f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c89f2-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89f2-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c89f2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c89f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c89f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c89f2-116">Not supported.</span></span>|
|<span data-ttu-id="c89f2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c89f2-117">Application</span></span>|<span data-ttu-id="c89f2-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89f2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c89f2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c89f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="c89f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c89f2-120">Request headers</span></span>
|<span data-ttu-id="c89f2-121">标头</span><span class="sxs-lookup"><span data-stu-id="c89f2-121">Header</span></span>|<span data-ttu-id="c89f2-122">值</span><span class="sxs-lookup"><span data-stu-id="c89f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c89f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89f2-123">Authorization</span></span>|<span data-ttu-id="c89f2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c89f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c89f2-125">接受</span><span class="sxs-lookup"><span data-stu-id="c89f2-125">Accept</span></span>|<span data-ttu-id="c89f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c89f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c89f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c89f2-127">Request body</span></span>
<span data-ttu-id="c89f2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c89f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c89f2-129">响应</span><span class="sxs-lookup"><span data-stu-id="c89f2-129">Response</span></span>
<span data-ttu-id="c89f2-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c89f2-130">If successful, this method returns a `200 OK` response code and a collection of [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c89f2-131">示例</span><span class="sxs-lookup"><span data-stu-id="c89f2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c89f2-132">请求</span><span class="sxs-lookup"><span data-stu-id="c89f2-132">Request</span></span>
<span data-ttu-id="c89f2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c89f2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
```

### <a name="response"></a><span data-ttu-id="c89f2-134">响应</span><span class="sxs-lookup"><span data-stu-id="c89f2-134">Response</span></span>
<span data-ttu-id="c89f2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c89f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
      "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
      "displayName": "Display Name value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
      "version": "Version value"
    }
  ]
}
```




