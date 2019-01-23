---
title: createGooglePlayWebToken 操作
description: 生成嵌入组件中使用的 web 标记。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 22190ed207a4678a865392afc659a51f096a419c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394710"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="da6fb-103">createGooglePlayWebToken 操作</span><span class="sxs-lookup"><span data-stu-id="da6fb-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="da6fb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="da6fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da6fb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da6fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da6fb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da6fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da6fb-107">生成嵌入组件中使用的 web 标记。</span><span class="sxs-lookup"><span data-stu-id="da6fb-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da6fb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da6fb-108">Prerequisites</span></span>
<span data-ttu-id="da6fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="da6fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da6fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da6fb-111">Permission type</span></span>|<span data-ttu-id="da6fb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da6fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da6fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da6fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da6fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da6fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da6fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da6fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da6fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da6fb-116">Not supported.</span></span>|
|<span data-ttu-id="da6fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da6fb-117">Application</span></span>|<span data-ttu-id="da6fb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="da6fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da6fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da6fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="da6fb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da6fb-120">Request headers</span></span>
|<span data-ttu-id="da6fb-121">标头</span><span class="sxs-lookup"><span data-stu-id="da6fb-121">Header</span></span>|<span data-ttu-id="da6fb-122">值</span><span class="sxs-lookup"><span data-stu-id="da6fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da6fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da6fb-123">Authorization</span></span>|<span data-ttu-id="da6fb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da6fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da6fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da6fb-125">Accept</span></span>|<span data-ttu-id="da6fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da6fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da6fb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da6fb-127">Request body</span></span>
<span data-ttu-id="da6fb-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da6fb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="da6fb-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="da6fb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="da6fb-130">属性</span><span class="sxs-lookup"><span data-stu-id="da6fb-130">Property</span></span>|<span data-ttu-id="da6fb-131">类型</span><span class="sxs-lookup"><span data-stu-id="da6fb-131">Type</span></span>|<span data-ttu-id="da6fb-132">说明</span><span class="sxs-lookup"><span data-stu-id="da6fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da6fb-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="da6fb-133">parentUri</span></span>|<span data-ttu-id="da6fb-134">String</span><span class="sxs-lookup"><span data-stu-id="da6fb-134">String</span></span>|<span data-ttu-id="da6fb-135">承载组件页上的 https 路径。</span><span class="sxs-lookup"><span data-stu-id="da6fb-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="da6fb-136">响应</span><span class="sxs-lookup"><span data-stu-id="da6fb-136">Response</span></span>
<span data-ttu-id="da6fb-137">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="da6fb-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da6fb-138">示例</span><span class="sxs-lookup"><span data-stu-id="da6fb-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="da6fb-139">请求</span><span class="sxs-lookup"><span data-stu-id="da6fb-139">Request</span></span>
<span data-ttu-id="da6fb-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da6fb-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="da6fb-141">响应</span><span class="sxs-lookup"><span data-stu-id="da6fb-141">Response</span></span>
<span data-ttu-id="da6fb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da6fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




