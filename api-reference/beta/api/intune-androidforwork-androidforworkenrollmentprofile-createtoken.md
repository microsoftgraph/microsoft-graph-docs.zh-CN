---
title: createToken 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5c8ca7dfb2400f3773232df5fbddb60791e834a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254956"
---
# <a name="createtoken-action"></a><span data-ttu-id="2e802-103">createToken 操作</span><span class="sxs-lookup"><span data-stu-id="2e802-103">createToken action</span></span>

<span data-ttu-id="2e802-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e802-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e802-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2e802-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e802-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2e802-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e802-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2e802-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e802-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e802-108">Prerequisites</span></span>
<span data-ttu-id="2e802-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e802-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e802-111">Permission type</span></span>|<span data-ttu-id="2e802-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e802-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e802-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e802-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e802-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e802-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e802-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e802-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e802-116">Not supported.</span></span>|
|<span data-ttu-id="2e802-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e802-117">Application</span></span>|<span data-ttu-id="2e802-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e802-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e802-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e802-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="2e802-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e802-120">Request headers</span></span>
|<span data-ttu-id="2e802-121">标头</span><span class="sxs-lookup"><span data-stu-id="2e802-121">Header</span></span>|<span data-ttu-id="2e802-122">值</span><span class="sxs-lookup"><span data-stu-id="2e802-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e802-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e802-123">Authorization</span></span>|<span data-ttu-id="2e802-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e802-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e802-125">接受</span><span class="sxs-lookup"><span data-stu-id="2e802-125">Accept</span></span>|<span data-ttu-id="2e802-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e802-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e802-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e802-127">Request body</span></span>
<span data-ttu-id="2e802-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e802-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2e802-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2e802-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2e802-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e802-130">Property</span></span>|<span data-ttu-id="2e802-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e802-131">Type</span></span>|<span data-ttu-id="2e802-132">描述</span><span class="sxs-lookup"><span data-stu-id="2e802-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e802-133">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="2e802-133">tokenValidityInSeconds</span></span>|<span data-ttu-id="2e802-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2e802-134">Int32</span></span>|<span data-ttu-id="2e802-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2e802-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2e802-136">响应</span><span class="sxs-lookup"><span data-stu-id="2e802-136">Response</span></span>
<span data-ttu-id="2e802-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2e802-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2e802-138">示例</span><span class="sxs-lookup"><span data-stu-id="2e802-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e802-139">请求</span><span class="sxs-lookup"><span data-stu-id="2e802-139">Request</span></span>
<span data-ttu-id="2e802-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e802-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="2e802-141">响应</span><span class="sxs-lookup"><span data-stu-id="2e802-141">Response</span></span>
<span data-ttu-id="2e802-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e802-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




