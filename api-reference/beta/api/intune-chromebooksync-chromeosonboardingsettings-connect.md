---
title: connect 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8acaa40e29e76dfd0d71652339664688a0147cf6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665721"
---
# <a name="connect-action"></a><span data-ttu-id="9a76b-103">connect 操作</span><span class="sxs-lookup"><span data-stu-id="9a76b-103">connect action</span></span>

<span data-ttu-id="9a76b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a76b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a76b-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a76b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a76b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a76b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a76b-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9a76b-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a76b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a76b-108">Prerequisites</span></span>
<span data-ttu-id="9a76b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a76b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a76b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a76b-111">Permission type</span></span>|<span data-ttu-id="9a76b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a76b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a76b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a76b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a76b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a76b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a76b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a76b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a76b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a76b-116">Not supported.</span></span>|
|<span data-ttu-id="9a76b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a76b-117">Application</span></span>|<span data-ttu-id="9a76b-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a76b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a76b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a76b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/chromeOSOnboardingSettings/connect
```

## <a name="request-headers"></a><span data-ttu-id="9a76b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a76b-120">Request headers</span></span>
|<span data-ttu-id="9a76b-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a76b-121">Header</span></span>|<span data-ttu-id="9a76b-122">值</span><span class="sxs-lookup"><span data-stu-id="9a76b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a76b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a76b-123">Authorization</span></span>|<span data-ttu-id="9a76b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a76b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a76b-125">接受</span><span class="sxs-lookup"><span data-stu-id="9a76b-125">Accept</span></span>|<span data-ttu-id="9a76b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a76b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a76b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a76b-127">Request body</span></span>
<span data-ttu-id="9a76b-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a76b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9a76b-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9a76b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9a76b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a76b-130">Property</span></span>|<span data-ttu-id="9a76b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a76b-131">Type</span></span>|<span data-ttu-id="9a76b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a76b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a76b-133">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a76b-133">ownerUserPrincipalName</span></span>|<span data-ttu-id="9a76b-134">String</span><span class="sxs-lookup"><span data-stu-id="9a76b-134">String</span></span>|<span data-ttu-id="9a76b-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9a76b-135">Not yet documented</span></span>|
|<span data-ttu-id="9a76b-136">serviceAccountCredentials</span><span class="sxs-lookup"><span data-stu-id="9a76b-136">serviceAccountCredentials</span></span>|<span data-ttu-id="9a76b-137">String</span><span class="sxs-lookup"><span data-stu-id="9a76b-137">String</span></span>|<span data-ttu-id="9a76b-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9a76b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9a76b-139">响应</span><span class="sxs-lookup"><span data-stu-id="9a76b-139">Response</span></span>
<span data-ttu-id="9a76b-140">如果成功，此操作在响应 `200 OK` 正文中返回 响应[代码和 chromeOSOnboardingStatus。](../resources/intune-chromebooksync-chromeosonboardingstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9a76b-140">If successful, this action returns a `200 OK` response code and a [chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a76b-141">示例</span><span class="sxs-lookup"><span data-stu-id="9a76b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a76b-142">请求</span><span class="sxs-lookup"><span data-stu-id="9a76b-142">Request</span></span>
<span data-ttu-id="9a76b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a76b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings/connect

Content-type: application/json
Content-length: 136

{
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "serviceAccountCredentials": "Service Account Credentials value"
}
```

### <a name="response"></a><span data-ttu-id="9a76b-144">响应</span><span class="sxs-lookup"><span data-stu-id="9a76b-144">Response</span></span>
<span data-ttu-id="9a76b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a76b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 29

{
  "value": "inprogress"
}
```




