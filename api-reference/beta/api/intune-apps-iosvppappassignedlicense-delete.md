---
title: 删除 iosVppAppAssignedLicense
description: 删除 iosVppAppAssignedLicense。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39a3200354399b8430662e10768a83b41c1b4db6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936173"
---
# <a name="delete-iosvppappassignedlicense"></a><span data-ttu-id="25389-103">删除 iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="25389-103">Delete iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="25389-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25389-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25389-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25389-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25389-106">删除[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)。</span><span class="sxs-lookup"><span data-stu-id="25389-106">Deletes a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25389-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="25389-107">Prerequisites</span></span>
<span data-ttu-id="25389-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25389-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25389-110">Permission type</span></span>|<span data-ttu-id="25389-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25389-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25389-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25389-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25389-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25389-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25389-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25389-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25389-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25389-115">Not supported.</span></span>|
|<span data-ttu-id="25389-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25389-116">Application</span></span>|<span data-ttu-id="25389-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25389-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25389-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25389-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="25389-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25389-119">Request headers</span></span>
|<span data-ttu-id="25389-120">标头</span><span class="sxs-lookup"><span data-stu-id="25389-120">Header</span></span>|<span data-ttu-id="25389-121">值</span><span class="sxs-lookup"><span data-stu-id="25389-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25389-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25389-122">Authorization</span></span>|<span data-ttu-id="25389-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25389-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25389-124">接受</span><span class="sxs-lookup"><span data-stu-id="25389-124">Accept</span></span>|<span data-ttu-id="25389-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25389-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25389-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="25389-126">Request body</span></span>
<span data-ttu-id="25389-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25389-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25389-128">响应</span><span class="sxs-lookup"><span data-stu-id="25389-128">Response</span></span>
<span data-ttu-id="25389-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25389-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="25389-130">示例</span><span class="sxs-lookup"><span data-stu-id="25389-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="25389-131">请求</span><span class="sxs-lookup"><span data-stu-id="25389-131">Request</span></span>
<span data-ttu-id="25389-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25389-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="25389-133">响应</span><span class="sxs-lookup"><span data-stu-id="25389-133">Response</span></span>
<span data-ttu-id="25389-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25389-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




