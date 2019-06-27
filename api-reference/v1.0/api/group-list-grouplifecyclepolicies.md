---
title: 列出 groupLifecyclePolicy
description: 检索组所属的 groupLifecyclePolicy 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5ace0257e6bf8389fc3149947903bfd7d64f4e82
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273519"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="e1500-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e1500-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="e1500-104">检索组所属的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e1500-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1500-105">权限</span><span class="sxs-lookup"><span data-stu-id="e1500-105">Permissions</span></span>

<span data-ttu-id="e1500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1500-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1500-108">Permission type</span></span>      | <span data-ttu-id="e1500-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1500-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1500-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1500-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1500-111">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1500-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e1500-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1500-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1500-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1500-113">Not supported.</span></span>    |
|<span data-ttu-id="e1500-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1500-114">Application</span></span> | <span data-ttu-id="e1500-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1500-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1500-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1500-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1500-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e1500-117">Optional query parameters</span></span>
<span data-ttu-id="e1500-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e1500-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1500-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1500-119">Request headers</span></span>
| <span data-ttu-id="e1500-120">名称</span><span class="sxs-lookup"><span data-stu-id="e1500-120">Name</span></span> | <span data-ttu-id="e1500-121">说明</span><span class="sxs-lookup"><span data-stu-id="e1500-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="e1500-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1500-122">Authorization</span></span> | <span data-ttu-id="e1500-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1500-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1500-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1500-125">Request body</span></span>
<span data-ttu-id="e1500-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e1500-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e1500-127">响应</span><span class="sxs-lookup"><span data-stu-id="e1500-127">Response</span></span>
<span data-ttu-id="e1500-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e1500-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1500-129">示例</span><span class="sxs-lookup"><span data-stu-id="e1500-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1500-130">请求</span><span class="sxs-lookup"><span data-stu-id="e1500-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="e1500-131">响应</span><span class="sxs-lookup"><span data-stu-id="e1500-131">Response</span></span>

<span data-ttu-id="e1500-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1500-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e1500-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e1500-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e1500-135">C#</span><span class="sxs-lookup"><span data-stu-id="e1500-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1500-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1500-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e1500-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="e1500-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
