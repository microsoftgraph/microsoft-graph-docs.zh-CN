---
title: 获取组
description: 获取组对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: edf1b53beaf519e86669e7ea8a472ea1562766af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572673"
---
# <a name="get-group"></a><span data-ttu-id="f7441-103">获取组</span><span class="sxs-lookup"><span data-stu-id="f7441-103">Get group</span></span>
<span data-ttu-id="f7441-104">获取组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7441-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="f7441-105">此操作在默认情况下仅返回所有可用属性的一部分，如[属性](../resources/group.md#properties)部分中所示。</span><span class="sxs-lookup"><span data-stu-id="f7441-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="f7441-106">若要获取_非_默认返回的属性，请在 `$select` OData 查询选项中指定这些属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="f7441-107">请参阅 `$select` 的[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="f7441-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="f7441-108">**hasMembersWithLicenseErrors** 属性是例外。</span><span class="sxs-lookup"><span data-stu-id="f7441-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="f7441-109">请参阅关于如何使用此属性的[示例](group-list.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="f7441-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7441-110">权限</span><span class="sxs-lookup"><span data-stu-id="f7441-110">Permissions</span></span>
<span data-ttu-id="f7441-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7441-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7441-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7441-113">Permission type</span></span>      | <span data-ttu-id="f7441-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7441-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7441-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7441-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f7441-116">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7441-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7441-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7441-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7441-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7441-118">Not supported.</span></span>    |
|<span data-ttu-id="f7441-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7441-119">Application</span></span> | <span data-ttu-id="f7441-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7441-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7441-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7441-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7441-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7441-122">Optional query parameters</span></span>
<span data-ttu-id="f7441-123">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="f7441-124">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="f7441-124">See an [example](#request-2) below.</span></span>

<span data-ttu-id="f7441-125">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f7441-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7441-126">请求头</span><span class="sxs-lookup"><span data-stu-id="f7441-126">Request headers</span></span>
| <span data-ttu-id="f7441-127">名称</span><span class="sxs-lookup"><span data-stu-id="f7441-127">Name</span></span>       | <span data-ttu-id="f7441-128">类型</span><span class="sxs-lookup"><span data-stu-id="f7441-128">Type</span></span> | <span data-ttu-id="f7441-129">说明</span><span class="sxs-lookup"><span data-stu-id="f7441-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7441-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7441-130">Authorization</span></span>  | <span data-ttu-id="f7441-131">string</span><span class="sxs-lookup"><span data-stu-id="f7441-131">string</span></span>  | <span data-ttu-id="f7441-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7441-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7441-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7441-134">Request body</span></span>
<span data-ttu-id="f7441-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7441-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7441-136">响应</span><span class="sxs-lookup"><span data-stu-id="f7441-136">Response</span></span>
<span data-ttu-id="f7441-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7441-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="f7441-138">除非使用 `$select` 指定特定属性，它会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="f7441-139">示例</span><span class="sxs-lookup"><span data-stu-id="f7441-139">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="f7441-140">请求 1</span><span class="sxs-lookup"><span data-stu-id="f7441-140">Request 1</span></span>
<span data-ttu-id="f7441-141">下面是一个 GET 请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7441-141">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="f7441-142">响应 1</span><span class="sxs-lookup"><span data-stu-id="f7441-142">Response 1</span></span>
<span data-ttu-id="f7441-143">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7441-143">The following is an example of the response.</span></span> <span data-ttu-id="f7441-144">它仅包括默认属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-144">It includes only the default properties.</span></span>

><span data-ttu-id="f7441-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7441-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f7441-146">在实际调用中会返回所有默认属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-146">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="f7441-147">请求 2</span><span class="sxs-lookup"><span data-stu-id="f7441-147">Request 2</span></span>
<span data-ttu-id="f7441-148">下一个示例使用 `$select` 查询选项获取非默认返回的一些属性。</span><span class="sxs-lookup"><span data-stu-id="f7441-148">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="f7441-149">响应 2</span><span class="sxs-lookup"><span data-stu-id="f7441-149">Response 2</span></span>
<span data-ttu-id="f7441-150">下面是一个包括所请求的非默认属性的响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7441-150">The following is an example of the response which includes the requested non-default properties.</span></span>

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
  "tocPath": ""
}-->
