---
title: 'synchronizationJob: validateCredentials'
description: 验证的凭据是在租户中有效。
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519001"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="38ad8-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="38ad8-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38ad8-104">验证的凭据是在租户中有效。</span><span class="sxs-lookup"><span data-stu-id="38ad8-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="38ad8-105">权限</span><span class="sxs-lookup"><span data-stu-id="38ad8-105">Permissions</span></span>
<span data-ttu-id="38ad8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38ad8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="38ad8-108">Permission type</span></span>                        | <span data-ttu-id="38ad8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38ad8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38ad8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38ad8-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="38ad8-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ad8-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="38ad8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38ad8-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="38ad8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="38ad8-113">Not supported.</span></span> |
|<span data-ttu-id="38ad8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="38ad8-114">Application</span></span>                            |<span data-ttu-id="38ad8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38ad8-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="38ad8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38ad8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="38ad8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="38ad8-117">Request headers</span></span>
| <span data-ttu-id="38ad8-118">名称</span><span class="sxs-lookup"><span data-stu-id="38ad8-118">Name</span></span>       | <span data-ttu-id="38ad8-119">说明</span><span class="sxs-lookup"><span data-stu-id="38ad8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38ad8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ad8-120">Authorization</span></span>  | <span data-ttu-id="38ad8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="38ad8-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="38ad8-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="38ad8-122">Request body</span></span>
<span data-ttu-id="38ad8-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="38ad8-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38ad8-124">参数</span><span class="sxs-lookup"><span data-stu-id="38ad8-124">Parameter</span></span>    | <span data-ttu-id="38ad8-125">类型</span><span class="sxs-lookup"><span data-stu-id="38ad8-125">Type</span></span>   |<span data-ttu-id="38ad8-126">说明</span><span class="sxs-lookup"><span data-stu-id="38ad8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38ad8-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="38ad8-127">useSavedCredentials</span></span>|<span data-ttu-id="38ad8-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="38ad8-128">Boolean</span></span>|<span data-ttu-id="38ad8-129">当`true`、`credentials`将忽略参数并将改为验证以前保存的凭据 （如果有）。</span><span class="sxs-lookup"><span data-stu-id="38ad8-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="38ad8-130">凭据</span><span class="sxs-lookup"><span data-stu-id="38ad8-130">credentials</span></span>|<span data-ttu-id="38ad8-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="38ad8-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="38ad8-132">若要验证的凭据。</span><span class="sxs-lookup"><span data-stu-id="38ad8-132">Credentials to validate.</span></span> <span data-ttu-id="38ad8-133">忽略何时`useSavedCredentials`，则参数`true`。</span><span class="sxs-lookup"><span data-stu-id="38ad8-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="38ad8-134">响应</span><span class="sxs-lookup"><span data-stu-id="38ad8-134">Response</span></span>
<span data-ttu-id="38ad8-135">验证是否成功，则此方法返回`204, No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="38ad8-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="38ad8-136">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="38ad8-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38ad8-137">示例</span><span class="sxs-lookup"><span data-stu-id="38ad8-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38ad8-138">请求</span><span class="sxs-lookup"><span data-stu-id="38ad8-138">Request</span></span>
<span data-ttu-id="38ad8-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38ad8-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="38ad8-140">响应</span><span class="sxs-lookup"><span data-stu-id="38ad8-140">Response</span></span>
<span data-ttu-id="38ad8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38ad8-141">The following is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
