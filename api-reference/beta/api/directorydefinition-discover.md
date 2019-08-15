---
title: 'directoryDefinition: 发现'
description: '发现为应用程序预配的最新架构定义。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b405bb29200b05fb23b8232ad9de2db2fdfb0e21
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417528"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="dd70f-103">directoryDefinition: 发现</span><span class="sxs-lookup"><span data-stu-id="dd70f-103">directoryDefinition: discover</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd70f-104">发现为应用程序预配的最新架构定义。</span><span class="sxs-lookup"><span data-stu-id="dd70f-104">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="dd70f-105">权限</span><span class="sxs-lookup"><span data-stu-id="dd70f-105">Permissions</span></span>

<span data-ttu-id="dd70f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd70f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd70f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd70f-108">Permission type</span></span>                        | <span data-ttu-id="dd70f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd70f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd70f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd70f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd70f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd70f-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="dd70f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd70f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd70f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd70f-113">Not supported.</span></span> |
| <span data-ttu-id="dd70f-114">仅限应用程序</span><span class="sxs-lookup"><span data-stu-id="dd70f-114">Application-only</span></span>                            | <span data-ttu-id="dd70f-115">无。</span><span class="sxs-lookup"><span data-stu-id="dd70f-115">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd70f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd70f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="dd70f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd70f-117">Request headers</span></span>

| <span data-ttu-id="dd70f-118">标头</span><span class="sxs-lookup"><span data-stu-id="dd70f-118">Header</span></span>        | <span data-ttu-id="dd70f-119">值</span><span class="sxs-lookup"><span data-stu-id="dd70f-119">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="dd70f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd70f-120">Authorization</span></span> | <span data-ttu-id="dd70f-121">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="dd70f-121">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dd70f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd70f-122">Request body</span></span>

<span data-ttu-id="dd70f-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd70f-123">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="dd70f-124">响应</span><span class="sxs-lookup"><span data-stu-id="dd70f-124">Response</span></span>

<span data-ttu-id="dd70f-125">如果成功, 此方法将`200 OK`返回一个包含[directoryDefinition](../resources/synchronization-directorydefinition.md)对象的响应。</span><span class="sxs-lookup"><span data-stu-id="dd70f-125">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="dd70f-126">示例</span><span class="sxs-lookup"><span data-stu-id="dd70f-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd70f-127">请求</span><span class="sxs-lookup"><span data-stu-id="dd70f-127">Request</span></span>
<span data-ttu-id="dd70f-128">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd70f-128">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd70f-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dd70f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd70f-130">C#</span><span class="sxs-lookup"><span data-stu-id="dd70f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd70f-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd70f-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd70f-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="dd70f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd70f-133">响应</span><span class="sxs-lookup"><span data-stu-id="dd70f-133">Response</span></span>

<span data-ttu-id="dd70f-134">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="dd70f-134">The following is an example of a response.</span></span>

><span data-ttu-id="dd70f-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dd70f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
