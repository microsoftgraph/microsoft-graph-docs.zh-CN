---
title: 列出 sideLoadingKeies
description: 列出 sideLoadingKey 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d07edfe836415ea740b263a4dcc05e8db736459
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994004"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="b7b58-103">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="b7b58-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="b7b58-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7b58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b58-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7b58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b58-106">列出[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7b58-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7b58-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7b58-107">Prerequisites</span></span>
<span data-ttu-id="b7b58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7b58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7b58-110">Permission type</span></span>|<span data-ttu-id="b7b58-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7b58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7b58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7b58-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7b58-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b7b58-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7b58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7b58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b58-115">Not supported.</span></span>|
|<span data-ttu-id="b7b58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7b58-116">Application</span></span>|<span data-ttu-id="b7b58-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7b58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7b58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7b58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="b7b58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7b58-119">Request headers</span></span>
|<span data-ttu-id="b7b58-120">标头</span><span class="sxs-lookup"><span data-stu-id="b7b58-120">Header</span></span>|<span data-ttu-id="b7b58-121">值</span><span class="sxs-lookup"><span data-stu-id="b7b58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7b58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7b58-122">Authorization</span></span>|<span data-ttu-id="b7b58-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7b58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7b58-124">接受</span><span class="sxs-lookup"><span data-stu-id="b7b58-124">Accept</span></span>|<span data-ttu-id="b7b58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7b58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b58-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7b58-126">Request body</span></span>
<span data-ttu-id="b7b58-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7b58-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7b58-128">响应</span><span class="sxs-lookup"><span data-stu-id="b7b58-128">Response</span></span>
<span data-ttu-id="b7b58-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b7b58-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b58-130">示例</span><span class="sxs-lookup"><span data-stu-id="b7b58-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7b58-131">请求</span><span class="sxs-lookup"><span data-stu-id="b7b58-131">Request</span></span>
<span data-ttu-id="b7b58-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7b58-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="b7b58-133">响应</span><span class="sxs-lookup"><span data-stu-id="b7b58-133">Response</span></span>
<span data-ttu-id="b7b58-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7b58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```





