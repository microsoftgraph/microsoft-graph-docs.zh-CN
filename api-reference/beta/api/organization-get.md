---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: befd5692cf2d1600d1e54049eda131514b5dbf88
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725995"
---
# <a name="get-organization"></a><span data-ttu-id="31eed-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="31eed-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31eed-104">获取当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31eed-104">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="31eed-105">由于**组织**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用操作`GET`来获取**组织**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="31eed-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="31eed-106">权限</span><span class="sxs-lookup"><span data-stu-id="31eed-106">Permissions</span></span>

<span data-ttu-id="31eed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31eed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31eed-109">Permission type</span></span> | <span data-ttu-id="31eed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31eed-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31eed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31eed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31eed-112">读取、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、读写。所有</span><span class="sxs-lookup"><span data-stu-id="31eed-112">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="31eed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31eed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31eed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31eed-114">Not supported.</span></span> |
|<span data-ttu-id="31eed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31eed-115">Application</span></span> | <span data-ttu-id="31eed-116">全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="31eed-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="31eed-117">**注意**: 授予用户的应用程序。读取权限只能读取组织的**id**、 **displayName**和**verifiedDomains**属性。</span><span class="sxs-lookup"><span data-stu-id="31eed-117">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="31eed-118">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="31eed-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="31eed-119">若要读取所有属性, 请使用组织关系。</span><span class="sxs-lookup"><span data-stu-id="31eed-119">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="31eed-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31eed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31eed-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31eed-121">Optional query parameters</span></span>

<span data-ttu-id="31eed-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31eed-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31eed-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="31eed-123">Request headers</span></span>

| <span data-ttu-id="31eed-124">名称</span><span class="sxs-lookup"><span data-stu-id="31eed-124">Name</span></span>       | <span data-ttu-id="31eed-125">说明</span><span class="sxs-lookup"><span data-stu-id="31eed-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="31eed-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="31eed-126">Authorization</span></span>  | <span data-ttu-id="31eed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31eed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31eed-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="31eed-129">Request body</span></span>

<span data-ttu-id="31eed-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31eed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31eed-131">响应</span><span class="sxs-lookup"><span data-stu-id="31eed-131">Response</span></span>

<span data-ttu-id="31eed-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31eed-132">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31eed-133">示例</span><span class="sxs-lookup"><span data-stu-id="31eed-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="31eed-134">请求</span><span class="sxs-lookup"><span data-stu-id="31eed-134">Request</span></span>

<span data-ttu-id="31eed-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31eed-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31eed-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="31eed-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="31eed-137">C#</span><span class="sxs-lookup"><span data-stu-id="31eed-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31eed-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31eed-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31eed-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="31eed-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="31eed-140">响应</span><span class="sxs-lookup"><span data-stu-id="31eed-140">Response</span></span>

<span data-ttu-id="31eed-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31eed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="31eed-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31eed-144">See also</span></span>

- [<span data-ttu-id="31eed-145">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="31eed-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="31eed-146">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="31eed-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
