---
title: assignLicense
description: 添加或删除用户的许可证，以启用或禁用其对 Microsoft 云产品的使用。 例如，组织可以拥有具有100许可证的 Microsoft 365 企业版 E3 订阅，此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要了解有关订阅和许可证的详细信息，请参阅此 Technet 文章。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2a0baa7aab8cc6e24b6e2e3d5d3c0e294b0f3933
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976623"
---
# <a name="user-assignlicense"></a><span data-ttu-id="06335-106">用户：assignLicense</span><span class="sxs-lookup"><span data-stu-id="06335-106">user: assignLicense</span></span>

<span data-ttu-id="06335-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06335-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06335-108">添加或删除用户的许可证，以启用或禁用其对 Microsoft 云产品的使用。</span><span class="sxs-lookup"><span data-stu-id="06335-108">Add or remove licenses for the user to enable or disable their use of Microsoft cloud offerings.</span></span> <span data-ttu-id="06335-109">例如，组织可以拥有具有100许可证的 Microsoft 365 企业版 E3 订阅，此请求将其中一个许可证分配给特定用户。</span><span class="sxs-lookup"><span data-stu-id="06335-109">For example, an organization can have a Microsoft 365 Enterprise E3 subscription with 100 licenses, and this request assigns one of those licenses to a specific user.</span></span> <span data-ttu-id="06335-110">还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="06335-110">You can also enable and disable specific plans associated with a subscription.</span></span> <span data-ttu-id="06335-111">若要了解有关订阅和许可证的详细信息，请参阅此 [Technet 文章](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings)。</span><span class="sxs-lookup"><span data-stu-id="06335-111">To learn more about subscriptions and licenses, see this [Technet article](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings).</span></span>

<span data-ttu-id="06335-112">若要获取目录中可用的订阅，请执行 [Get subscribedsku 请求](subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="06335-112">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="06335-113">权限</span><span class="sxs-lookup"><span data-stu-id="06335-113">Permissions</span></span>
<span data-ttu-id="06335-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06335-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06335-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="06335-116">Permission type</span></span>      | <span data-ttu-id="06335-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06335-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06335-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06335-118">Delegated (work or school account)</span></span> | <span data-ttu-id="06335-119">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06335-119">User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="06335-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06335-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06335-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="06335-121">Not supported.</span></span>    |
|<span data-ttu-id="06335-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="06335-122">Application</span></span> | <span data-ttu-id="06335-123">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06335-123">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06335-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06335-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="06335-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="06335-125">Request headers</span></span>
| <span data-ttu-id="06335-126">标头</span><span class="sxs-lookup"><span data-stu-id="06335-126">Header</span></span>       | <span data-ttu-id="06335-127">值</span><span class="sxs-lookup"><span data-stu-id="06335-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06335-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="06335-128">Authorization</span></span>  | <span data-ttu-id="06335-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06335-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06335-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06335-131">Content-Type</span></span>  | <span data-ttu-id="06335-132">application/json</span><span class="sxs-lookup"><span data-stu-id="06335-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06335-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="06335-133">Request body</span></span>
<span data-ttu-id="06335-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="06335-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06335-135">参数</span><span class="sxs-lookup"><span data-stu-id="06335-135">Parameter</span></span>    | <span data-ttu-id="06335-136">类型</span><span class="sxs-lookup"><span data-stu-id="06335-136">Type</span></span>   |<span data-ttu-id="06335-137">说明</span><span class="sxs-lookup"><span data-stu-id="06335-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06335-138">addLicenses</span><span class="sxs-lookup"><span data-stu-id="06335-138">addLicenses</span></span>|<span data-ttu-id="06335-139">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="06335-139">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="06335-140">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="06335-140">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="06335-141">您可以通过在 [assignedLicense](../resources/assignedlicense.md)对象上设置 **disabledPlans** 属性来禁用与许可证关联的 servicePlans。</span><span class="sxs-lookup"><span data-stu-id="06335-141">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="06335-142">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="06335-142">removeLicenses</span></span>|<span data-ttu-id="06335-143">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="06335-143">Guid collection</span></span>|<span data-ttu-id="06335-144">标识要删除的许可证的 skuIds 的集合。</span><span class="sxs-lookup"><span data-stu-id="06335-144">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="06335-145">响应</span><span class="sxs-lookup"><span data-stu-id="06335-145">Response</span></span>

<span data-ttu-id="06335-146">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06335-146">If successful, this method returns `200 OK` response code and an updated [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06335-147">示例</span><span class="sxs-lookup"><span data-stu-id="06335-147">Example</span></span>
<span data-ttu-id="06335-148">向用户添加许可证。</span><span class="sxs-lookup"><span data-stu-id="06335-148">Add licenses to the user.</span></span>
##### <a name="request"></a><span data-ttu-id="06335-149">请求</span><span class="sxs-lookup"><span data-stu-id="06335-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06335-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="06335-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[<span data-ttu-id="06335-151">C#</span><span class="sxs-lookup"><span data-stu-id="06335-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06335-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06335-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06335-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06335-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06335-154">Java</span><span class="sxs-lookup"><span data-stu-id="06335-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="example"></a><span data-ttu-id="06335-155">示例</span><span class="sxs-lookup"><span data-stu-id="06335-155">Example</span></span>
<span data-ttu-id="06335-156">删除用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="06335-156">Remove licenses from the user.</span></span>

##### <a name="request"></a><span data-ttu-id="06335-157">请求</span><span class="sxs-lookup"><span data-stu-id="06335-157">Request</span></span>
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json
Content-length: 185

{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```

##### <a name="response"></a><span data-ttu-id="06335-158">响应</span><span class="sxs-lookup"><span data-stu-id="06335-158">Response</span></span>
<span data-ttu-id="06335-159">在这两个示例中，响应是更新的用户对象。</span><span class="sxs-lookup"><span data-stu-id="06335-159">In both examples, the response is the updated user object.</span></span> <span data-ttu-id="06335-160">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06335-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="06335-161">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06335-161">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

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
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
