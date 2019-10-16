---
title: 用户： reprocessLicenseAssignment
description: 重新处理用户的所有基于组的许可证分配。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4de2d47baf7f830cf12b645f0ee4bb7520f0980c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538394"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="c014d-103">用户： reprocessLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="c014d-103">user: reprocessLicenseAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c014d-104">重新处理用户的所有基于组的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="c014d-104">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="c014d-105">若要了解有关基于组的许可的详细信息，请参阅[什么是 Azure Active Directory 中的基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="c014d-105">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="c014d-106">有关更多详细信息，请参阅[识别和解决 Azure Active Directory 中的组的许可证分配问题](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="c014d-106">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="c014d-107">权限</span><span class="sxs-lookup"><span data-stu-id="c014d-107">Permissions</span></span>
<span data-ttu-id="c014d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c014d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c014d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c014d-110">Permission type</span></span>      | <span data-ttu-id="c014d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c014d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c014d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c014d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c014d-113">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c014d-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c014d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c014d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c014d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c014d-115">Not supported.</span></span>    |
|<span data-ttu-id="c014d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c014d-116">Application</span></span> | <span data-ttu-id="c014d-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c014d-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c014d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c014d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="c014d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c014d-119">Request headers</span></span>
| <span data-ttu-id="c014d-120">标头</span><span class="sxs-lookup"><span data-stu-id="c014d-120">Header</span></span>       | <span data-ttu-id="c014d-121">值</span><span class="sxs-lookup"><span data-stu-id="c014d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c014d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c014d-122">Authorization</span></span>  | <span data-ttu-id="c014d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c014d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c014d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c014d-125">Request body</span></span>
<span data-ttu-id="c014d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c014d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c014d-127">响应</span><span class="sxs-lookup"><span data-stu-id="c014d-127">Response</span></span>

<span data-ttu-id="c014d-128">如果成功，此方法在`200 OK`响应正文中返回响应代码和更新的[user](../resources/user.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c014d-128">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c014d-129">示例</span><span class="sxs-lookup"><span data-stu-id="c014d-129">Example</span></span>
<span data-ttu-id="c014d-130">下面的示例展示了如何重新处理用户的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="c014d-130">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="c014d-131">请求</span><span class="sxs-lookup"><span data-stu-id="c014d-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c014d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c014d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/beta/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c014d-133">C#</span><span class="sxs-lookup"><span data-stu-id="c014d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reprocesslicenseassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c014d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c014d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reprocesslicenseassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c014d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c014d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reprocesslicenseassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c014d-136">响应</span><span class="sxs-lookup"><span data-stu-id="c014d-136">Response</span></span>
<span data-ttu-id="c014d-137">响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="c014d-137">The response is the updated user object.</span></span>

><span data-ttu-id="c014d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c014d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "2016-10-19T10:37:00Z",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: reprocessLicenseAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
