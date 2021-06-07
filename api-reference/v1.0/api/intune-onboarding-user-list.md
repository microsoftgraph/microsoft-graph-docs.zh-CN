---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dcb25811cd9ba56959ec8c203f00d95c7a87f15
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751844"
---
# <a name="list-users"></a><span data-ttu-id="257fb-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="257fb-103">List users</span></span>

<span data-ttu-id="257fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="257fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="257fb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="257fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="257fb-106">列出 [user](../resources/intune-onboarding-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="257fb-106">List properties and relationships of the [user](../resources/intune-onboarding-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="257fb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="257fb-107">Prerequisites</span></span>
<span data-ttu-id="257fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="257fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="257fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="257fb-110">Permission type</span></span>|<span data-ttu-id="257fb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="257fb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="257fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="257fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="257fb-113">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="257fb-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="257fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="257fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="257fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="257fb-115">Not supported.</span></span>|
|<span data-ttu-id="257fb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="257fb-116">Application</span></span>|<span data-ttu-id="257fb-117">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="257fb-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="257fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="257fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="257fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="257fb-119">Request headers</span></span>
|<span data-ttu-id="257fb-120">标头</span><span class="sxs-lookup"><span data-stu-id="257fb-120">Header</span></span>|<span data-ttu-id="257fb-121">值</span><span class="sxs-lookup"><span data-stu-id="257fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="257fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="257fb-122">Authorization</span></span>|<span data-ttu-id="257fb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="257fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="257fb-124">接受</span><span class="sxs-lookup"><span data-stu-id="257fb-124">Accept</span></span>|<span data-ttu-id="257fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="257fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="257fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="257fb-126">Request body</span></span>
<span data-ttu-id="257fb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="257fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="257fb-128">响应</span><span class="sxs-lookup"><span data-stu-id="257fb-128">Response</span></span>
<span data-ttu-id="257fb-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-onboarding-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="257fb-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-onboarding-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="257fb-130">示例</span><span class="sxs-lookup"><span data-stu-id="257fb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="257fb-131">请求</span><span class="sxs-lookup"><span data-stu-id="257fb-131">Request</span></span>
<span data-ttu-id="257fb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="257fb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="257fb-133">响应</span><span class="sxs-lookup"><span data-stu-id="257fb-133">Response</span></span>
<span data-ttu-id="257fb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="257fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
      "deviceEnrollmentLimit": 5
    }
  ]
}
```




