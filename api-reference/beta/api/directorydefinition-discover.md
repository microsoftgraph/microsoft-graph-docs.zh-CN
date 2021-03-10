---
title: directoryDefinition：发现
description: '发现用于预配到应用程序的最新架构定义。 '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4b83168464b8f8ab563ffa549d601e35929684bb
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625883"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="96e2e-103">directoryDefinition：发现</span><span class="sxs-lookup"><span data-stu-id="96e2e-103">directoryDefinition: discover</span></span>

<span data-ttu-id="96e2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e2e-105">发现用于预配到应用程序的最新架构定义。</span><span class="sxs-lookup"><span data-stu-id="96e2e-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="96e2e-106">权限</span><span class="sxs-lookup"><span data-stu-id="96e2e-106">Permissions</span></span>

<span data-ttu-id="96e2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96e2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e2e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96e2e-109">Permission type</span></span>                        | <span data-ttu-id="96e2e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96e2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="96e2e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96e2e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="96e2e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e2e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="96e2e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96e2e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="96e2e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="96e2e-114">Not supported.</span></span>|
|<span data-ttu-id="96e2e-115">Application</span><span class="sxs-lookup"><span data-stu-id="96e2e-115">Application</span></span>                            |<span data-ttu-id="96e2e-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e2e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="96e2e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96e2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="96e2e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96e2e-118">Request headers</span></span>

| <span data-ttu-id="96e2e-119">标头</span><span class="sxs-lookup"><span data-stu-id="96e2e-119">Header</span></span>        | <span data-ttu-id="96e2e-120">值</span><span class="sxs-lookup"><span data-stu-id="96e2e-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="96e2e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e2e-121">Authorization</span></span> | <span data-ttu-id="96e2e-122">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="96e2e-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96e2e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="96e2e-123">Request body</span></span>

<span data-ttu-id="96e2e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96e2e-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="96e2e-125">响应</span><span class="sxs-lookup"><span data-stu-id="96e2e-125">Response</span></span>

<span data-ttu-id="96e2e-126">如果成功，此方法返回 `200 OK` 一个 [包含 directoryDefinition 对象的](../resources/synchronization-directorydefinition.md) 响应。</span><span class="sxs-lookup"><span data-stu-id="96e2e-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="96e2e-127">示例</span><span class="sxs-lookup"><span data-stu-id="96e2e-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="96e2e-128">请求</span><span class="sxs-lookup"><span data-stu-id="96e2e-128">Request</span></span>
<span data-ttu-id="96e2e-129">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="96e2e-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96e2e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="96e2e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="96e2e-131">C#</span><span class="sxs-lookup"><span data-stu-id="96e2e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96e2e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96e2e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96e2e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96e2e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96e2e-134">Java</span><span class="sxs-lookup"><span data-stu-id="96e2e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96e2e-135">响应</span><span class="sxs-lookup"><span data-stu-id="96e2e-135">Response</span></span>

<span data-ttu-id="96e2e-136">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="96e2e-136">The following is an example of a response.</span></span>

><span data-ttu-id="96e2e-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96e2e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


