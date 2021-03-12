---
title: user： reprocessLicenseAssignment
description: 重新处理用户的所有基于组的许可证分配。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e3b20fa97bddcc9d5dbab674e1a5af24a2e15f8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720709"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="143e0-103">user： reprocessLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="143e0-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="143e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="143e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="143e0-105">重新处理用户的所有基于组的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="143e0-105">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="143e0-106">若要了解有关基于组的许可的信息，请参阅什么是 [Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)中基于组的许可。</span><span class="sxs-lookup"><span data-stu-id="143e0-106">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="143e0-107">另请参阅 [标识并解决 Azure Active Directory](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) 中组的许可证分配问题了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="143e0-107">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="143e0-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="143e0-108">Permissions</span></span>
<span data-ttu-id="143e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="143e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="143e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="143e0-111">Permission type</span></span>      | <span data-ttu-id="143e0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="143e0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="143e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="143e0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="143e0-114">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="143e0-114">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="143e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="143e0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="143e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="143e0-116">Not supported.</span></span>    |
|<span data-ttu-id="143e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="143e0-117">Application</span></span> | <span data-ttu-id="143e0-118">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="143e0-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="143e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="143e0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="143e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="143e0-120">Request headers</span></span>
| <span data-ttu-id="143e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="143e0-121">Header</span></span>       | <span data-ttu-id="143e0-122">值</span><span class="sxs-lookup"><span data-stu-id="143e0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="143e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="143e0-123">Authorization</span></span>  | <span data-ttu-id="143e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="143e0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="143e0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="143e0-126">Request body</span></span>
<span data-ttu-id="143e0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="143e0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="143e0-128">响应</span><span class="sxs-lookup"><span data-stu-id="143e0-128">Response</span></span>

<span data-ttu-id="143e0-129">如果成功，此方法在 `200 OK` 响应正文中返回 响应[](../resources/user.md)代码和更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="143e0-129">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="143e0-130">示例</span><span class="sxs-lookup"><span data-stu-id="143e0-130">Example</span></span>
<span data-ttu-id="143e0-131">以下示例演示如何重新处理用户的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="143e0-131">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="143e0-132">请求</span><span class="sxs-lookup"><span data-stu-id="143e0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="143e0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="143e0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```
# <a name="c"></a>[<span data-ttu-id="143e0-134">C#</span><span class="sxs-lookup"><span data-stu-id="143e0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reprocesslicenseassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="143e0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="143e0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reprocesslicenseassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="143e0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="143e0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reprocesslicenseassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="143e0-137">Java</span><span class="sxs-lookup"><span data-stu-id="143e0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reprocesslicenseassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="143e0-138">响应</span><span class="sxs-lookup"><span data-stu-id="143e0-138">Response</span></span>

<span data-ttu-id="143e0-139">响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="143e0-139">The response is the updated user object.</span></span>

><span data-ttu-id="143e0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="143e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
