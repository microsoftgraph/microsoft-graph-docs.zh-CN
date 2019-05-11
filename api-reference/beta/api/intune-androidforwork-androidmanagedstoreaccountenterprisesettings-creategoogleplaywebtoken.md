---
title: createGooglePlayWebToken 操作
description: 生成在可嵌入组件中使用的 web 令牌。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 520a8ce4e54a43fc84a28440930a093863599ceb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939124"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="b7793-103">createGooglePlayWebToken 操作</span><span class="sxs-lookup"><span data-stu-id="b7793-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="b7793-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7793-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7793-106">生成在可嵌入组件中使用的 web 令牌。</span><span class="sxs-lookup"><span data-stu-id="b7793-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7793-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7793-107">Prerequisites</span></span>
<span data-ttu-id="b7793-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7793-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7793-110">Permission type</span></span>|<span data-ttu-id="b7793-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7793-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7793-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7793-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7793-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7793-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7793-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7793-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7793-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7793-115">Not supported.</span></span>|
|<span data-ttu-id="b7793-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7793-116">Application</span></span>|<span data-ttu-id="b7793-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7793-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7793-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7793-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="b7793-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7793-119">Request headers</span></span>
|<span data-ttu-id="b7793-120">标头</span><span class="sxs-lookup"><span data-stu-id="b7793-120">Header</span></span>|<span data-ttu-id="b7793-121">值</span><span class="sxs-lookup"><span data-stu-id="b7793-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7793-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7793-122">Authorization</span></span>|<span data-ttu-id="b7793-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7793-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7793-124">接受</span><span class="sxs-lookup"><span data-stu-id="b7793-124">Accept</span></span>|<span data-ttu-id="b7793-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7793-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7793-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7793-126">Request body</span></span>
<span data-ttu-id="b7793-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7793-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b7793-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b7793-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b7793-129">属性</span><span class="sxs-lookup"><span data-stu-id="b7793-129">Property</span></span>|<span data-ttu-id="b7793-130">类型</span><span class="sxs-lookup"><span data-stu-id="b7793-130">Type</span></span>|<span data-ttu-id="b7793-131">说明</span><span class="sxs-lookup"><span data-stu-id="b7793-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7793-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="b7793-132">parentUri</span></span>|<span data-ttu-id="b7793-133">String</span><span class="sxs-lookup"><span data-stu-id="b7793-133">String</span></span>|<span data-ttu-id="b7793-134">承载组件的页面的 https 路径。</span><span class="sxs-lookup"><span data-stu-id="b7793-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="b7793-135">响应</span><span class="sxs-lookup"><span data-stu-id="b7793-135">Response</span></span>
<span data-ttu-id="b7793-136">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="b7793-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7793-137">示例</span><span class="sxs-lookup"><span data-stu-id="b7793-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7793-138">请求</span><span class="sxs-lookup"><span data-stu-id="b7793-138">Request</span></span>
<span data-ttu-id="b7793-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7793-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="b7793-140">响应</span><span class="sxs-lookup"><span data-stu-id="b7793-140">Response</span></span>
<span data-ttu-id="b7793-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7793-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




