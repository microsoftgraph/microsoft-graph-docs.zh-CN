---
title: directoryDefinition：发现
description: '发现为应用程序预配的最新架构定义。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 093622b9da3e59f7230547451eac8fc8aedd6bc7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435078"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="14695-103">directoryDefinition：发现</span><span class="sxs-lookup"><span data-stu-id="14695-103">directoryDefinition: discover</span></span>

<span data-ttu-id="14695-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14695-105">发现为应用程序预配的最新架构定义。</span><span class="sxs-lookup"><span data-stu-id="14695-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="14695-106">权限</span><span class="sxs-lookup"><span data-stu-id="14695-106">Permissions</span></span>

<span data-ttu-id="14695-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14695-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14695-109">Permission type</span></span>                        | <span data-ttu-id="14695-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14695-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14695-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14695-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14695-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14695-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="14695-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14695-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14695-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14695-114">Not supported.</span></span> |
| <span data-ttu-id="14695-115">仅限应用程序</span><span class="sxs-lookup"><span data-stu-id="14695-115">Application-only</span></span>                            | <span data-ttu-id="14695-116">无。</span><span class="sxs-lookup"><span data-stu-id="14695-116">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14695-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14695-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="14695-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="14695-118">Request headers</span></span>

| <span data-ttu-id="14695-119">标头</span><span class="sxs-lookup"><span data-stu-id="14695-119">Header</span></span>        | <span data-ttu-id="14695-120">值</span><span class="sxs-lookup"><span data-stu-id="14695-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="14695-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14695-121">Authorization</span></span> | <span data-ttu-id="14695-122">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="14695-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14695-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="14695-123">Request body</span></span>

<span data-ttu-id="14695-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14695-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="14695-125">响应</span><span class="sxs-lookup"><span data-stu-id="14695-125">Response</span></span>

<span data-ttu-id="14695-126">如果成功，此方法将`200 OK`返回一个包含[directoryDefinition](../resources/synchronization-directorydefinition.md)对象的响应。</span><span class="sxs-lookup"><span data-stu-id="14695-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="14695-127">示例</span><span class="sxs-lookup"><span data-stu-id="14695-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="14695-128">请求</span><span class="sxs-lookup"><span data-stu-id="14695-128">Request</span></span>
<span data-ttu-id="14695-129">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="14695-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14695-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="14695-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="14695-131">C#</span><span class="sxs-lookup"><span data-stu-id="14695-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14695-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14695-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14695-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14695-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14695-134">响应</span><span class="sxs-lookup"><span data-stu-id="14695-134">Response</span></span>

<span data-ttu-id="14695-135">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="14695-135">The following is an example of a response.</span></span>

><span data-ttu-id="14695-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14695-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```
