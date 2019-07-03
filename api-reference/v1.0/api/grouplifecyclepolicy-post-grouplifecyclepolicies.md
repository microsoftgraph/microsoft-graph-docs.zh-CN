---
title: 创建 groupLifecyclePolicy
description: 新建 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 68b9fc2437be6c6d3825f68e02f778db69f85c2b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445686"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="807ae-103">创建 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="807ae-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="807ae-104">新建 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="807ae-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="807ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="807ae-105">Permissions</span></span>

<span data-ttu-id="807ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="807ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="807ae-108">Permission type</span></span>      | <span data-ttu-id="807ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="807ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="807ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="807ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="807ae-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="807ae-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="807ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="807ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="807ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="807ae-113">Not supported.</span></span>    |
|<span data-ttu-id="807ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="807ae-114">Application</span></span> | <span data-ttu-id="807ae-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="807ae-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="807ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="807ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="807ae-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="807ae-117">Request headers</span></span>

| <span data-ttu-id="807ae-118">名称</span><span class="sxs-lookup"><span data-stu-id="807ae-118">Name</span></span> | <span data-ttu-id="807ae-119">说明</span><span class="sxs-lookup"><span data-stu-id="807ae-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="807ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="807ae-120">Authorization</span></span> | <span data-ttu-id="807ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="807ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="807ae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="807ae-123">Content-Type</span></span>  | <span data-ttu-id="807ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="807ae-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="807ae-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="807ae-125">Request body</span></span>
<span data-ttu-id="807ae-126">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="807ae-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="807ae-127">响应</span><span class="sxs-lookup"><span data-stu-id="807ae-127">Response</span></span>

<span data-ttu-id="807ae-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="807ae-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="807ae-129">示例</span><span class="sxs-lookup"><span data-stu-id="807ae-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="807ae-130">请求</span><span class="sxs-lookup"><span data-stu-id="807ae-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="807ae-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="807ae-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="807ae-132">C#</span><span class="sxs-lookup"><span data-stu-id="807ae-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="807ae-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="807ae-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="807ae-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="807ae-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="807ae-135">在请求正文中，提供 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="807ae-135">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="807ae-136">响应</span><span class="sxs-lookup"><span data-stu-id="807ae-136">Response</span></span>

<span data-ttu-id="807ae-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="807ae-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
