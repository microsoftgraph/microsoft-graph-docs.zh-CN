---
title: 列出 iosVppAppAssignedUserLicenses
description: 列出 iosVppAppAssignedUserLicense 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a11366ad6582cdd4c0a686a0c4fa4566daa99a3e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804975"
---
# <a name="list-iosvppappassigneduserlicenses"></a><span data-ttu-id="03397-103">列出 iosVppAppAssignedUserLicenses</span><span class="sxs-lookup"><span data-stu-id="03397-103">List iosVppAppAssignedUserLicenses</span></span>

> <span data-ttu-id="03397-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03397-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03397-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03397-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03397-106">列出[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03397-106">List properties and relationships of the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03397-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="03397-107">Prerequisites</span></span>
<span data-ttu-id="03397-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03397-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03397-110">Permission type</span></span>|<span data-ttu-id="03397-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03397-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03397-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03397-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03397-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03397-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="03397-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03397-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03397-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03397-115">Not supported.</span></span>|
|<span data-ttu-id="03397-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03397-116">Application</span></span>|<span data-ttu-id="03397-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="03397-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03397-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03397-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="03397-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="03397-119">Request headers</span></span>
|<span data-ttu-id="03397-120">标头</span><span class="sxs-lookup"><span data-stu-id="03397-120">Header</span></span>|<span data-ttu-id="03397-121">值</span><span class="sxs-lookup"><span data-stu-id="03397-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03397-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03397-122">Authorization</span></span>|<span data-ttu-id="03397-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03397-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03397-124">接受</span><span class="sxs-lookup"><span data-stu-id="03397-124">Accept</span></span>|<span data-ttu-id="03397-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03397-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03397-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="03397-126">Request body</span></span>
<span data-ttu-id="03397-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03397-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03397-128">响应</span><span class="sxs-lookup"><span data-stu-id="03397-128">Response</span></span>
<span data-ttu-id="03397-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="03397-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03397-130">示例</span><span class="sxs-lookup"><span data-stu-id="03397-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="03397-131">请求</span><span class="sxs-lookup"><span data-stu-id="03397-131">Request</span></span>
<span data-ttu-id="03397-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03397-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="03397-133">响应</span><span class="sxs-lookup"><span data-stu-id="03397-133">Response</span></span>
<span data-ttu-id="03397-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03397-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
      "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





