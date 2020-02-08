---
title: 用户： reprocessLicenseAssignment
description: 重新处理用户的所有基于组的许可证分配。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9136931b08a2e86f582a0272a6be214740562e4b
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865768"
---
# <a name="user-reprocesslicenseassignment"></a><span data-ttu-id="25540-103">用户： reprocessLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="25540-103">user: reprocessLicenseAssignment</span></span>

<span data-ttu-id="25540-104">重新处理用户的所有基于组的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="25540-104">Reprocess all group-based license assignments for the user.</span></span> <span data-ttu-id="25540-105">若要了解有关基于组的许可的详细信息，请参阅[什么是 Azure Active Directory 中的基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="25540-105">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span> <span data-ttu-id="25540-106">有关更多详细信息，请参阅[识别和解决 Azure Active Directory 中的组的许可证分配问题](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。</span><span class="sxs-lookup"><span data-stu-id="25540-106">Also see [Identify and resolve license assignment problems for a group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems) for more details.</span></span>


## <a name="permissions"></a><span data-ttu-id="25540-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="25540-107">Permissions</span></span>
<span data-ttu-id="25540-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25540-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25540-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25540-110">Permission type</span></span>      | <span data-ttu-id="25540-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25540-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25540-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25540-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25540-113">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25540-113">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="25540-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25540-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25540-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25540-115">Not supported.</span></span>    |
|<span data-ttu-id="25540-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25540-116">Application</span></span> | <span data-ttu-id="25540-117">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25540-117">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25540-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25540-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/reprocessLicenseAssignment

```
## <a name="request-headers"></a><span data-ttu-id="25540-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25540-119">Request headers</span></span>
| <span data-ttu-id="25540-120">标头</span><span class="sxs-lookup"><span data-stu-id="25540-120">Header</span></span>       | <span data-ttu-id="25540-121">值</span><span class="sxs-lookup"><span data-stu-id="25540-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25540-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25540-122">Authorization</span></span>  | <span data-ttu-id="25540-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25540-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25540-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="25540-125">Request body</span></span>
<span data-ttu-id="25540-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25540-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25540-127">响应</span><span class="sxs-lookup"><span data-stu-id="25540-127">Response</span></span>

<span data-ttu-id="25540-128">如果成功，此方法在`200 OK`响应正文中返回响应代码和更新的[user](../resources/user.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25540-128">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25540-129">示例</span><span class="sxs-lookup"><span data-stu-id="25540-129">Example</span></span>
<span data-ttu-id="25540-130">下面的示例展示了如何重新处理用户的许可证分配。</span><span class="sxs-lookup"><span data-stu-id="25540-130">The following example shows how to reprocess license assignments for the user.</span></span>
### <a name="request"></a><span data-ttu-id="25540-131">请求</span><span class="sxs-lookup"><span data-stu-id="25540-131">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="25540-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="25540-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reprocessLicenseAssignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/047dd774-f1c4-40f2-82f0-278de79f9b83/reprocessLicenseAssignment

```

### <a name="response"></a><span data-ttu-id="25540-133">响应</span><span class="sxs-lookup"><span data-stu-id="25540-133">Response</span></span>

<span data-ttu-id="25540-134">响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="25540-134">The response is the updated user object.</span></span>

><span data-ttu-id="25540-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="25540-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
