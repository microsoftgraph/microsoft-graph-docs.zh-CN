---
title: 获取组设置
description: 检索特定组设置对象的属性。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b92840fd1a10ab6960886e8d783ee758d5d1e96b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679776"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="d6eeb-103">获取组设置</span><span class="sxs-lookup"><span data-stu-id="d6eeb-103">Get a group setting</span></span>

<span data-ttu-id="d6eeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6eeb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6eeb-105">检索特定组设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-105">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6eeb-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6eeb-106">Permissions</span></span>

<span data-ttu-id="d6eeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d6eeb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6eeb-109">Permission type</span></span>      | <span data-ttu-id="d6eeb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6eeb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6eeb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6eeb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6eeb-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6eeb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6eeb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6eeb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6eeb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-114">Not supported.</span></span>    |
|<span data-ttu-id="d6eeb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6eeb-115">Application</span></span> | <span data-ttu-id="d6eeb-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6eeb-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6eeb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6eeb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d6eeb-118">获取特定租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-118">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6eeb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6eeb-119">Optional query parameters</span></span>
<span data-ttu-id="d6eeb-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="d6eeb-121">注意：不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-121">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6eeb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6eeb-122">Request headers</span></span>
| <span data-ttu-id="d6eeb-123">名称</span><span class="sxs-lookup"><span data-stu-id="d6eeb-123">Name</span></span> | <span data-ttu-id="d6eeb-124">说明</span><span class="sxs-lookup"><span data-stu-id="d6eeb-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d6eeb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6eeb-125">Authorization</span></span> | <span data-ttu-id="d6eeb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6eeb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6eeb-128">Request body</span></span>

<span data-ttu-id="d6eeb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6eeb-130">响应</span><span class="sxs-lookup"><span data-stu-id="d6eeb-130">Response</span></span>

<span data-ttu-id="d6eeb-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-131">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6eeb-132">示例</span><span class="sxs-lookup"><span data-stu-id="d6eeb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6eeb-133">请求</span><span class="sxs-lookup"><span data-stu-id="d6eeb-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d6eeb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6eeb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="d6eeb-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6eeb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6eeb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6eeb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6eeb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6eeb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6eeb-138">Java</span><span class="sxs-lookup"><span data-stu-id="d6eeb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6eeb-139">响应</span><span class="sxs-lookup"><span data-stu-id="d6eeb-139">Response</span></span>

<span data-ttu-id="d6eeb-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d6eeb-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
