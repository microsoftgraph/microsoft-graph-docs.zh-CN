---
title: 获取组
description: 获取组对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 48bc4322326087895542ac24e23c7a57f5ddf07e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838673"
---
# <a name="get-group"></a><span data-ttu-id="09c20-103">获取组</span><span class="sxs-lookup"><span data-stu-id="09c20-103">Get group</span></span>

> <span data-ttu-id="09c20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09c20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09c20-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09c20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09c20-106">要获取的属性和一个[group](../resources/group.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="09c20-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="09c20-107">默认属性</span><span class="sxs-lookup"><span data-stu-id="09c20-107">Default properties</span></span>

<span data-ttu-id="09c20-p102">下面展示了在获取或列出组时返回的一组默认属性。这些默认属性是所有可用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="09c20-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="09c20-110">Classification</span><span class="sxs-lookup"><span data-stu-id="09c20-110">classification</span></span>
* <span data-ttu-id="09c20-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09c20-111">createdDateTime</span></span>
* <span data-ttu-id="09c20-112">说明</span><span class="sxs-lookup"><span data-stu-id="09c20-112">description</span></span>
* <span data-ttu-id="09c20-113">displayName</span><span class="sxs-lookup"><span data-stu-id="09c20-113">displayName</span></span>
* <span data-ttu-id="09c20-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="09c20-114">groupTypes</span></span>
* <span data-ttu-id="09c20-115">id</span><span class="sxs-lookup"><span data-stu-id="09c20-115">id</span></span>
* <span data-ttu-id="09c20-116">mail</span><span class="sxs-lookup"><span data-stu-id="09c20-116">mail</span></span>
* <span data-ttu-id="09c20-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="09c20-117">mailEnabled</span></span>
* <span data-ttu-id="09c20-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="09c20-118">mailNickname</span></span>
* <span data-ttu-id="09c20-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="09c20-119">membershipRule</span></span>
* <span data-ttu-id="09c20-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="09c20-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="09c20-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="09c20-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="09c20-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="09c20-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="09c20-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="09c20-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="09c20-124">preferredLanguage-不支持;此属性的值不能设置和返回`null`调用时。</span><span class="sxs-lookup"><span data-stu-id="09c20-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="09c20-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="09c20-125">proxyAddresses</span></span>
* <span data-ttu-id="09c20-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="09c20-126">renewedDateTime</span></span>
* <span data-ttu-id="09c20-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="09c20-127">securityEnabled</span></span>
* <span data-ttu-id="09c20-128">主题</span><span class="sxs-lookup"><span data-stu-id="09c20-128">theme</span></span>
* <span data-ttu-id="09c20-129">visibility</span><span class="sxs-lookup"><span data-stu-id="09c20-129">visibility</span></span>

<span data-ttu-id="09c20-130">默认情况下，不返回下列组属性：</span><span class="sxs-lookup"><span data-stu-id="09c20-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="09c20-131">accessType</span><span class="sxs-lookup"><span data-stu-id="09c20-131">accessType</span></span>
* <span data-ttu-id="09c20-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="09c20-132">allowExternalSenders</span></span>
* <span data-ttu-id="09c20-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="09c20-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="09c20-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="09c20-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="09c20-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="09c20-135">isSubscribedByMail</span></span>
* <span data-ttu-id="09c20-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="09c20-136">isFavorite</span></span>
* <span data-ttu-id="09c20-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="09c20-137">unseenConversationsCount</span></span>
* <span data-ttu-id="09c20-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="09c20-138">unseenCount</span></span>
* <span data-ttu-id="09c20-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="09c20-139">unseenMessagesCount</span></span>

<span data-ttu-id="09c20-140">若要获取这些属性 （除了**isFavorite**和**hasMembersWithLicenseErrors**），使用`$select`查询参数。</span><span class="sxs-lookup"><span data-stu-id="09c20-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="09c20-141">示例如下：</span><span class="sxs-lookup"><span data-stu-id="09c20-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="09c20-142">若要返回包含与许可错误的成员的组，请使用 **$filter**查询参数：</span><span class="sxs-lookup"><span data-stu-id="09c20-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="09c20-143">由于**group**资源支持[扩展](/graph/extensibility-overview)，您还可以使用`GET`操作来获取**组**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="09c20-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="09c20-144">权限</span><span class="sxs-lookup"><span data-stu-id="09c20-144">Permissions</span></span>
<span data-ttu-id="09c20-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09c20-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09c20-147">权限类型</span><span class="sxs-lookup"><span data-stu-id="09c20-147">Permission type</span></span>      | <span data-ttu-id="09c20-148">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09c20-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09c20-149">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09c20-149">Delegated (work or school account)</span></span> | <span data-ttu-id="09c20-150">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c20-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="09c20-151">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09c20-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09c20-152">不支持。</span><span class="sxs-lookup"><span data-stu-id="09c20-152">Not supported.</span></span>    |
|<span data-ttu-id="09c20-153">应用程序</span><span class="sxs-lookup"><span data-stu-id="09c20-153">Application</span></span> | <span data-ttu-id="09c20-154">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09c20-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09c20-155">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09c20-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="09c20-156">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="09c20-156">Optional query parameters</span></span>
<span data-ttu-id="09c20-157">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="09c20-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09c20-158">请求标头</span><span class="sxs-lookup"><span data-stu-id="09c20-158">Request headers</span></span>
| <span data-ttu-id="09c20-159">名称</span><span class="sxs-lookup"><span data-stu-id="09c20-159">Name</span></span>       | <span data-ttu-id="09c20-160">类型</span><span class="sxs-lookup"><span data-stu-id="09c20-160">Type</span></span> | <span data-ttu-id="09c20-161">说明</span><span class="sxs-lookup"><span data-stu-id="09c20-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="09c20-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="09c20-162">Authorization</span></span>  | <span data-ttu-id="09c20-163">string</span><span class="sxs-lookup"><span data-stu-id="09c20-163">string</span></span>  | <span data-ttu-id="09c20-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09c20-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09c20-166">请求正文</span><span class="sxs-lookup"><span data-stu-id="09c20-166">Request body</span></span>
<span data-ttu-id="09c20-167">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09c20-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09c20-168">响应</span><span class="sxs-lookup"><span data-stu-id="09c20-168">Response</span></span>
<span data-ttu-id="09c20-169">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09c20-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c20-170">示例</span><span class="sxs-lookup"><span data-stu-id="09c20-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="09c20-171">请求</span><span class="sxs-lookup"><span data-stu-id="09c20-171">Request</span></span>
<span data-ttu-id="09c20-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09c20-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="09c20-173">响应</span><span class="sxs-lookup"><span data-stu-id="09c20-173">Response</span></span>
<span data-ttu-id="09c20-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09c20-174">The following is an example of the response.</span></span> 
><span data-ttu-id="09c20-175">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="09c20-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09c20-176">如上所述，默认属性将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09c20-176">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

## <a name="see-also"></a><span data-ttu-id="09c20-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="09c20-177">See also</span></span>

- [<span data-ttu-id="09c20-178">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="09c20-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="09c20-179">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="09c20-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="09c20-180">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="09c20-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
