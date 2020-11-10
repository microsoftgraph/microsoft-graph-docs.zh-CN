---
title: 创建 groupLifecyclePolicy
description: 新建 groupLifecyclePolicy。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0700729a30e6e58eaed8f3a90c87111bf3cfe971
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953634"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="a9049-103">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a9049-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="a9049-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9049-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9049-105">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="a9049-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9049-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9049-106">Permissions</span></span>

<span data-ttu-id="a9049-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9049-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9049-109">Permission type</span></span>      | <span data-ttu-id="a9049-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9049-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9049-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9049-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9049-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9049-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9049-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9049-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9049-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a9049-114">Not supported</span></span> |
|<span data-ttu-id="a9049-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9049-115">Application</span></span> |  <span data-ttu-id="a9049-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9049-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9049-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9049-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="a9049-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9049-118">Request headers</span></span>

| <span data-ttu-id="a9049-119">名称</span><span class="sxs-lookup"><span data-stu-id="a9049-119">Name</span></span> | <span data-ttu-id="a9049-120">说明</span><span class="sxs-lookup"><span data-stu-id="a9049-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a9049-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9049-121">Authorization</span></span> | <span data-ttu-id="a9049-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9049-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9049-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9049-124">Content-Type</span></span>  | <span data-ttu-id="a9049-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9049-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9049-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9049-126">Request body</span></span>
<span data-ttu-id="a9049-127">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9049-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a9049-128">响应</span><span class="sxs-lookup"><span data-stu-id="a9049-128">Response</span></span>

<span data-ttu-id="a9049-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9049-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9049-130">示例</span><span class="sxs-lookup"><span data-stu-id="a9049-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a9049-131">请求</span><span class="sxs-lookup"><span data-stu-id="a9049-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a9049-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9049-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="a9049-133">C#</span><span class="sxs-lookup"><span data-stu-id="a9049-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9049-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9049-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9049-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9049-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9049-136">Java</span><span class="sxs-lookup"><span data-stu-id="a9049-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a9049-137">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9049-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a9049-138">响应</span><span class="sxs-lookup"><span data-stu-id="a9049-138">Response</span></span>

<span data-ttu-id="a9049-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9049-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


