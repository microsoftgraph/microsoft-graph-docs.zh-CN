---
title: 删除 mobileThreatDefenseConnector
description: 删除 mobileThreatDefenseConnector。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6d817fc80606ce09a2da457dfdb339f28b4ac1e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757987"
---
# <a name="delete-mobilethreatdefenseconnector"></a><span data-ttu-id="0a7cc-103">删除 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="0a7cc-103">Delete mobileThreatDefenseConnector</span></span>

<span data-ttu-id="0a7cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a7cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a7cc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a7cc-106">删除 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-106">Deletes a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a7cc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a7cc-107">Prerequisites</span></span>
<span data-ttu-id="0a7cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a7cc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a7cc-110">Permission type</span></span>|<span data-ttu-id="0a7cc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a7cc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a7cc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a7cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a7cc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a7cc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a7cc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a7cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a7cc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-115">Not supported.</span></span>|
|<span data-ttu-id="0a7cc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a7cc-116">Application</span></span>|<span data-ttu-id="0a7cc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a7cc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a7cc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a7cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="0a7cc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a7cc-119">Request headers</span></span>
|<span data-ttu-id="0a7cc-120">标头</span><span class="sxs-lookup"><span data-stu-id="0a7cc-120">Header</span></span>|<span data-ttu-id="0a7cc-121">值</span><span class="sxs-lookup"><span data-stu-id="0a7cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a7cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a7cc-122">Authorization</span></span>|<span data-ttu-id="0a7cc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a7cc-124">接受</span><span class="sxs-lookup"><span data-stu-id="0a7cc-124">Accept</span></span>|<span data-ttu-id="0a7cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a7cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a7cc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a7cc-126">Request body</span></span>
<span data-ttu-id="0a7cc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a7cc-128">响应</span><span class="sxs-lookup"><span data-stu-id="0a7cc-128">Response</span></span>
<span data-ttu-id="0a7cc-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a7cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="0a7cc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a7cc-131">请求</span><span class="sxs-lookup"><span data-stu-id="0a7cc-131">Request</span></span>
<span data-ttu-id="0a7cc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="0a7cc-133">响应</span><span class="sxs-lookup"><span data-stu-id="0a7cc-133">Response</span></span>
<span data-ttu-id="0a7cc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a7cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




