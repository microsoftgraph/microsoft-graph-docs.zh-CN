---
title: sync 操作
description: 从适用于企业应用商店和其他门户启动所有 AutoPilot 注册设备的同步。 如果同步成功，此操作将返回"204 无内容"响应代码。 如果同步正在进行，该操作将返回 409 冲突响应代码。  如果在上一个同步的 10 分钟内调用此同步操作，该操作将返回 429"请求过多"响应代码。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 047d03ac938dabf185173a6fea3e01c8b17e3a9c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158798"
---
# <a name="sync-action"></a><span data-ttu-id="c278a-106">sync 操作</span><span class="sxs-lookup"><span data-stu-id="c278a-106">sync action</span></span>

<span data-ttu-id="c278a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c278a-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c278a-108">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c278a-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c278a-109">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c278a-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c278a-110">从适用于企业应用商店和其他门户启动所有 AutoPilot 注册设备的同步。</span><span class="sxs-lookup"><span data-stu-id="c278a-110">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="c278a-111">如果同步成功，此操作将返回"204 无内容"响应代码。</span><span class="sxs-lookup"><span data-stu-id="c278a-111">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="c278a-112">如果同步正在进行，该操作将返回 409 冲突响应代码。</span><span class="sxs-lookup"><span data-stu-id="c278a-112">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="c278a-113">如果在上一个同步的 10 分钟内调用此同步操作，该操作将返回 429"请求过多"响应代码。</span><span class="sxs-lookup"><span data-stu-id="c278a-113">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c278a-114">先决条件</span><span class="sxs-lookup"><span data-stu-id="c278a-114">Prerequisites</span></span>
<span data-ttu-id="c278a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c278a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c278a-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="c278a-117">Permission type</span></span>|<span data-ttu-id="c278a-118">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c278a-118">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c278a-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c278a-119">Delegated (work or school account)</span></span>|<span data-ttu-id="c278a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c278a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c278a-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c278a-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c278a-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="c278a-122">Not supported.</span></span>|
|<span data-ttu-id="c278a-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="c278a-123">Application</span></span>|<span data-ttu-id="c278a-124">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c278a-124">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c278a-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c278a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="c278a-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c278a-126">Request headers</span></span>
|<span data-ttu-id="c278a-127">标头</span><span class="sxs-lookup"><span data-stu-id="c278a-127">Header</span></span>|<span data-ttu-id="c278a-128">值</span><span class="sxs-lookup"><span data-stu-id="c278a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c278a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c278a-129">Authorization</span></span>|<span data-ttu-id="c278a-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c278a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c278a-131">接受</span><span class="sxs-lookup"><span data-stu-id="c278a-131">Accept</span></span>|<span data-ttu-id="c278a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c278a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c278a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c278a-133">Request body</span></span>
<span data-ttu-id="c278a-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c278a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c278a-135">响应</span><span class="sxs-lookup"><span data-stu-id="c278a-135">Response</span></span>
<span data-ttu-id="c278a-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c278a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c278a-137">示例</span><span class="sxs-lookup"><span data-stu-id="c278a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c278a-138">请求</span><span class="sxs-lookup"><span data-stu-id="c278a-138">Request</span></span>
<span data-ttu-id="c278a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c278a-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="c278a-140">响应</span><span class="sxs-lookup"><span data-stu-id="c278a-140">Response</span></span>
<span data-ttu-id="c278a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c278a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




