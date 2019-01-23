---
title: sync 操作
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e3b87b9033c4329837da704011153d0a4c496df8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414786"
---
# <a name="sync-action"></a><span data-ttu-id="9de54-103">sync 操作</span><span class="sxs-lookup"><span data-stu-id="9de54-103">sync action</span></span>

> <span data-ttu-id="9de54-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9de54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9de54-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9de54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9de54-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9de54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9de54-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9de54-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9de54-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9de54-108">Prerequisites</span></span>
<span data-ttu-id="9de54-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9de54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9de54-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9de54-111">Permission type</span></span>|<span data-ttu-id="9de54-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9de54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9de54-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9de54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9de54-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9de54-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9de54-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9de54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9de54-116">Not supported.</span></span>|
|<span data-ttu-id="9de54-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9de54-117">Application</span></span>|<span data-ttu-id="9de54-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9de54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9de54-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9de54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="9de54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9de54-120">Request headers</span></span>
|<span data-ttu-id="9de54-121">标头</span><span class="sxs-lookup"><span data-stu-id="9de54-121">Header</span></span>|<span data-ttu-id="9de54-122">值</span><span class="sxs-lookup"><span data-stu-id="9de54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9de54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9de54-123">Authorization</span></span>|<span data-ttu-id="9de54-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9de54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9de54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9de54-125">Accept</span></span>|<span data-ttu-id="9de54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9de54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9de54-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9de54-127">Request body</span></span>
<span data-ttu-id="9de54-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9de54-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9de54-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9de54-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9de54-130">属性</span><span class="sxs-lookup"><span data-stu-id="9de54-130">Property</span></span>|<span data-ttu-id="9de54-131">类型</span><span class="sxs-lookup"><span data-stu-id="9de54-131">Type</span></span>|<span data-ttu-id="9de54-132">说明</span><span class="sxs-lookup"><span data-stu-id="9de54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9de54-133">syncType</span><span class="sxs-lookup"><span data-stu-id="9de54-133">syncType</span></span>|[<span data-ttu-id="9de54-134">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="9de54-134">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="9de54-135">将执行的同步类型，完全同步或增量同步。</span><span class="sxs-lookup"><span data-stu-id="9de54-135">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="9de54-136">响应</span><span class="sxs-lookup"><span data-stu-id="9de54-136">Response</span></span>
<span data-ttu-id="9de54-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9de54-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9de54-138">示例</span><span class="sxs-lookup"><span data-stu-id="9de54-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de54-139">请求</span><span class="sxs-lookup"><span data-stu-id="9de54-139">Request</span></span>
<span data-ttu-id="9de54-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9de54-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="9de54-141">响应</span><span class="sxs-lookup"><span data-stu-id="9de54-141">Response</span></span>
<span data-ttu-id="9de54-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9de54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




