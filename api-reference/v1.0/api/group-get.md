---
title: 获取组
description: 获取组对象的属性和关系。
author: Jordanndahl
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 46c50e3ec6d3e646ff4102472687b5bacee3bb1f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682024"
---
# <a name="get-group"></a><span data-ttu-id="50a5b-103">获取组</span><span class="sxs-lookup"><span data-stu-id="50a5b-103">Get group</span></span>

<span data-ttu-id="50a5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50a5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50a5b-105">获取组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50a5b-105">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="50a5b-106">此操作在默认情况下仅返回所有可用属性的一部分，如[属性](../resources/group.md#properties)部分中所示。</span><span class="sxs-lookup"><span data-stu-id="50a5b-106">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="50a5b-107">若要获取 _非_ 默认返回的属性，请在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-107">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="50a5b-108">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="50a5b-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a5b-109">权限</span><span class="sxs-lookup"><span data-stu-id="50a5b-109">Permissions</span></span>
<span data-ttu-id="50a5b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50a5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a5b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="50a5b-112">Permission type</span></span>      | <span data-ttu-id="50a5b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50a5b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50a5b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50a5b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="50a5b-115">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50a5b-115">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="50a5b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50a5b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50a5b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="50a5b-117">Not supported.</span></span>    |
|<span data-ttu-id="50a5b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="50a5b-118">Application</span></span> | <span data-ttu-id="50a5b-119">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a5b-119">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="50a5b-120">**注意：** 根据你尝试访问的组功能，权限可能会受到限制。</span><span class="sxs-lookup"><span data-stu-id="50a5b-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="50a5b-121">有关详细信息，请参阅 [Microsoft Graph 的已知问题](/graph/known-issues)中的[组](/graph/known-issues#groups)部分。</span><span class="sxs-lookup"><span data-stu-id="50a5b-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="50a5b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50a5b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50a5b-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50a5b-123">Optional query parameters</span></span>
<span data-ttu-id="50a5b-124">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="50a5b-125">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="50a5b-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="50a5b-126">请求头</span><span class="sxs-lookup"><span data-stu-id="50a5b-126">Request headers</span></span>
| <span data-ttu-id="50a5b-127">名称</span><span class="sxs-lookup"><span data-stu-id="50a5b-127">Name</span></span>       | <span data-ttu-id="50a5b-128">类型</span><span class="sxs-lookup"><span data-stu-id="50a5b-128">Type</span></span> | <span data-ttu-id="50a5b-129">说明</span><span class="sxs-lookup"><span data-stu-id="50a5b-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50a5b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a5b-130">Authorization</span></span>  | <span data-ttu-id="50a5b-131">string</span><span class="sxs-lookup"><span data-stu-id="50a5b-131">string</span></span>  | <span data-ttu-id="50a5b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50a5b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50a5b-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="50a5b-134">Request body</span></span>
<span data-ttu-id="50a5b-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50a5b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50a5b-136">响应</span><span class="sxs-lookup"><span data-stu-id="50a5b-136">Response</span></span>
<span data-ttu-id="50a5b-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50a5b-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="50a5b-138">除非使用 `$select` 指定特定属性，它会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="50a5b-139">示例</span><span class="sxs-lookup"><span data-stu-id="50a5b-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="50a5b-140">示例 1：返回所有默认属性</span><span class="sxs-lookup"><span data-stu-id="50a5b-140">Example 1: Return all default properties</span></span>

<span data-ttu-id="50a5b-141">返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-141">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="50a5b-142">请求</span><span class="sxs-lookup"><span data-stu-id="50a5b-142">Request</span></span> 

<span data-ttu-id="50a5b-143">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="50a5b-143">The following is an example of a GET request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="50a5b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a5b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```
# <a name="c"></a>[<span data-ttu-id="50a5b-145">C#</span><span class="sxs-lookup"><span data-stu-id="50a5b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50a5b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50a5b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50a5b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50a5b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50a5b-148">Java</span><span class="sxs-lookup"><span data-stu-id="50a5b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50a5b-149">响应</span><span class="sxs-lookup"><span data-stu-id="50a5b-149">Response</span></span>
<span data-ttu-id="50a5b-p106">下面是一个响应示例。它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-p106">The following is an example of the response. It includes only the default properties.</span></span>

><span data-ttu-id="50a5b-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="50a5b-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="50a5b-153">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-153">All the default properties are returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-22T00:51:37Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "groupTypes": [
        "Unified"
    ],
    "mail": "library2@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "smtp:library7423@contoso.com",
        "SMTP:library2@contoso.com"
    ],
    "renewedDateTime": "2018-12-22T00:51:37Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="50a5b-154">示例 2：通过使用 $select 返回其他属性</span><span class="sxs-lookup"><span data-stu-id="50a5b-154">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="50a5b-155">通过使用 `$select` 返回其他属性。</span><span class="sxs-lookup"><span data-stu-id="50a5b-155">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="50a5b-156">请求</span><span class="sxs-lookup"><span data-stu-id="50a5b-156">Request</span></span>

<span data-ttu-id="50a5b-157">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="50a5b-157">The following is an example of a GET request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50a5b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a5b-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[<span data-ttu-id="50a5b-159">C#</span><span class="sxs-lookup"><span data-stu-id="50a5b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50a5b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50a5b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50a5b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50a5b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50a5b-162">Java</span><span class="sxs-lookup"><span data-stu-id="50a5b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50a5b-163">响应</span><span class="sxs-lookup"><span data-stu-id="50a5b-163">Response</span></span>

<span data-ttu-id="50a5b-164">下面是一个包括所请求的非默认属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="50a5b-164">The following is an example of the response which includes the requested non-default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

