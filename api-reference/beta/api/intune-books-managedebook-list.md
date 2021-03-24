---
title: 列出 managedEBooks
description: 列出 managedEBook 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f985fb906b50e3a17368e24174ac5a5aab8dfb8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133120"
---
# <a name="list-managedebooks"></a><span data-ttu-id="3a477-103">列出 managedEBooks</span><span class="sxs-lookup"><span data-stu-id="3a477-103">List managedEBooks</span></span>

<span data-ttu-id="3a477-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a477-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a477-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a477-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a477-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a477-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a477-107">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a477-107">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a477-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3a477-108">Prerequisites</span></span>
<span data-ttu-id="3a477-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a477-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a477-111">Permission type</span></span>|<span data-ttu-id="3a477-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a477-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a477-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a477-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a477-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a477-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a477-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a477-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a477-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a477-116">Not supported.</span></span>|
|<span data-ttu-id="3a477-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a477-117">Application</span></span>|<span data-ttu-id="3a477-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a477-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a477-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a477-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="3a477-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a477-120">Request headers</span></span>
|<span data-ttu-id="3a477-121">标头</span><span class="sxs-lookup"><span data-stu-id="3a477-121">Header</span></span>|<span data-ttu-id="3a477-122">值</span><span class="sxs-lookup"><span data-stu-id="3a477-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a477-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a477-123">Authorization</span></span>|<span data-ttu-id="3a477-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3a477-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a477-125">接受</span><span class="sxs-lookup"><span data-stu-id="3a477-125">Accept</span></span>|<span data-ttu-id="3a477-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a477-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a477-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a477-127">Request body</span></span>
<span data-ttu-id="3a477-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3a477-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a477-129">响应</span><span class="sxs-lookup"><span data-stu-id="3a477-129">Response</span></span>
<span data-ttu-id="3a477-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedEBook](../resources/intune-books-managedebook.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3a477-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a477-131">示例</span><span class="sxs-lookup"><span data-stu-id="3a477-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a477-132">请求</span><span class="sxs-lookup"><span data-stu-id="3a477-132">Request</span></span>
<span data-ttu-id="3a477-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a477-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="3a477-134">响应</span><span class="sxs-lookup"><span data-stu-id="3a477-134">Response</span></span>
<span data-ttu-id="3a477-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a477-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```




