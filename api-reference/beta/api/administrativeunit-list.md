---
title: 列出 administrativeUnits
description: 检索 administrativeUnit 对象的列表。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29ab43c08728c6c60d3ed048a02bab9a17f8f452
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312643"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="038c5-103">列出 administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="038c5-103">List administrativeUnits</span></span>

<span data-ttu-id="038c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="038c5-105">检索 [administrativeUnit](../resources/administrativeunit.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="038c5-105">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="038c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="038c5-106">Permissions</span></span>
<span data-ttu-id="038c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="038c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="038c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="038c5-109">Permission type</span></span>      | <span data-ttu-id="038c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="038c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="038c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="038c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="038c5-112">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="038c5-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="038c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="038c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="038c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="038c5-114">Not supported.</span></span>    |
|<span data-ttu-id="038c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="038c5-115">Application</span></span> | <span data-ttu-id="038c5-116">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="038c5-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="038c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="038c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="038c5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="038c5-118">Optional query parameters</span></span>
<span data-ttu-id="038c5-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="038c5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="038c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="038c5-120">Request headers</span></span>
| <span data-ttu-id="038c5-121">名称</span><span class="sxs-lookup"><span data-stu-id="038c5-121">Name</span></span>      |<span data-ttu-id="038c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="038c5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="038c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="038c5-123">Authorization</span></span>  | <span data-ttu-id="038c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="038c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="038c5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="038c5-126">Request body</span></span>
<span data-ttu-id="038c5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="038c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="038c5-128">响应</span><span class="sxs-lookup"><span data-stu-id="038c5-128">Response</span></span>

<span data-ttu-id="038c5-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="038c5-129">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="038c5-130">示例</span><span class="sxs-lookup"><span data-stu-id="038c5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="038c5-131">请求</span><span class="sxs-lookup"><span data-stu-id="038c5-131">Request</span></span>
<span data-ttu-id="038c5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="038c5-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="038c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="038c5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="c"></a>[<span data-ttu-id="038c5-134">C#</span><span class="sxs-lookup"><span data-stu-id="038c5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038c5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038c5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038c5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038c5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="038c5-137">响应</span><span class="sxs-lookup"><span data-stu-id="038c5-137">Response</span></span>
<span data-ttu-id="038c5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="038c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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