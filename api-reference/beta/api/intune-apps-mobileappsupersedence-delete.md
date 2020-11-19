---
title: 删除 mobileAppSupersedence
description: 删除 mobileAppSupersedence。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2c72cf2984b660ff99395d5314b4b68a3fae166
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247977"
---
# <a name="delete-mobileappsupersedence"></a><span data-ttu-id="04459-103">删除 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="04459-103">Delete mobileAppSupersedence</span></span>

<span data-ttu-id="04459-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04459-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04459-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04459-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04459-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04459-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04459-107">删除 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)。</span><span class="sxs-lookup"><span data-stu-id="04459-107">Deletes a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04459-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="04459-108">Prerequisites</span></span>
<span data-ttu-id="04459-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04459-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04459-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="04459-111">Permission type</span></span>|<span data-ttu-id="04459-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04459-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04459-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04459-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04459-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04459-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04459-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04459-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04459-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04459-116">Not supported.</span></span>|
|<span data-ttu-id="04459-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="04459-117">Application</span></span>|<span data-ttu-id="04459-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04459-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04459-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04459-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="04459-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="04459-120">Request headers</span></span>
|<span data-ttu-id="04459-121">标头</span><span class="sxs-lookup"><span data-stu-id="04459-121">Header</span></span>|<span data-ttu-id="04459-122">值</span><span class="sxs-lookup"><span data-stu-id="04459-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04459-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04459-123">Authorization</span></span>|<span data-ttu-id="04459-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04459-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04459-125">接受</span><span class="sxs-lookup"><span data-stu-id="04459-125">Accept</span></span>|<span data-ttu-id="04459-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04459-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04459-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04459-127">Request body</span></span>
<span data-ttu-id="04459-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04459-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04459-129">响应</span><span class="sxs-lookup"><span data-stu-id="04459-129">Response</span></span>
<span data-ttu-id="04459-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="04459-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04459-131">示例</span><span class="sxs-lookup"><span data-stu-id="04459-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="04459-132">请求</span><span class="sxs-lookup"><span data-stu-id="04459-132">Request</span></span>
<span data-ttu-id="04459-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04459-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="04459-134">响应</span><span class="sxs-lookup"><span data-stu-id="04459-134">Response</span></span>
<span data-ttu-id="04459-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04459-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




