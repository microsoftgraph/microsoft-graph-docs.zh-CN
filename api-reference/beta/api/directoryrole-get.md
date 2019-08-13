---
title: 获取 directoryRole
description: 检索 directoryRole 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad0081f88f9ce227807039ed45e842cc4b6e0973
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321253"
---
# <a name="get-directoryrole"></a><span data-ttu-id="ae7b7-103">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="ae7b7-103">Get directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae7b7-104">检索 directoryRole 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-104">Retrieve the properties of a directoryRole object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae7b7-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae7b7-105">Permissions</span></span>
<span data-ttu-id="ae7b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae7b7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae7b7-108">Permission type</span></span>      | <span data-ttu-id="ae7b7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae7b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae7b7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae7b7-111">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae7b7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae7b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7b7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-113">Not supported.</span></span>    |
|<span data-ttu-id="ae7b7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae7b7-114">Application</span></span> | <span data-ttu-id="ae7b7-115">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="ae7b7-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7b7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae7b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae7b7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae7b7-117">Optional query parameters</span></span>
<span data-ttu-id="ae7b7-118">此方法**不**支持使用 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应（例如，此处不支持使用 $filter）。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae7b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae7b7-119">Request headers</span></span>
| <span data-ttu-id="ae7b7-120">名称</span><span class="sxs-lookup"><span data-stu-id="ae7b7-120">Name</span></span>       | <span data-ttu-id="ae7b7-121">类型</span><span class="sxs-lookup"><span data-stu-id="ae7b7-121">Type</span></span> | <span data-ttu-id="ae7b7-122">说明</span><span class="sxs-lookup"><span data-stu-id="ae7b7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae7b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7b7-123">Authorization</span></span>  | <span data-ttu-id="ae7b7-124">string</span><span class="sxs-lookup"><span data-stu-id="ae7b7-124">string</span></span>  | <span data-ttu-id="ae7b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae7b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae7b7-127">Request body</span></span>
<span data-ttu-id="ae7b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae7b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="ae7b7-129">Response</span></span>

<span data-ttu-id="ae7b7-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-130">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae7b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="ae7b7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae7b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="ae7b7-132">Request</span></span>
<span data-ttu-id="ae7b7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ae7b7-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ae7b7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae7b7-135">C#</span><span class="sxs-lookup"><span data-stu-id="ae7b7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae7b7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae7b7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae7b7-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="ae7b7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ae7b7-138">Java</span><span class="sxs-lookup"><span data-stu-id="ae7b7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae7b7-139">响应</span><span class="sxs-lookup"><span data-stu-id="ae7b7-139">Response</span></span>
<span data-ttu-id="ae7b7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae7b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 142

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
