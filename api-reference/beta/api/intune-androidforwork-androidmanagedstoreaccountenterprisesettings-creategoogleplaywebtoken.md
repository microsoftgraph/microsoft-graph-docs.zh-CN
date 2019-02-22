---
title: createGooglePlayWebToken 操作
description: 生成在可嵌入组件中使用的 web 令牌。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50355af2e5f9e593501094c0bfd1638cb070df9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141242"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="c8810-103">createGooglePlayWebToken 操作</span><span class="sxs-lookup"><span data-stu-id="c8810-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="c8810-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8810-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8810-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8810-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8810-106">生成在可嵌入组件中使用的 web 令牌。</span><span class="sxs-lookup"><span data-stu-id="c8810-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8810-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8810-107">Prerequisites</span></span>
<span data-ttu-id="c8810-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c8810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8810-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8810-110">Permission type</span></span>|<span data-ttu-id="c8810-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8810-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8810-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8810-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8810-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8810-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8810-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8810-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8810-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8810-115">Not supported.</span></span>|
|<span data-ttu-id="c8810-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8810-116">Application</span></span>|<span data-ttu-id="c8810-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8810-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8810-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8810-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="c8810-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8810-119">Request headers</span></span>
|<span data-ttu-id="c8810-120">标头</span><span class="sxs-lookup"><span data-stu-id="c8810-120">Header</span></span>|<span data-ttu-id="c8810-121">值</span><span class="sxs-lookup"><span data-stu-id="c8810-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8810-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8810-122">Authorization</span></span>|<span data-ttu-id="c8810-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8810-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8810-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c8810-124">Accept</span></span>|<span data-ttu-id="c8810-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8810-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8810-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8810-126">Request body</span></span>
<span data-ttu-id="c8810-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8810-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c8810-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c8810-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c8810-129">属性</span><span class="sxs-lookup"><span data-stu-id="c8810-129">Property</span></span>|<span data-ttu-id="c8810-130">类型</span><span class="sxs-lookup"><span data-stu-id="c8810-130">Type</span></span>|<span data-ttu-id="c8810-131">说明</span><span class="sxs-lookup"><span data-stu-id="c8810-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8810-132">parentUri</span><span class="sxs-lookup"><span data-stu-id="c8810-132">parentUri</span></span>|<span data-ttu-id="c8810-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c8810-133">String</span></span>|<span data-ttu-id="c8810-134">承载组件的页面的 https 路径。</span><span class="sxs-lookup"><span data-stu-id="c8810-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="c8810-135">响应</span><span class="sxs-lookup"><span data-stu-id="c8810-135">Response</span></span>
<span data-ttu-id="c8810-136">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="c8810-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8810-137">示例</span><span class="sxs-lookup"><span data-stu-id="c8810-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8810-138">请求</span><span class="sxs-lookup"><span data-stu-id="c8810-138">Request</span></span>
<span data-ttu-id="c8810-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8810-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="c8810-140">响应</span><span class="sxs-lookup"><span data-stu-id="c8810-140">Response</span></span>
<span data-ttu-id="c8810-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8810-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




