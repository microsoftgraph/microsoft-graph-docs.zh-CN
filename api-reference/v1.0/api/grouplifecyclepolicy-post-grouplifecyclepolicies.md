---
title: 创建 groupLifecyclePolicy
description: 新建 groupLifecyclePolicy。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 13c351c9fd98486886c28cd2486841067989907c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679804"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="7e87c-103">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7e87c-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="7e87c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e87c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e87c-105">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="7e87c-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e87c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e87c-106">Permissions</span></span>

<span data-ttu-id="7e87c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e87c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e87c-109">Permission type</span></span>      | <span data-ttu-id="7e87c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e87c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e87c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e87c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e87c-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e87c-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e87c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e87c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e87c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e87c-114">Not supported.</span></span>    |
|<span data-ttu-id="7e87c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e87c-115">Application</span></span> | <span data-ttu-id="7e87c-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e87c-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e87c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e87c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="7e87c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e87c-118">Request headers</span></span>

| <span data-ttu-id="7e87c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7e87c-119">Name</span></span> | <span data-ttu-id="7e87c-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e87c-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7e87c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e87c-121">Authorization</span></span> | <span data-ttu-id="7e87c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e87c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e87c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e87c-124">Content-Type</span></span>  | <span data-ttu-id="7e87c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e87c-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e87c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e87c-126">Request body</span></span>
<span data-ttu-id="7e87c-127">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e87c-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7e87c-128">响应</span><span class="sxs-lookup"><span data-stu-id="7e87c-128">Response</span></span>

<span data-ttu-id="7e87c-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7e87c-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e87c-130">示例</span><span class="sxs-lookup"><span data-stu-id="7e87c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e87c-131">请求</span><span class="sxs-lookup"><span data-stu-id="7e87c-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7e87c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e87c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="7e87c-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e87c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e87c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e87c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e87c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e87c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e87c-136">Java</span><span class="sxs-lookup"><span data-stu-id="7e87c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7e87c-137">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e87c-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7e87c-138">响应</span><span class="sxs-lookup"><span data-stu-id="7e87c-138">Response</span></span>

<span data-ttu-id="7e87c-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7e87c-139">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

