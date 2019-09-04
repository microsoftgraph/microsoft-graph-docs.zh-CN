---
title: 列出 administrativeUnits
description: 检索 administrativeUnit 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e48373cb2e26111e9ffe2fbd12213db0207396e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719155"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="2bb99-103">列出 administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="2bb99-103">List administrativeUnits</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bb99-104">检索[administrativeUnit](../resources/administrativeunit.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2bb99-104">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2bb99-105">权限</span><span class="sxs-lookup"><span data-stu-id="2bb99-105">Permissions</span></span>
<span data-ttu-id="2bb99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bb99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2bb99-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bb99-108">Permission type</span></span>      | <span data-ttu-id="2bb99-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bb99-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bb99-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb99-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2bb99-111">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="2bb99-111">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2bb99-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bb99-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bb99-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bb99-113">Not supported.</span></span>    |
|<span data-ttu-id="2bb99-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bb99-114">Application</span></span> | <span data-ttu-id="2bb99-115">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="2bb99-115">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bb99-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bb99-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bb99-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2bb99-117">Optional query parameters</span></span>
<span data-ttu-id="2bb99-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2bb99-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bb99-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bb99-119">Request headers</span></span>
| <span data-ttu-id="2bb99-120">名称</span><span class="sxs-lookup"><span data-stu-id="2bb99-120">Name</span></span>      |<span data-ttu-id="2bb99-121">说明</span><span class="sxs-lookup"><span data-stu-id="2bb99-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2bb99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb99-122">Authorization</span></span>  | <span data-ttu-id="2bb99-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bb99-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bb99-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bb99-125">Request body</span></span>
<span data-ttu-id="2bb99-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bb99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bb99-127">响应</span><span class="sxs-lookup"><span data-stu-id="2bb99-127">Response</span></span>

<span data-ttu-id="2bb99-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[administrativeUnit](../resources/administrativeunit.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2bb99-128">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bb99-129">示例</span><span class="sxs-lookup"><span data-stu-id="2bb99-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bb99-130">请求</span><span class="sxs-lookup"><span data-stu-id="2bb99-130">Request</span></span>
<span data-ttu-id="2bb99-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bb99-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2bb99-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2bb99-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2bb99-133">C#</span><span class="sxs-lookup"><span data-stu-id="2bb99-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2bb99-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bb99-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2bb99-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="2bb99-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2bb99-136">响应</span><span class="sxs-lookup"><span data-stu-id="2bb99-136">Response</span></span>
<span data-ttu-id="2bb99-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bb99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
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
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
