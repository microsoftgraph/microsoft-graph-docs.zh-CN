---
title: 列出 directoryRoleTemplates
description: 检索 directoryRoleTemplate 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 68b0d69ee8f85e32dbf719e16dc08153c65e3954
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891078"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="58d2e-103">列出 directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="58d2e-103">List directoryRoleTemplates</span></span>

<span data-ttu-id="58d2e-104">检索 directoryRoleTemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="58d2e-104">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="58d2e-105">权限</span><span class="sxs-lookup"><span data-stu-id="58d2e-105">Permissions</span></span>
<span data-ttu-id="58d2e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58d2e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="58d2e-108">Permission type</span></span>      | <span data-ttu-id="58d2e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58d2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58d2e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58d2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58d2e-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58d2e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58d2e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58d2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d2e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="58d2e-113">Not supported.</span></span>    |
|<span data-ttu-id="58d2e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="58d2e-114">Application</span></span> | <span data-ttu-id="58d2e-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d2e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58d2e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58d2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58d2e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="58d2e-117">Optional query parameters</span></span>
<span data-ttu-id="58d2e-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="58d2e-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="58d2e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="58d2e-119">Request headers</span></span>
| <span data-ttu-id="58d2e-120">名称</span><span class="sxs-lookup"><span data-stu-id="58d2e-120">Name</span></span>       | <span data-ttu-id="58d2e-121">类型</span><span class="sxs-lookup"><span data-stu-id="58d2e-121">Type</span></span> | <span data-ttu-id="58d2e-122">说明</span><span class="sxs-lookup"><span data-stu-id="58d2e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58d2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d2e-123">Authorization</span></span>  | <span data-ttu-id="58d2e-124">string</span><span class="sxs-lookup"><span data-stu-id="58d2e-124">string</span></span>  | <span data-ttu-id="58d2e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58d2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58d2e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58d2e-127">Request body</span></span>
<span data-ttu-id="58d2e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58d2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58d2e-129">响应</span><span class="sxs-lookup"><span data-stu-id="58d2e-129">Response</span></span>

<span data-ttu-id="58d2e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRoleTemplate](../resources/directoryroletemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="58d2e-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58d2e-131">示例</span><span class="sxs-lookup"><span data-stu-id="58d2e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58d2e-132">请求</span><span class="sxs-lookup"><span data-stu-id="58d2e-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="58d2e-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="58d2e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="58d2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="58d2e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="58d2e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="58d2e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="58d2e-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="58d2e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="58d2e-137">Java</span><span class="sxs-lookup"><span data-stu-id="58d2e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroletemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58d2e-138">响应</span><span class="sxs-lookup"><span data-stu-id="58d2e-138">Response</span></span>
<span data-ttu-id="58d2e-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58d2e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
