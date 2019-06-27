---
title: 检查成员组
description: 检查指定组列表中的成员身份, 并从该列表返回这些组
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc858afd18430635d991ce5e564b1a7c7976ad86
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275591"
---
# <a name="check-member-groups"></a><span data-ttu-id="b244d-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="b244d-103">Check member groups</span></span>

<span data-ttu-id="b244d-p101">检查特定组列表中的成员资格，并从该列表返回成员为指定的 user、group 或 directory 对象的组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b244d-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b244d-106">权限</span><span class="sxs-lookup"><span data-stu-id="b244d-106">Permissions</span></span>
<span data-ttu-id="b244d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b244d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b244d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b244d-109">Permission type</span></span>      | <span data-ttu-id="b244d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b244d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b244d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b244d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b244d-112">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b244d-112">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="b244d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b244d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b244d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b244d-114">Not supported.</span></span>    |
|<span data-ttu-id="b244d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b244d-115">Application</span></span> | <span data-ttu-id="b244d-116">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b244d-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b244d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b244d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b244d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b244d-118">Request headers</span></span>
| <span data-ttu-id="b244d-119">名称</span><span class="sxs-lookup"><span data-stu-id="b244d-119">Name</span></span>       | <span data-ttu-id="b244d-120">类型</span><span class="sxs-lookup"><span data-stu-id="b244d-120">Type</span></span> | <span data-ttu-id="b244d-121">说明</span><span class="sxs-lookup"><span data-stu-id="b244d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b244d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b244d-122">Authorization</span></span>  | <span data-ttu-id="b244d-123">string</span><span class="sxs-lookup"><span data-stu-id="b244d-123">string</span></span>  | <span data-ttu-id="b244d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b244d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b244d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b244d-126">Content-Type</span></span>  | <span data-ttu-id="b244d-127">string</span><span class="sxs-lookup"><span data-stu-id="b244d-127">string</span></span> | <span data-ttu-id="b244d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b244d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b244d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b244d-129">Request body</span></span>
<span data-ttu-id="b244d-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b244d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b244d-131">参数</span><span class="sxs-lookup"><span data-stu-id="b244d-131">Parameter</span></span>    | <span data-ttu-id="b244d-132">类型</span><span class="sxs-lookup"><span data-stu-id="b244d-132">Type</span></span>   |<span data-ttu-id="b244d-133">说明</span><span class="sxs-lookup"><span data-stu-id="b244d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b244d-134">groupIds</span><span class="sxs-lookup"><span data-stu-id="b244d-134">groupIds</span></span>|<span data-ttu-id="b244d-135">String collection</span><span class="sxs-lookup"><span data-stu-id="b244d-135">String collection</span></span>|<span data-ttu-id="b244d-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="b244d-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b244d-138">响应</span><span class="sxs-lookup"><span data-stu-id="b244d-138">Response</span></span>

<span data-ttu-id="b244d-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b244d-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b244d-140">示例</span><span class="sxs-lookup"><span data-stu-id="b244d-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b244d-141">请求</span><span class="sxs-lookup"><span data-stu-id="b244d-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="b244d-142">响应</span><span class="sxs-lookup"><span data-stu-id="b244d-142">Response</span></span>
<span data-ttu-id="b244d-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b244d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b244d-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b244d-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b244d-146">C#</span><span class="sxs-lookup"><span data-stu-id="b244d-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b244d-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="b244d-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b244d-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="b244d-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
