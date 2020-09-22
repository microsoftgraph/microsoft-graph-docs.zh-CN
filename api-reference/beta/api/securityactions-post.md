---
title: 创建 securityAction
description: 创建新的 securityAction 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 098348a8bd8793765d5fa9dfb7bd8ba7502c7eda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044765"
---
# <a name="create-securityaction"></a><span data-ttu-id="f3170-103">创建 securityAction</span><span class="sxs-lookup"><span data-stu-id="f3170-103">Create securityAction</span></span>

<span data-ttu-id="f3170-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3170-105">创建新的 [securityAction](../resources/securityaction.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3170-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3170-106">权限</span><span class="sxs-lookup"><span data-stu-id="f3170-106">Permissions</span></span>

<span data-ttu-id="f3170-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f3170-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3170-109">Permission type</span></span>                        | <span data-ttu-id="f3170-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3170-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f3170-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3170-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3170-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3170-112">Not supported.</span></span> |
| <span data-ttu-id="f3170-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3170-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3170-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3170-114">Not supported.</span></span> |
| <span data-ttu-id="f3170-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3170-115">Application</span></span>                            | <span data-ttu-id="f3170-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3170-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3170-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3170-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="f3170-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3170-118">Request headers</span></span>

| <span data-ttu-id="f3170-119">名称</span><span class="sxs-lookup"><span data-stu-id="f3170-119">Name</span></span>          | <span data-ttu-id="f3170-120">说明</span><span class="sxs-lookup"><span data-stu-id="f3170-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f3170-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3170-121">Authorization</span></span> | <span data-ttu-id="f3170-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f3170-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3170-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3170-123">Request body</span></span>

<span data-ttu-id="f3170-124">在请求正文中，提供 [securityAction](../resources/securityaction.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3170-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3170-125">响应</span><span class="sxs-lookup"><span data-stu-id="f3170-125">Response</span></span>

<span data-ttu-id="f3170-126">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [securityAction](../resources/securityaction.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3170-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f3170-127">示例</span><span class="sxs-lookup"><span data-stu-id="f3170-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f3170-128">请求</span><span class="sxs-lookup"><span data-stu-id="f3170-128">Request</span></span>

<span data-ttu-id="f3170-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f3170-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3170-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3170-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f3170-131">C#</span><span class="sxs-lookup"><span data-stu-id="f3170-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3170-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3170-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3170-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3170-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3170-134">响应</span><span class="sxs-lookup"><span data-stu-id="f3170-134">Response</span></span>

<span data-ttu-id="f3170-135">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="f3170-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f3170-136">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f3170-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f3170-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f3170-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


