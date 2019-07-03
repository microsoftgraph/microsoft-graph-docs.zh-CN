---
title: 列出 directoryRoleTemplates
description: 检索 directoryroletemplate 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c92a872a2db9cace2a70625f17cce8d4c394959
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436856"
---
# <a name="list-directoryroletemplates"></a><span data-ttu-id="edf58-103">列出 directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="edf58-103">List directoryRoleTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edf58-104">检索 directoryroletemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="edf58-104">Retrieve a list of directoryroletemplate objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="edf58-105">权限</span><span class="sxs-lookup"><span data-stu-id="edf58-105">Permissions</span></span>
<span data-ttu-id="edf58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edf58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edf58-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="edf58-108">Permission type</span></span>      | <span data-ttu-id="edf58-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edf58-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edf58-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edf58-110">Delegated (work or school account)</span></span> | <span data-ttu-id="edf58-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edf58-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edf58-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edf58-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edf58-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="edf58-113">Not supported.</span></span>    |
|<span data-ttu-id="edf58-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="edf58-114">Application</span></span> | <span data-ttu-id="edf58-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edf58-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="edf58-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edf58-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="edf58-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="edf58-117">Optional query parameters</span></span>
<span data-ttu-id="edf58-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="edf58-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="edf58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="edf58-119">Request headers</span></span>
| <span data-ttu-id="edf58-120">名称</span><span class="sxs-lookup"><span data-stu-id="edf58-120">Name</span></span>       | <span data-ttu-id="edf58-121">类型</span><span class="sxs-lookup"><span data-stu-id="edf58-121">Type</span></span> | <span data-ttu-id="edf58-122">说明</span><span class="sxs-lookup"><span data-stu-id="edf58-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="edf58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edf58-123">Authorization</span></span>  | <span data-ttu-id="edf58-124">string</span><span class="sxs-lookup"><span data-stu-id="edf58-124">string</span></span>  | <span data-ttu-id="edf58-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edf58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="edf58-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="edf58-127">Request body</span></span>
<span data-ttu-id="edf58-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="edf58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edf58-129">响应</span><span class="sxs-lookup"><span data-stu-id="edf58-129">Response</span></span>

<span data-ttu-id="edf58-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRoleTemplate](../resources/directoryroletemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="edf58-130">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edf58-131">示例</span><span class="sxs-lookup"><span data-stu-id="edf58-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edf58-132">请求</span><span class="sxs-lookup"><span data-stu-id="edf58-132">Request</span></span>
<span data-ttu-id="edf58-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edf58-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="edf58-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="edf58-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="edf58-135">C#</span><span class="sxs-lookup"><span data-stu-id="edf58-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroletemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="edf58-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="edf58-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroletemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="edf58-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="edf58-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroletemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="edf58-138">响应</span><span class="sxs-lookup"><span data-stu-id="edf58-138">Response</span></span>
<span data-ttu-id="edf58-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edf58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 139

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
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
