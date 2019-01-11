---
title: 'synchronizationJob: validateCredentials'
description: 验证的凭据是在租户中有效。
localization_priority: Normal
ms.openlocfilehash: b78d6f7b3ff197607897fbdce123aa1e7e646afc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834915"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="3c0b4-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="3c0b4-103">synchronizationJob: validateCredentials</span></span>

> <span data-ttu-id="3c0b4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c0b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c0b4-106">验证的凭据是在租户中有效。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-106">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c0b4-107">权限</span><span class="sxs-lookup"><span data-stu-id="3c0b4-107">Permissions</span></span>
<span data-ttu-id="3c0b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c0b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c0b4-110">Permission type</span></span>                        | <span data-ttu-id="3c0b4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c0b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c0b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0b4-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3c0b4-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c0b4-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3c0b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0b4-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3c0b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-115">Not supported.</span></span> |
|<span data-ttu-id="3c0b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c0b4-116">Application</span></span>                            |<span data-ttu-id="3c0b4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="3c0b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c0b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="3c0b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c0b4-119">Request headers</span></span>
| <span data-ttu-id="3c0b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c0b4-120">Name</span></span>       | <span data-ttu-id="3c0b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="3c0b4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3c0b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c0b4-122">Authorization</span></span>  | <span data-ttu-id="3c0b4-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3c0b4-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0b4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c0b4-124">Request body</span></span>
<span data-ttu-id="3c0b4-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c0b4-126">参数</span><span class="sxs-lookup"><span data-stu-id="3c0b4-126">Parameter</span></span>    | <span data-ttu-id="3c0b4-127">类型</span><span class="sxs-lookup"><span data-stu-id="3c0b4-127">Type</span></span>   |<span data-ttu-id="3c0b4-128">Description</span><span class="sxs-lookup"><span data-stu-id="3c0b4-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c0b4-129">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="3c0b4-129">useSavedCredentials</span></span>|<span data-ttu-id="3c0b4-130">布尔</span><span class="sxs-lookup"><span data-stu-id="3c0b4-130">Boolean</span></span>|<span data-ttu-id="3c0b4-131">当`true`、`credentials`将忽略参数并将改为验证以前保存的凭据 （如果有）。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-131">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="3c0b4-132">凭据</span><span class="sxs-lookup"><span data-stu-id="3c0b4-132">credentials</span></span>|<span data-ttu-id="3c0b4-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c0b4-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="3c0b4-134">若要验证的凭据。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-134">Credentials to validate.</span></span> <span data-ttu-id="3c0b4-135">忽略何时`useSavedCredentials`，则参数`true`。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-135">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="3c0b4-136">响应</span><span class="sxs-lookup"><span data-stu-id="3c0b4-136">Response</span></span>
<span data-ttu-id="3c0b4-137">验证是否成功，则此方法返回`204, No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-137">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="3c0b4-138">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c0b4-139">示例</span><span class="sxs-lookup"><span data-stu-id="3c0b4-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c0b4-140">请求</span><span class="sxs-lookup"><span data-stu-id="3c0b4-140">Request</span></span>
<span data-ttu-id="3c0b4-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="3c0b4-142">响应</span><span class="sxs-lookup"><span data-stu-id="3c0b4-142">Response</span></span>
<span data-ttu-id="3c0b4-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c0b4-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
