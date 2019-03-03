---
title: 创建安全操作
description: 创建新的安全操作对象。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e1958f80219234fcae54220491629a921dd8bcfd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366887"
---
# <a name="create-security-action"></a><span data-ttu-id="d9045-103">创建安全操作</span><span class="sxs-lookup"><span data-stu-id="d9045-103">Create security action</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9045-104">创建新的[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9045-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9045-105">权限</span><span class="sxs-lookup"><span data-stu-id="d9045-105">Permissions</span></span>

<span data-ttu-id="d9045-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9045-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9045-108">Permission type</span></span>                        | <span data-ttu-id="d9045-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9045-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d9045-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9045-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9045-111">SecurityActions</span><span class="sxs-lookup"><span data-stu-id="d9045-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="d9045-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9045-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9045-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9045-113">Not supported.</span></span> |
| <span data-ttu-id="d9045-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9045-114">Application</span></span>                            | <span data-ttu-id="d9045-115">SecurityActions</span><span class="sxs-lookup"><span data-stu-id="d9045-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9045-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9045-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="d9045-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9045-117">Request headers</span></span>

| <span data-ttu-id="d9045-118">名称</span><span class="sxs-lookup"><span data-stu-id="d9045-118">Name</span></span>          | <span data-ttu-id="d9045-119">说明</span><span class="sxs-lookup"><span data-stu-id="d9045-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d9045-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9045-120">Authorization</span></span> | <span data-ttu-id="d9045-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d9045-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9045-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9045-122">Request body</span></span>

<span data-ttu-id="d9045-123">在请求正文中, 提供[securityAction](../resources/securityaction.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9045-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d9045-124">响应</span><span class="sxs-lookup"><span data-stu-id="d9045-124">Response</span></span>

<span data-ttu-id="d9045-125">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d9045-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9045-126">示例</span><span class="sxs-lookup"><span data-stu-id="d9045-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9045-127">请求</span><span class="sxs-lookup"><span data-stu-id="d9045-127">Request</span></span>

<span data-ttu-id="d9045-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9045-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9045-129">响应</span><span class="sxs-lookup"><span data-stu-id="d9045-129">Response</span></span>

<span data-ttu-id="d9045-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d9045-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d9045-131">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d9045-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d9045-132">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9045-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
