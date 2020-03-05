---
title: 创建 securityAction
description: 创建新的 securityAction 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ea1d95e1ff9380919d3d4afd2877cab2e370eae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453546"
---
# <a name="create-securityaction"></a><span data-ttu-id="47e2a-103">创建 securityAction</span><span class="sxs-lookup"><span data-stu-id="47e2a-103">Create securityAction</span></span>

<span data-ttu-id="47e2a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="47e2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47e2a-105">创建新的[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47e2a-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47e2a-106">权限</span><span class="sxs-lookup"><span data-stu-id="47e2a-106">Permissions</span></span>

<span data-ttu-id="47e2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47e2a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47e2a-109">Permission type</span></span>                        | <span data-ttu-id="47e2a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47e2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47e2a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47e2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47e2a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="47e2a-112">Not supported.</span></span> |
| <span data-ttu-id="47e2a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47e2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e2a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47e2a-114">Not supported.</span></span> |
| <span data-ttu-id="47e2a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47e2a-115">Application</span></span>                            | <span data-ttu-id="47e2a-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e2a-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47e2a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47e2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="47e2a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="47e2a-118">Request headers</span></span>

| <span data-ttu-id="47e2a-119">名称</span><span class="sxs-lookup"><span data-stu-id="47e2a-119">Name</span></span>          | <span data-ttu-id="47e2a-120">说明</span><span class="sxs-lookup"><span data-stu-id="47e2a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="47e2a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47e2a-121">Authorization</span></span> | <span data-ttu-id="47e2a-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="47e2a-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="47e2a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="47e2a-123">Request body</span></span>

<span data-ttu-id="47e2a-124">在请求正文中，提供[securityAction](../resources/securityaction.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e2a-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="47e2a-125">响应</span><span class="sxs-lookup"><span data-stu-id="47e2a-125">Response</span></span>

<span data-ttu-id="47e2a-126">如果成功，此方法在`201 Created`响应正文中返回响应代码和[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47e2a-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47e2a-127">示例</span><span class="sxs-lookup"><span data-stu-id="47e2a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47e2a-128">请求</span><span class="sxs-lookup"><span data-stu-id="47e2a-128">Request</span></span>

<span data-ttu-id="47e2a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47e2a-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47e2a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="47e2a-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="47e2a-131">C#</span><span class="sxs-lookup"><span data-stu-id="47e2a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47e2a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47e2a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47e2a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47e2a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47e2a-134">响应</span><span class="sxs-lookup"><span data-stu-id="47e2a-134">Response</span></span>

<span data-ttu-id="47e2a-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="47e2a-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="47e2a-136">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="47e2a-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="47e2a-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="47e2a-137">All the properties will be returned from an actual call.</span></span>

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
