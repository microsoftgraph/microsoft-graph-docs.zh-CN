---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b339431a995f610214317aa98dd914f598a2ec2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055868"
---
# <a name="get-organization"></a><span data-ttu-id="013b9-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="013b9-103">Get organization</span></span>

<span data-ttu-id="013b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="013b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="013b9-105">获取当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="013b9-105">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="013b9-106">由于 **organization** 资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **organization** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="013b9-106">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="013b9-107">权限</span><span class="sxs-lookup"><span data-stu-id="013b9-107">Permissions</span></span>

<span data-ttu-id="013b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="013b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="013b9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="013b9-110">Permission type</span></span> | <span data-ttu-id="013b9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="013b9-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="013b9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="013b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="013b9-113">User.Read、Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013b9-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="013b9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="013b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="013b9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="013b9-115">Not supported.</span></span> |
|<span data-ttu-id="013b9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="013b9-116">Application</span></span> | <span data-ttu-id="013b9-117">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013b9-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="013b9-118">**注意**：授予 User.Read 权限的应用程序仅能读取组织的 **id**, **displayName** 和 **verifiedDomains** 属性。</span><span class="sxs-lookup"><span data-stu-id="013b9-118">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="013b9-119">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="013b9-119">All other properties will return with `null` values.</span></span> <span data-ttu-id="013b9-120">若要读取所有属性，请使用 Organization.Read.All。</span><span class="sxs-lookup"><span data-stu-id="013b9-120">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="013b9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="013b9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="013b9-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="013b9-122">Optional query parameters</span></span>

<span data-ttu-id="013b9-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="013b9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="013b9-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="013b9-124">Request headers</span></span>

| <span data-ttu-id="013b9-125">名称</span><span class="sxs-lookup"><span data-stu-id="013b9-125">Name</span></span>       | <span data-ttu-id="013b9-126">说明</span><span class="sxs-lookup"><span data-stu-id="013b9-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="013b9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="013b9-127">Authorization</span></span>  | <span data-ttu-id="013b9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="013b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="013b9-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="013b9-130">Request body</span></span>

<span data-ttu-id="013b9-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="013b9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="013b9-132">响应</span><span class="sxs-lookup"><span data-stu-id="013b9-132">Response</span></span>

<span data-ttu-id="013b9-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一个[组织](../resources/organization.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="013b9-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013b9-134">示例</span><span class="sxs-lookup"><span data-stu-id="013b9-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="013b9-135">请求</span><span class="sxs-lookup"><span data-stu-id="013b9-135">Request</span></span>

<span data-ttu-id="013b9-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="013b9-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="013b9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="013b9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[<span data-ttu-id="013b9-138">C#</span><span class="sxs-lookup"><span data-stu-id="013b9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="013b9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="013b9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="013b9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="013b9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="013b9-141">响应</span><span class="sxs-lookup"><span data-stu-id="013b9-141">Response</span></span>

<span data-ttu-id="013b9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="013b9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="013b9-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="013b9-145">See also</span></span>

- [<span data-ttu-id="013b9-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="013b9-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="013b9-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="013b9-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


