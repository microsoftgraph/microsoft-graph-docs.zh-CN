---
title: 删除 embeddedSIMActivationCodePoolAssignment
description: 删除嵌入的SIMActivationCodePoolAssignment。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c694bfe87f2f29a3107b76ec56ee6da2e7776743
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126119"
---
# <a name="delete-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="bae0e-103">删除 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="bae0e-103">Delete embeddedSIMActivationCodePoolAssignment</span></span>

<span data-ttu-id="bae0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bae0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bae0e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bae0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bae0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bae0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bae0e-107">删除嵌入式 [SIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bae0e-107">Deletes a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bae0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bae0e-108">Prerequisites</span></span>
<span data-ttu-id="bae0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bae0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bae0e-111">Permission type</span></span>|<span data-ttu-id="bae0e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bae0e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bae0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bae0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bae0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bae0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bae0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bae0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bae0e-116">Not supported.</span></span>|
|<span data-ttu-id="bae0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bae0e-117">Application</span></span>|<span data-ttu-id="bae0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bae0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bae0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bae0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bae0e-120">Request headers</span></span>
|<span data-ttu-id="bae0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="bae0e-121">Header</span></span>|<span data-ttu-id="bae0e-122">值</span><span class="sxs-lookup"><span data-stu-id="bae0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bae0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae0e-123">Authorization</span></span>|<span data-ttu-id="bae0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bae0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bae0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="bae0e-125">Accept</span></span>|<span data-ttu-id="bae0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bae0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bae0e-127">Request body</span></span>
<span data-ttu-id="bae0e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bae0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bae0e-129">响应</span><span class="sxs-lookup"><span data-stu-id="bae0e-129">Response</span></span>
<span data-ttu-id="bae0e-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bae0e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bae0e-131">示例</span><span class="sxs-lookup"><span data-stu-id="bae0e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae0e-132">请求</span><span class="sxs-lookup"><span data-stu-id="bae0e-132">Request</span></span>
<span data-ttu-id="bae0e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bae0e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bae0e-134">响应</span><span class="sxs-lookup"><span data-stu-id="bae0e-134">Response</span></span>
<span data-ttu-id="bae0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bae0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




