---
title: 列出 servicePrincipals
description: 检索 servicePrincipal 对象列表。
localization_priority: Normal
ms.openlocfilehash: 4b408e0af724c6a4b406ca30aef5c77ace50325e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263775"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="d5c82-103">列出 servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="d5c82-103">List servicePrincipals</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5c82-104">检索 servicePrincipal 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d5c82-104">Retrieve a list of servicePrincipal objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c82-105">权限</span><span class="sxs-lookup"><span data-stu-id="d5c82-105">Permissions</span></span>

<span data-ttu-id="d5c82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5c82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5c82-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c82-108">Permission type</span></span>      | <span data-ttu-id="d5c82-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5c82-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c82-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c82-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5c82-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5c82-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5c82-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c82-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c82-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c82-113">Not supported.</span></span>    |
|<span data-ttu-id="d5c82-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5c82-114">Application</span></span> | <span data-ttu-id="d5c82-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c82-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c82-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c82-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5c82-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5c82-117">Optional query parameters</span></span>

<span data-ttu-id="d5c82-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5c82-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5c82-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c82-119">Request headers</span></span>
| <span data-ttu-id="d5c82-120">名称</span><span class="sxs-lookup"><span data-stu-id="d5c82-120">Name</span></span> | <span data-ttu-id="d5c82-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5c82-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d5c82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c82-122">Authorization</span></span>  | <span data-ttu-id="d5c82-123">string</span><span class="sxs-lookup"><span data-stu-id="d5c82-123">string</span></span>  | <span data-ttu-id="d5c82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5c82-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5c82-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c82-126">Request body</span></span>

<span data-ttu-id="d5c82-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5c82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c82-128">响应</span><span class="sxs-lookup"><span data-stu-id="d5c82-128">Response</span></span>

<span data-ttu-id="d5c82-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d5c82-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c82-130">示例</span><span class="sxs-lookup"><span data-stu-id="d5c82-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5c82-131">请求</span><span class="sxs-lookup"><span data-stu-id="d5c82-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipals"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals
```
##### <a name="response"></a><span data-ttu-id="d5c82-132">响应</span><span class="sxs-lookup"><span data-stu-id="d5c82-132">Response</span></span>

<span data-ttu-id="d5c82-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5c82-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d5c82-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d5c82-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d5c82-136">C#</span><span class="sxs-lookup"><span data-stu-id="d5c82-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5c82-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5c82-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d5c82-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="d5c82-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_serviceprincipals-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
