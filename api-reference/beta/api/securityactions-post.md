---
title: 创建 securityAction
description: 创建新的 securityAction 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 97eb08d27388d1396c203bd0309f80d5f3e941ff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364122"
---
# <a name="create-securityaction"></a><span data-ttu-id="41284-103">创建 securityAction</span><span class="sxs-lookup"><span data-stu-id="41284-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41284-104">创建新的[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41284-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41284-105">权限</span><span class="sxs-lookup"><span data-stu-id="41284-105">Permissions</span></span>

<span data-ttu-id="41284-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41284-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="41284-108">Permission type</span></span>                        | <span data-ttu-id="41284-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41284-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41284-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41284-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41284-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="41284-111">Not supported.</span></span> |
| <span data-ttu-id="41284-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41284-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41284-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="41284-113">Not supported.</span></span> |
| <span data-ttu-id="41284-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="41284-114">Application</span></span>                            | <span data-ttu-id="41284-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41284-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41284-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41284-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="41284-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="41284-117">Request headers</span></span>

| <span data-ttu-id="41284-118">名称</span><span class="sxs-lookup"><span data-stu-id="41284-118">Name</span></span>          | <span data-ttu-id="41284-119">说明</span><span class="sxs-lookup"><span data-stu-id="41284-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="41284-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="41284-120">Authorization</span></span> | <span data-ttu-id="41284-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="41284-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41284-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="41284-122">Request body</span></span>

<span data-ttu-id="41284-123">在请求正文中, 提供[securityAction](../resources/securityaction.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41284-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="41284-124">响应</span><span class="sxs-lookup"><span data-stu-id="41284-124">Response</span></span>

<span data-ttu-id="41284-125">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41284-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41284-126">示例</span><span class="sxs-lookup"><span data-stu-id="41284-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41284-127">请求</span><span class="sxs-lookup"><span data-stu-id="41284-127">Request</span></span>

<span data-ttu-id="41284-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="41284-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41284-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="41284-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="41284-130">C#</span><span class="sxs-lookup"><span data-stu-id="41284-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41284-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41284-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41284-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="41284-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41284-133">Java</span><span class="sxs-lookup"><span data-stu-id="41284-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41284-134">响应</span><span class="sxs-lookup"><span data-stu-id="41284-134">Response</span></span>

<span data-ttu-id="41284-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41284-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="41284-136">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="41284-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="41284-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="41284-137">All the properties will be returned from an actual call.</span></span>

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
