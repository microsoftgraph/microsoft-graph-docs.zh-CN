---
title: 列出 groupLifecyclePolicy
description: 检索组所属的 groupLifecyclePolicy 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c4c63497b82c23bbefb2eee6bae5fc0ec30c4849
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419462"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="a0982-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a0982-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="a0982-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a0982-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0982-105">检索组所属的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a0982-105">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0982-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0982-106">Permissions</span></span>

<span data-ttu-id="a0982-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0982-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0982-109">Permission type</span></span>      | <span data-ttu-id="a0982-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0982-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0982-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0982-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0982-112">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0982-112">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a0982-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0982-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0982-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0982-114">Not supported.</span></span>    |
|<span data-ttu-id="a0982-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0982-115">Application</span></span> | <span data-ttu-id="a0982-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0982-116">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0982-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0982-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0982-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0982-118">Optional query parameters</span></span>
<span data-ttu-id="a0982-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0982-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0982-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0982-120">Request headers</span></span>
| <span data-ttu-id="a0982-121">名称</span><span class="sxs-lookup"><span data-stu-id="a0982-121">Name</span></span> | <span data-ttu-id="a0982-122">说明</span><span class="sxs-lookup"><span data-stu-id="a0982-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a0982-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0982-123">Authorization</span></span> | <span data-ttu-id="a0982-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0982-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0982-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0982-126">Request body</span></span>
<span data-ttu-id="a0982-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0982-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a0982-128">响应</span><span class="sxs-lookup"><span data-stu-id="a0982-128">Response</span></span>
<span data-ttu-id="a0982-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a0982-129">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0982-130">示例</span><span class="sxs-lookup"><span data-stu-id="a0982-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0982-131">请求</span><span class="sxs-lookup"><span data-stu-id="a0982-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a0982-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0982-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="a0982-133">C#</span><span class="sxs-lookup"><span data-stu-id="a0982-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0982-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0982-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0982-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0982-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0982-136">响应</span><span class="sxs-lookup"><span data-stu-id="a0982-136">Response</span></span>

<span data-ttu-id="a0982-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0982-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 227

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
