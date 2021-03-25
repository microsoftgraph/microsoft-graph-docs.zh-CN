---
title: sync 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b349998eb1ece4fdb5544420d5ea29305c86519
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158757"
---
# <a name="sync-action"></a><span data-ttu-id="2cbc3-103">sync 操作</span><span class="sxs-lookup"><span data-stu-id="2cbc3-103">sync action</span></span>

<span data-ttu-id="2cbc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cbc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cbc3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cbc3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cbc3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2cbc3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cbc3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2cbc3-108">Prerequisites</span></span>
<span data-ttu-id="2cbc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cbc3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cbc3-111">Permission type</span></span>|<span data-ttu-id="2cbc3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cbc3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cbc3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cbc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cbc3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cbc3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2cbc3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cbc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cbc3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-116">Not supported.</span></span>|
|<span data-ttu-id="2cbc3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cbc3-117">Application</span></span>|<span data-ttu-id="2cbc3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cbc3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cbc3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cbc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="2cbc3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cbc3-120">Request headers</span></span>
|<span data-ttu-id="2cbc3-121">标头</span><span class="sxs-lookup"><span data-stu-id="2cbc3-121">Header</span></span>|<span data-ttu-id="2cbc3-122">值</span><span class="sxs-lookup"><span data-stu-id="2cbc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cbc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cbc3-123">Authorization</span></span>|<span data-ttu-id="2cbc3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cbc3-125">接受</span><span class="sxs-lookup"><span data-stu-id="2cbc3-125">Accept</span></span>|<span data-ttu-id="2cbc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cbc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cbc3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cbc3-127">Request body</span></span>
<span data-ttu-id="2cbc3-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2cbc3-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2cbc3-130">属性</span><span class="sxs-lookup"><span data-stu-id="2cbc3-130">Property</span></span>|<span data-ttu-id="2cbc3-131">类型</span><span class="sxs-lookup"><span data-stu-id="2cbc3-131">Type</span></span>|<span data-ttu-id="2cbc3-132">说明</span><span class="sxs-lookup"><span data-stu-id="2cbc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cbc3-133">syncType</span><span class="sxs-lookup"><span data-stu-id="2cbc3-133">syncType</span></span>|[<span data-ttu-id="2cbc3-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="2cbc3-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="2cbc3-135">将执行的同步类型，完全同步或增量同步。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="2cbc3-136">响应</span><span class="sxs-lookup"><span data-stu-id="2cbc3-136">Response</span></span>
<span data-ttu-id="2cbc3-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cbc3-138">示例</span><span class="sxs-lookup"><span data-stu-id="2cbc3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cbc3-139">请求</span><span class="sxs-lookup"><span data-stu-id="2cbc3-139">Request</span></span>
<span data-ttu-id="2cbc3-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="2cbc3-141">响应</span><span class="sxs-lookup"><span data-stu-id="2cbc3-141">Response</span></span>
<span data-ttu-id="2cbc3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2cbc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




