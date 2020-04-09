---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Priority
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7283a25bf36ae798d5a2b5a521a67849bd354229
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181607"
---
# <a name="get-organization"></a><span data-ttu-id="fb5ff-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="fb5ff-103">Get organization</span></span>

<span data-ttu-id="fb5ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb5ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb5ff-105">获取当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-105">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="fb5ff-106">由于 **organization** 资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **organization** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-106">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb5ff-107">权限</span><span class="sxs-lookup"><span data-stu-id="fb5ff-107">Permissions</span></span>

<span data-ttu-id="fb5ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb5ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb5ff-110">Permission type</span></span>      | <span data-ttu-id="fb5ff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb5ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb5ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb5ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb5ff-113">User.Read、Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb5ff-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="fb5ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb5ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb5ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-115">Not supported.</span></span>    |
|<span data-ttu-id="fb5ff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb5ff-116">Application</span></span> | <span data-ttu-id="fb5ff-117">Organization.Read.All、Directory.Read.All、Organization.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb5ff-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="fb5ff-118">**注意**：授予 User.Read 权限的应用程序仅能读取组织的 **id**, **displayName** 和 **verifiedDomains** 属性。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-118">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="fb5ff-119">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-119">All other properties will return with `null` values.</span></span> <span data-ttu-id="fb5ff-120">若要读取所有属性，请使用 Organization.Read.All。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-120">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="fb5ff-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb5ff-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb5ff-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fb5ff-122">Optional query parameters</span></span>

<span data-ttu-id="fb5ff-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb5ff-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb5ff-124">Request headers</span></span>

| <span data-ttu-id="fb5ff-125">名称</span><span class="sxs-lookup"><span data-stu-id="fb5ff-125">Name</span></span>       | <span data-ttu-id="fb5ff-126">说明</span><span class="sxs-lookup"><span data-stu-id="fb5ff-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="fb5ff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb5ff-127">Authorization</span></span>  | <span data-ttu-id="fb5ff-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb5ff-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb5ff-130">Request body</span></span>

<span data-ttu-id="fb5ff-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb5ff-132">响应</span><span class="sxs-lookup"><span data-stu-id="fb5ff-132">Response</span></span>

<span data-ttu-id="fb5ff-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一个[组织](../resources/organization.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb5ff-134">示例</span><span class="sxs-lookup"><span data-stu-id="fb5ff-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fb5ff-135">请求</span><span class="sxs-lookup"><span data-stu-id="fb5ff-135">Request</span></span>

<span data-ttu-id="fb5ff-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb5ff-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb5ff-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="fb5ff-138">C#</span><span class="sxs-lookup"><span data-stu-id="fb5ff-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb5ff-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb5ff-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb5ff-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb5ff-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb5ff-141">Java</span><span class="sxs-lookup"><span data-stu-id="fb5ff-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fb5ff-142">响应</span><span class="sxs-lookup"><span data-stu-id="fb5ff-142">Response</span></span>

<span data-ttu-id="fb5ff-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb5ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
