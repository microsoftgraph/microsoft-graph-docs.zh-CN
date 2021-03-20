---
title: 获取组
description: 获取组对象的属性和关系。
author: yyuank
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8578083aecaeb34f838bcffad80be4e4c742fe2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961805"
---
# <a name="get-group"></a><span data-ttu-id="e8415-103">获取组</span><span class="sxs-lookup"><span data-stu-id="e8415-103">Get group</span></span>

<span data-ttu-id="e8415-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8415-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8415-105">获取 [group](../resources/group.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e8415-105">Get the properties and relationships of a [group](../resources/group.md) object.</span></span> 

<span data-ttu-id="e8415-106">此操作在默认情况下仅返回所有可用属性的一部分，如[属性](../resources/group.md#properties)部分中所示。</span><span class="sxs-lookup"><span data-stu-id="e8415-106">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="e8415-107">若要获取 _非_ 默认返回的属性，请在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="e8415-107">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="e8415-108">**hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。</span><span class="sxs-lookup"><span data-stu-id="e8415-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span> <span data-ttu-id="e8415-109">由于 **组** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **组** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="e8415-109">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8415-110">权限</span><span class="sxs-lookup"><span data-stu-id="e8415-110">Permissions</span></span>
<span data-ttu-id="e8415-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8415-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8415-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8415-113">Permission type</span></span>      | <span data-ttu-id="e8415-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8415-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8415-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8415-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e8415-116">GroupMember.Read.All、Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8415-116">GroupMember.Read.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e8415-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8415-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8415-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8415-118">Not supported.</span></span>    |
|<span data-ttu-id="e8415-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8415-119">Application</span></span> | <span data-ttu-id="e8415-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8415-120">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="e8415-121">**注意：** 根据你尝试访问的组功能，权限可能会受到限制。</span><span class="sxs-lookup"><span data-stu-id="e8415-121">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="e8415-122">有关详细信息，请参阅 [Microsoft Graph 的已知问题](/graph/known-issues)中的[组](/graph/known-issues#groups)部分。</span><span class="sxs-lookup"><span data-stu-id="e8415-122">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="e8415-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8415-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8415-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8415-124">Optional query parameters</span></span>
<span data-ttu-id="e8415-125">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="e8415-125">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="e8415-126">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e8415-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8415-127">请求头</span><span class="sxs-lookup"><span data-stu-id="e8415-127">Request headers</span></span>
| <span data-ttu-id="e8415-128">名称</span><span class="sxs-lookup"><span data-stu-id="e8415-128">Name</span></span>       | <span data-ttu-id="e8415-129">类型</span><span class="sxs-lookup"><span data-stu-id="e8415-129">Type</span></span> | <span data-ttu-id="e8415-130">说明</span><span class="sxs-lookup"><span data-stu-id="e8415-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e8415-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8415-131">Authorization</span></span>  | <span data-ttu-id="e8415-132">string</span><span class="sxs-lookup"><span data-stu-id="e8415-132">string</span></span>  | <span data-ttu-id="e8415-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8415-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8415-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8415-135">Request body</span></span>
<span data-ttu-id="e8415-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8415-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8415-137">响应</span><span class="sxs-lookup"><span data-stu-id="e8415-137">Response</span></span>
<span data-ttu-id="e8415-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8415-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e8415-139">除非使用 `$select` 指定特定属性，它会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="e8415-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="e8415-140">示例</span><span class="sxs-lookup"><span data-stu-id="e8415-140">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="e8415-141">示例 1：返回所有默认属性</span><span class="sxs-lookup"><span data-stu-id="e8415-141">Example 1: Return all default properties</span></span>

#### <a name="request"></a><span data-ttu-id="e8415-142">请求</span><span class="sxs-lookup"><span data-stu-id="e8415-142">Request</span></span>

<span data-ttu-id="e8415-143">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8415-143">The following is an example of a GET request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="e8415-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8415-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```
# <a name="c"></a>[<span data-ttu-id="e8415-145">C#</span><span class="sxs-lookup"><span data-stu-id="e8415-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8415-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8415-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8415-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8415-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8415-148">Java</span><span class="sxs-lookup"><span data-stu-id="e8415-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e8415-149">响应</span><span class="sxs-lookup"><span data-stu-id="e8415-149">Response</span></span>
<span data-ttu-id="e8415-150">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8415-150">The following is an example of the response.</span></span> <span data-ttu-id="e8415-151">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="e8415-151">It includes only the default properties.</span></span>

><span data-ttu-id="e8415-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8415-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8415-153">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="e8415-153">All the default properties are returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_1"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-12-22T02:21:05Z",
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "expirationDateTime": null,
  "groupTypes": [
      "Unified"
  ],
  "isAssignableToRole": null,
  "mail": "golfassist@contoso.com",
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
  "onPremisesLastSyncDateTime": null,
  "onPremisesSecurityIdentifier": null,
  "onPremisesSyncEnabled": null,
  "preferredDataLocation": "CAN",
  "preferredLanguage": null,
  "proxyAddresses": [
      "smtp:golfassist@contoso.onmicrosoft.com",
      "SMTP:golfassist@contoso.com"
  ],
  "renewedDateTime": "2018-12-22T02:21:05Z",
  "resourceBehaviorOptions": [],
  "resourceProvisioningOptions": [],
  "securityEnabled": false,
  "theme": null,
  "visibility": "Public",
  "onPremisesProvisioningErrors": []
}
```


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="e8415-154">示例 2：通过使用 $select 返回其他属性</span><span class="sxs-lookup"><span data-stu-id="e8415-154">Example 2: Return additional properties by using $select</span></span>

#### <a name="request"></a><span data-ttu-id="e8415-155">请求</span><span class="sxs-lookup"><span data-stu-id="e8415-155">Request</span></span>

<span data-ttu-id="e8415-156">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8415-156">The following is an example of a GET request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="e8415-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8415-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="c"></a>[<span data-ttu-id="e8415-158">C#</span><span class="sxs-lookup"><span data-stu-id="e8415-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8415-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8415-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8415-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8415-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8415-161">Java</span><span class="sxs-lookup"><span data-stu-id="e8415-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e8415-162">响应</span><span class="sxs-lookup"><span data-stu-id="e8415-162">Response</span></span>

<span data-ttu-id="e8415-163">下面是一个包括所请求的非默认属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8415-163">The following is an example of the response which includes the requested non-default properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```
### <a name="example-3-read-a-specific-dynamic-group"></a><span data-ttu-id="e8415-164">示例 3：读取特定动态组</span><span class="sxs-lookup"><span data-stu-id="e8415-164">Example 3: Read a specific dynamic group</span></span>

#### <a name="request"></a><span data-ttu-id="e8415-165">请求</span><span class="sxs-lookup"><span data-stu-id="e8415-165">Request</span></span>

<span data-ttu-id="e8415-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8415-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["1cdf9c18-a7dc-46b1-b47f-094d5656376d"],
  "name": "get_dynamic_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/1cdf9c18-a7dc-46b1-b47f-094d5656376d?$select=id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus
```

#### <a name="response"></a><span data-ttu-id="e8415-167">响应</span><span class="sxs-lookup"><span data-stu-id="e8415-167">Response</span></span>

<span data-ttu-id="e8415-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8415-168">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus)/$entity",
  "id": "1cdf9c18-a7dc-46b1-b47f-094d5656376d",
  "membershipRule": "accountEnabled eq true",
  "membershipRuleProcessingState": "On",
  "membershipRuleProcessingStatus": {
    "status" : "NotStarted",
    "lastMembershipUpdated"  : null,
    "errorMessage" : null
  }
}
```

## <a name="see-also"></a><span data-ttu-id="e8415-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e8415-169">See also</span></span>

- [<span data-ttu-id="e8415-170">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e8415-170">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e8415-171">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e8415-171">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e8415-172">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e8415-172">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


