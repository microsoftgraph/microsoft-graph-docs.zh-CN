---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e0105a5a81a754beab637fe2199dd7e5bf5d6a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450567"
---
# <a name="get-organization"></a><span data-ttu-id="45e7f-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="45e7f-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e7f-104">检索当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45e7f-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="45e7f-105">由于**组织**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用操作`GET`来获取**组织**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="45e7f-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="45e7f-106">权限</span><span class="sxs-lookup"><span data-stu-id="45e7f-106">Permissions</span></span>

<span data-ttu-id="45e7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45e7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e7f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45e7f-109">Permission type</span></span> | <span data-ttu-id="45e7f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45e7f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45e7f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45e7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45e7f-112">Read、目录。所有</span><span class="sxs-lookup"><span data-stu-id="45e7f-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="45e7f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45e7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45e7f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45e7f-114">Not supported.</span></span> |
|<span data-ttu-id="45e7f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45e7f-115">Application</span></span> | <span data-ttu-id="45e7f-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="45e7f-116">Directory.Read.All</span></span> |

> <span data-ttu-id="45e7f-117">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="45e7f-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="45e7f-118">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="45e7f-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="45e7f-119">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="45e7f-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="45e7f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45e7f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45e7f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="45e7f-121">Optional query parameters</span></span>

<span data-ttu-id="45e7f-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45e7f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45e7f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="45e7f-123">Request headers</span></span>

| <span data-ttu-id="45e7f-124">名称</span><span class="sxs-lookup"><span data-stu-id="45e7f-124">Name</span></span>       | <span data-ttu-id="45e7f-125">类型</span><span class="sxs-lookup"><span data-stu-id="45e7f-125">Type</span></span> | <span data-ttu-id="45e7f-126">说明</span><span class="sxs-lookup"><span data-stu-id="45e7f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45e7f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="45e7f-127">Authorization</span></span>  | <span data-ttu-id="45e7f-128">string</span><span class="sxs-lookup"><span data-stu-id="45e7f-128">string</span></span>  | <span data-ttu-id="45e7f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45e7f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45e7f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="45e7f-131">Request body</span></span>

<span data-ttu-id="45e7f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45e7f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e7f-133">响应</span><span class="sxs-lookup"><span data-stu-id="45e7f-133">Response</span></span>

<span data-ttu-id="45e7f-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="45e7f-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45e7f-135">示例</span><span class="sxs-lookup"><span data-stu-id="45e7f-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="45e7f-136">请求</span><span class="sxs-lookup"><span data-stu-id="45e7f-136">Request</span></span>

<span data-ttu-id="45e7f-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45e7f-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="45e7f-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="45e7f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45e7f-139">C#</span><span class="sxs-lookup"><span data-stu-id="45e7f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45e7f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="45e7f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45e7f-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="45e7f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="45e7f-142">响应</span><span class="sxs-lookup"><span data-stu-id="45e7f-142">Response</span></span>

<span data-ttu-id="45e7f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45e7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="45e7f-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="45e7f-146">See also</span></span>

- [<span data-ttu-id="45e7f-147">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="45e7f-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="45e7f-148">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="45e7f-148">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
