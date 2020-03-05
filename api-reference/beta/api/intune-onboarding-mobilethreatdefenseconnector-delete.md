---
title: 删除 mobileThreatDefenseConnector
description: 删除 mobileThreatDefenseConnector。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93d0972884e7584f8f9c014ea4bcd674f4f9c38a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461961"
---
# <a name="delete-mobilethreatdefenseconnector"></a><span data-ttu-id="48fc4-103">删除 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="48fc4-103">Delete mobileThreatDefenseConnector</span></span>

<span data-ttu-id="48fc4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="48fc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48fc4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="48fc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48fc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48fc4-107">删除 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="48fc4-107">Deletes a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48fc4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="48fc4-108">Prerequisites</span></span>
<span data-ttu-id="48fc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48fc4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48fc4-111">Permission type</span></span>|<span data-ttu-id="48fc4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48fc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48fc4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48fc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48fc4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48fc4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="48fc4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48fc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48fc4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48fc4-116">Not supported.</span></span>|
|<span data-ttu-id="48fc4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48fc4-117">Application</span></span>|<span data-ttu-id="48fc4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48fc4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48fc4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48fc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="48fc4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48fc4-120">Request headers</span></span>
|<span data-ttu-id="48fc4-121">标头</span><span class="sxs-lookup"><span data-stu-id="48fc4-121">Header</span></span>|<span data-ttu-id="48fc4-122">值</span><span class="sxs-lookup"><span data-stu-id="48fc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48fc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48fc4-123">Authorization</span></span>|<span data-ttu-id="48fc4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48fc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48fc4-125">接受</span><span class="sxs-lookup"><span data-stu-id="48fc4-125">Accept</span></span>|<span data-ttu-id="48fc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48fc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48fc4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48fc4-127">Request body</span></span>
<span data-ttu-id="48fc4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="48fc4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48fc4-129">响应</span><span class="sxs-lookup"><span data-stu-id="48fc4-129">Response</span></span>
<span data-ttu-id="48fc4-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="48fc4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="48fc4-131">示例</span><span class="sxs-lookup"><span data-stu-id="48fc4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="48fc4-132">请求</span><span class="sxs-lookup"><span data-stu-id="48fc4-132">Request</span></span>
<span data-ttu-id="48fc4-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48fc4-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="48fc4-134">响应</span><span class="sxs-lookup"><span data-stu-id="48fc4-134">Response</span></span>
<span data-ttu-id="48fc4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48fc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





