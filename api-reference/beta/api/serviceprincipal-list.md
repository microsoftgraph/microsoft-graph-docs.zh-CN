---
title: 列出 servicePrincipals
description: 检索 servicePrincipal 对象列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 728766ae1bb092ce1e5783f2d6adc08860928c67
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218638"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="0e6f8-103">列出 servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="0e6f8-103">List servicePrincipals</span></span>

<span data-ttu-id="0e6f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e6f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e6f8-105">检索 servicePrincipal 对象列表。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-105">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e6f8-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e6f8-106">Permissions</span></span>

<span data-ttu-id="0e6f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0e6f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e6f8-109">Permission type</span></span>      | <span data-ttu-id="0e6f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e6f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e6f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e6f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e6f8-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e6f8-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e6f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e6f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e6f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-114">Not supported.</span></span>    |
|<span data-ttu-id="0e6f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e6f8-115">Application</span></span> | <span data-ttu-id="0e6f8-116">应用程序。全部，全部读取全部，全部</span><span class="sxs-lookup"><span data-stu-id="0e6f8-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e6f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e6f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e6f8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e6f8-118">Optional query parameters</span></span>

<span data-ttu-id="0e6f8-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e6f8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e6f8-120">Request headers</span></span>
| <span data-ttu-id="0e6f8-121">名称</span><span class="sxs-lookup"><span data-stu-id="0e6f8-121">Name</span></span> | <span data-ttu-id="0e6f8-122">说明</span><span class="sxs-lookup"><span data-stu-id="0e6f8-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0e6f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e6f8-123">Authorization</span></span>  | <span data-ttu-id="0e6f8-124">string</span><span class="sxs-lookup"><span data-stu-id="0e6f8-124">string</span></span>  | <span data-ttu-id="0e6f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e6f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e6f8-127">Request body</span></span>

<span data-ttu-id="0e6f8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e6f8-129">响应</span><span class="sxs-lookup"><span data-stu-id="0e6f8-129">Response</span></span>

<span data-ttu-id="0e6f8-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-130">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e6f8-131">示例</span><span class="sxs-lookup"><span data-stu-id="0e6f8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e6f8-132">请求</span><span class="sxs-lookup"><span data-stu-id="0e6f8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0e6f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e6f8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals
```
# <a name="c"></a>[<span data-ttu-id="0e6f8-134">C#</span><span class="sxs-lookup"><span data-stu-id="0e6f8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e6f8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e6f8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e6f8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e6f8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0e6f8-137">响应</span><span class="sxs-lookup"><span data-stu-id="0e6f8-137">Response</span></span>

<span data-ttu-id="0e6f8-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e6f8-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 488

{
  "value": [
    {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
