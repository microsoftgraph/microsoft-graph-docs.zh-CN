---
title: 获取组
description: 获取组对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8455985891701e0d1a9fd1062eebc648375c0a2a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502405"
---
# <a name="get-group"></a><span data-ttu-id="cc4b2-103">获取组</span><span class="sxs-lookup"><span data-stu-id="cc4b2-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc4b2-104">获取 [group](../resources/group.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="cc4b2-105">此操作在默认情况下仅返回所有可用属性的一部分，如[属性](../resources/group.md#properties)部分中所示。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="cc4b2-106">若要获取_非_默认返回的属性，请在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="cc4b2-107">请参阅 `$select` 的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="cc4b2-108">**hasMembersWithLicenseErrors** 属性是例外。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="cc4b2-109">请参阅关于如何使用此属性的[示例](group-list.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="cc4b2-110">由于**组**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**组**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-110">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **user** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc4b2-111">权限</span><span class="sxs-lookup"><span data-stu-id="cc4b2-111">Permissions</span></span>
<span data-ttu-id="cc4b2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc4b2-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc4b2-114">Permission type</span></span>      | <span data-ttu-id="cc4b2-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc4b2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc4b2-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc4b2-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cc4b2-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc4b2-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc4b2-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc4b2-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc4b2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-119">Not supported.</span></span>    |
|<span data-ttu-id="cc4b2-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc4b2-120">Application</span></span> | <span data-ttu-id="cc4b2-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc4b2-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc4b2-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc4b2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc4b2-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc4b2-123">Optional query parameters</span></span>
<span data-ttu-id="cc4b2-124">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="cc4b2-125">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-125">See an [example](#request-2) below.</span></span>

<span data-ttu-id="cc4b2-126">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-126">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc4b2-127">请求头</span><span class="sxs-lookup"><span data-stu-id="cc4b2-127">Request headers</span></span>
| <span data-ttu-id="cc4b2-128">名称</span><span class="sxs-lookup"><span data-stu-id="cc4b2-128">Name</span></span>       | <span data-ttu-id="cc4b2-129">类型</span><span class="sxs-lookup"><span data-stu-id="cc4b2-129">Type</span></span> | <span data-ttu-id="cc4b2-130">说明</span><span class="sxs-lookup"><span data-stu-id="cc4b2-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc4b2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc4b2-131">Authorization</span></span>  | <span data-ttu-id="cc4b2-132">string</span><span class="sxs-lookup"><span data-stu-id="cc4b2-132">string</span></span>  | <span data-ttu-id="cc4b2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc4b2-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc4b2-135">Request body</span></span>
<span data-ttu-id="cc4b2-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc4b2-137">响应</span><span class="sxs-lookup"><span data-stu-id="cc4b2-137">Response</span></span>
<span data-ttu-id="cc4b2-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-138">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="cc4b2-139">除非使用 `$select` 指定特定属性，它会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-139">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="cc4b2-140">示例</span><span class="sxs-lookup"><span data-stu-id="cc4b2-140">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="cc4b2-141">请求 1</span><span class="sxs-lookup"><span data-stu-id="cc4b2-141">Request 1</span></span>
<span data-ttu-id="cc4b2-142">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="cc4b2-143">响应 1</span><span class="sxs-lookup"><span data-stu-id="cc4b2-143">Response 1</span></span>
<span data-ttu-id="cc4b2-144">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-144">The following is an example of the response.</span></span> <span data-ttu-id="cc4b2-145">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-145">It includes only the default properties.</span></span>

><span data-ttu-id="cc4b2-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cc4b2-147">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-147">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="cc4b2-148">请求 2</span><span class="sxs-lookup"><span data-stu-id="cc4b2-148">Request 2</span></span>
<span data-ttu-id="cc4b2-149">下一个示例使用 `$select` 查询选项获取非默认返回的一些属性。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-149">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="cc4b2-150">响应 2</span><span class="sxs-lookup"><span data-stu-id="cc4b2-150">Response 2</span></span>
<span data-ttu-id="cc4b2-151">下面是一个包括所请求的非默认属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc4b2-151">The following is an example of the response which includes the requested non-default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="cc4b2-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="cc4b2-152">See also</span></span>

- [<span data-ttu-id="cc4b2-153">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="cc4b2-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cc4b2-154">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="cc4b2-154">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cc4b2-155">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="cc4b2-155">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
