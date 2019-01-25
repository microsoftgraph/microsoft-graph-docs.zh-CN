---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0313fb5912d8cc9e12319fafac518becfee105a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520079"
---
# <a name="get-organization"></a><span data-ttu-id="77de7-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="77de7-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77de7-104">检索当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77de7-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="77de7-105">由于**组织**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**组织**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="77de7-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="77de7-106">权限</span><span class="sxs-lookup"><span data-stu-id="77de7-106">Permissions</span></span>

<span data-ttu-id="77de7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77de7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77de7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="77de7-109">Permission type</span></span> | <span data-ttu-id="77de7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77de7-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77de7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77de7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77de7-112">User.Read、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="77de7-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="77de7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77de7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77de7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="77de7-114">Not supported.</span></span> |
|<span data-ttu-id="77de7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="77de7-115">Application</span></span> | <span data-ttu-id="77de7-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="77de7-116">Directory.Read.All</span></span> |

> <span data-ttu-id="77de7-117">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="77de7-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="77de7-118">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="77de7-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="77de7-119">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="77de7-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="77de7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77de7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77de7-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77de7-121">Optional query parameters</span></span>

<span data-ttu-id="77de7-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77de7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77de7-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="77de7-123">Request headers</span></span>

| <span data-ttu-id="77de7-124">名称</span><span class="sxs-lookup"><span data-stu-id="77de7-124">Name</span></span>       | <span data-ttu-id="77de7-125">类型</span><span class="sxs-lookup"><span data-stu-id="77de7-125">Type</span></span> | <span data-ttu-id="77de7-126">说明</span><span class="sxs-lookup"><span data-stu-id="77de7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="77de7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="77de7-127">Authorization</span></span>  | <span data-ttu-id="77de7-128">string</span><span class="sxs-lookup"><span data-stu-id="77de7-128">string</span></span>  | <span data-ttu-id="77de7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77de7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77de7-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="77de7-131">Request body</span></span>

<span data-ttu-id="77de7-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77de7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77de7-133">响应</span><span class="sxs-lookup"><span data-stu-id="77de7-133">Response</span></span>

<span data-ttu-id="77de7-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77de7-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77de7-135">示例</span><span class="sxs-lookup"><span data-stu-id="77de7-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="77de7-136">请求</span><span class="sxs-lookup"><span data-stu-id="77de7-136">Request</span></span>

<span data-ttu-id="77de7-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77de7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="77de7-138">响应</span><span class="sxs-lookup"><span data-stu-id="77de7-138">Response</span></span>

<span data-ttu-id="77de7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77de7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="77de7-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="77de7-142">See also</span></span>

- [<span data-ttu-id="77de7-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="77de7-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="77de7-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="77de7-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/organization-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
