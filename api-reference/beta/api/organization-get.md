---
title: 获取组织
description: 检索当前经过身份验证的组织的属性和关系。
ms.openlocfilehash: f3d2ca5c6881a06f397101a0050fe29f8a646614
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748281"
---
# <a name="get-organization"></a><span data-ttu-id="2c2df-103">获取组织</span><span class="sxs-lookup"><span data-stu-id="2c2df-103">Get organization</span></span>

> <span data-ttu-id="2c2df-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2c2df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c2df-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c2df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c2df-106">检索当前经过身份验证的组织的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2c2df-106">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="2c2df-107">由于**组织**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**组织**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="2c2df-107">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c2df-108">权限</span><span class="sxs-lookup"><span data-stu-id="2c2df-108">Permissions</span></span>

<span data-ttu-id="2c2df-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c2df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c2df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c2df-111">Permission type</span></span> | <span data-ttu-id="2c2df-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c2df-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c2df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c2df-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c2df-114">User.Read、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c2df-114">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="2c2df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c2df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c2df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c2df-116">Not supported.</span></span> |
|<span data-ttu-id="2c2df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c2df-117">Application</span></span> | <span data-ttu-id="2c2df-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c2df-118">Directory.Read.All</span></span> |

> <span data-ttu-id="2c2df-119">注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。</span><span class="sxs-lookup"><span data-stu-id="2c2df-119">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="2c2df-120">所有其他属性将返回 `null` 值。</span><span class="sxs-lookup"><span data-stu-id="2c2df-120">All other properties will return with `null` values.</span></span> <span data-ttu-id="2c2df-121">若要读取所有属性，请使用 Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="2c2df-121">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="2c2df-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c2df-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c2df-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c2df-123">Optional query parameters</span></span>

<span data-ttu-id="2c2df-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c2df-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c2df-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c2df-125">Request headers</span></span>

| <span data-ttu-id="2c2df-126">名称</span><span class="sxs-lookup"><span data-stu-id="2c2df-126">Name</span></span>       | <span data-ttu-id="2c2df-127">类型</span><span class="sxs-lookup"><span data-stu-id="2c2df-127">Type</span></span> | <span data-ttu-id="2c2df-128">说明</span><span class="sxs-lookup"><span data-stu-id="2c2df-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c2df-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c2df-129">Authorization</span></span>  | <span data-ttu-id="2c2df-130">string</span><span class="sxs-lookup"><span data-stu-id="2c2df-130">string</span></span>  | <span data-ttu-id="2c2df-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c2df-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c2df-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c2df-133">Request body</span></span>

<span data-ttu-id="2c2df-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c2df-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c2df-135">响应</span><span class="sxs-lookup"><span data-stu-id="2c2df-135">Response</span></span>

<span data-ttu-id="2c2df-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c2df-136">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c2df-137">示例</span><span class="sxs-lookup"><span data-stu-id="2c2df-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2c2df-138">请求</span><span class="sxs-lookup"><span data-stu-id="2c2df-138">Request</span></span>

<span data-ttu-id="2c2df-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c2df-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="2c2df-140">响应</span><span class="sxs-lookup"><span data-stu-id="2c2df-140">Response</span></span>

<span data-ttu-id="2c2df-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c2df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2c2df-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2c2df-144">See also</span></span>

- [<span data-ttu-id="2c2df-145">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2c2df-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2c2df-146">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="2c2df-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->