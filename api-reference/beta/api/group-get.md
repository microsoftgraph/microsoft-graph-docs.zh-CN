---
title: 获取组
description: 获取组对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 18eb80938247d56326620a6ac866073acad6f715
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353074"
---
# <a name="get-group"></a><span data-ttu-id="bff7e-103">获取组</span><span class="sxs-lookup"><span data-stu-id="bff7e-103">Get group</span></span>

> <span data-ttu-id="bff7e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bff7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bff7e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bff7e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bff7e-106">获取 [group](../resources/group.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bff7e-106">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="bff7e-107">此操作在默认情况下仅返回所有可用属性的一部分，如[属性](../resources/group.md#properties)部分中所示。</span><span class="sxs-lookup"><span data-stu-id="bff7e-107">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="bff7e-108">若要获取_非_默认返回的属性，请在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-108">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="bff7e-109">请参阅 `$select` 的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="bff7e-109">See an [example](#request-2).</span></span> <span data-ttu-id="bff7e-110">**hasMembersWithLicenseErrors** 属性是例外。</span><span class="sxs-lookup"><span data-stu-id="bff7e-110">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="bff7e-111">请参阅关于如何使用此属性的[示例](group-list.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="bff7e-111">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="bff7e-112">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**组**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="bff7e-112">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="bff7e-113">权限</span><span class="sxs-lookup"><span data-stu-id="bff7e-113">Permissions</span></span>
<span data-ttu-id="bff7e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bff7e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bff7e-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="bff7e-116">Permission type</span></span>      | <span data-ttu-id="bff7e-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bff7e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bff7e-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bff7e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="bff7e-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff7e-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bff7e-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bff7e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bff7e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="bff7e-121">Not supported.</span></span>    |
|<span data-ttu-id="bff7e-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="bff7e-122">Application</span></span> | <span data-ttu-id="bff7e-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff7e-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bff7e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bff7e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bff7e-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bff7e-125">Optional query parameters</span></span>
<span data-ttu-id="bff7e-126">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-126">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="bff7e-127">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="bff7e-127">See an [example](#request-2) below.</span></span>

<span data-ttu-id="bff7e-128">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bff7e-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bff7e-129">请求头</span><span class="sxs-lookup"><span data-stu-id="bff7e-129">Request headers</span></span>
| <span data-ttu-id="bff7e-130">名称</span><span class="sxs-lookup"><span data-stu-id="bff7e-130">Name</span></span>       | <span data-ttu-id="bff7e-131">类型</span><span class="sxs-lookup"><span data-stu-id="bff7e-131">Type</span></span> | <span data-ttu-id="bff7e-132">说明</span><span class="sxs-lookup"><span data-stu-id="bff7e-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bff7e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="bff7e-133">Authorization</span></span>  | <span data-ttu-id="bff7e-134">string</span><span class="sxs-lookup"><span data-stu-id="bff7e-134">string</span></span>  | <span data-ttu-id="bff7e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bff7e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bff7e-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="bff7e-137">Request body</span></span>
<span data-ttu-id="bff7e-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bff7e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bff7e-139">响应</span><span class="sxs-lookup"><span data-stu-id="bff7e-139">Response</span></span>
<span data-ttu-id="bff7e-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bff7e-140">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="bff7e-141">除非使用 `$select` 指定特定属性，它会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-141">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="bff7e-142">示例</span><span class="sxs-lookup"><span data-stu-id="bff7e-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="bff7e-143">请求 1</span><span class="sxs-lookup"><span data-stu-id="bff7e-143">Request 1</span></span>
<span data-ttu-id="bff7e-144">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="bff7e-144">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="bff7e-145">响应 1</span><span class="sxs-lookup"><span data-stu-id="bff7e-145">Response 1</span></span>
<span data-ttu-id="bff7e-146">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="bff7e-146">The following is an example of the response.</span></span> <span data-ttu-id="bff7e-147">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-147">It includes only the default properties.</span></span>

><span data-ttu-id="bff7e-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bff7e-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bff7e-149">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-149">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="bff7e-150">请求 2</span><span class="sxs-lookup"><span data-stu-id="bff7e-150">Request 2</span></span>
<span data-ttu-id="bff7e-151">下一个示例使用 `$select` 查询选项获取非默认返回的一些属性。</span><span class="sxs-lookup"><span data-stu-id="bff7e-151">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="bff7e-152">响应 2</span><span class="sxs-lookup"><span data-stu-id="bff7e-152">Response 2</span></span>
<span data-ttu-id="bff7e-153">下面是一个包括所请求的非默认属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="bff7e-153">The following is an example of the response which includes the requested non-default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bff7e-154">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bff7e-154">See also</span></span>

- [<span data-ttu-id="bff7e-155">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bff7e-155">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bff7e-156">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bff7e-156">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bff7e-157">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bff7e-157">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
