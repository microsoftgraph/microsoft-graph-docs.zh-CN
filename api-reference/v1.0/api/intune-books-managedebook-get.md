---
title: 获取 managedEBook
description: 读取 managedEBook 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 354cfbee964449195b4cc6a4260c7effb798d25f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758468"
---
# <a name="get-managedebook"></a><span data-ttu-id="56982-103">获取 managedEBook</span><span class="sxs-lookup"><span data-stu-id="56982-103">Get managedEBook</span></span>

<span data-ttu-id="56982-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56982-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56982-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56982-106">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56982-106">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56982-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="56982-107">Prerequisites</span></span>
<span data-ttu-id="56982-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56982-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="56982-110">Permission type</span></span>|<span data-ttu-id="56982-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56982-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56982-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56982-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56982-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56982-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56982-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56982-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56982-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56982-115">Not supported.</span></span>|
|<span data-ttu-id="56982-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="56982-116">Application</span></span>|<span data-ttu-id="56982-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56982-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56982-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56982-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56982-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56982-119">Optional query parameters</span></span>
<span data-ttu-id="56982-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="56982-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56982-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="56982-121">Request headers</span></span>
|<span data-ttu-id="56982-122">标头</span><span class="sxs-lookup"><span data-stu-id="56982-122">Header</span></span>|<span data-ttu-id="56982-123">值</span><span class="sxs-lookup"><span data-stu-id="56982-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56982-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="56982-124">Authorization</span></span>|<span data-ttu-id="56982-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56982-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56982-126">接受</span><span class="sxs-lookup"><span data-stu-id="56982-126">Accept</span></span>|<span data-ttu-id="56982-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56982-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56982-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="56982-128">Request body</span></span>
<span data-ttu-id="56982-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56982-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56982-130">响应</span><span class="sxs-lookup"><span data-stu-id="56982-130">Response</span></span>
<span data-ttu-id="56982-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedEBook](../resources/intune-books-managedebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56982-131">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56982-132">示例</span><span class="sxs-lookup"><span data-stu-id="56982-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="56982-133">请求</span><span class="sxs-lookup"><span data-stu-id="56982-133">Request</span></span>
<span data-ttu-id="56982-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56982-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="56982-135">响应</span><span class="sxs-lookup"><span data-stu-id="56982-135">Response</span></span>
<span data-ttu-id="56982-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56982-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```




