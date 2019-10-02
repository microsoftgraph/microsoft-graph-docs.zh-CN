---
title: 列出 organizations
description: 列出 organization 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9edd123dc9c71a6da742e4acaf76c2ad271187a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362153"
---
# <a name="list-organizations"></a><span data-ttu-id="9f719-103">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="9f719-103">List organizations</span></span>

> <span data-ttu-id="9f719-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f719-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f719-105">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9f719-105">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f719-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f719-106">Prerequisites</span></span>
<span data-ttu-id="9f719-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f719-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f719-109">Permission type</span></span>|<span data-ttu-id="9f719-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f719-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f719-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f719-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f719-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f719-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9f719-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f719-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f719-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f719-114">Not supported.</span></span>|
|<span data-ttu-id="9f719-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f719-115">Application</span></span>|<span data-ttu-id="9f719-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f719-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f719-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f719-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="9f719-118">请求头</span><span class="sxs-lookup"><span data-stu-id="9f719-118">Request headers</span></span>
|<span data-ttu-id="9f719-119">标头</span><span class="sxs-lookup"><span data-stu-id="9f719-119">Header</span></span>|<span data-ttu-id="9f719-120">值</span><span class="sxs-lookup"><span data-stu-id="9f719-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f719-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f719-121">Authorization</span></span>|<span data-ttu-id="9f719-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f719-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f719-123">接受</span><span class="sxs-lookup"><span data-stu-id="9f719-123">Accept</span></span>|<span data-ttu-id="9f719-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9f719-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f719-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f719-125">Request body</span></span>
<span data-ttu-id="9f719-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f719-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f719-127">响应</span><span class="sxs-lookup"><span data-stu-id="9f719-127">Response</span></span>
<span data-ttu-id="9f719-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/intune-onboarding-organization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9f719-128">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f719-129">示例</span><span class="sxs-lookup"><span data-stu-id="9f719-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f719-130">请求</span><span class="sxs-lookup"><span data-stu-id="9f719-130">Request</span></span>
<span data-ttu-id="9f719-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f719-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="9f719-132">响应</span><span class="sxs-lookup"><span data-stu-id="9f719-132">Response</span></span>
<span data-ttu-id="9f719-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f719-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```




