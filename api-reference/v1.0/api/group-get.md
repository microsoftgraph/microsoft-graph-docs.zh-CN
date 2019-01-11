---
title: 获取组
description: 获取组对象的属性和关系。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 554a0b6bf6fcb4afb2a57f12e2c814cf5fa57951
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873407"
---
# <a name="get-group"></a><span data-ttu-id="514a0-103">获取组</span><span class="sxs-lookup"><span data-stu-id="514a0-103">Get group</span></span>
<span data-ttu-id="514a0-104">获取组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="514a0-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="514a0-105">默认属性</span><span class="sxs-lookup"><span data-stu-id="514a0-105">Default properties</span></span>

<span data-ttu-id="514a0-p101">下面展示了在获取或列出组时返回的一组默认属性。这些默认属性是所有可用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="514a0-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="514a0-108">说明</span><span class="sxs-lookup"><span data-stu-id="514a0-108">description</span></span>
* <span data-ttu-id="514a0-109">displayName</span><span class="sxs-lookup"><span data-stu-id="514a0-109">displayName</span></span>
* <span data-ttu-id="514a0-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="514a0-110">groupTypes</span></span>
* <span data-ttu-id="514a0-111">id</span><span class="sxs-lookup"><span data-stu-id="514a0-111">id</span></span>
* <span data-ttu-id="514a0-112">mail</span><span class="sxs-lookup"><span data-stu-id="514a0-112">mail</span></span>
* <span data-ttu-id="514a0-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="514a0-113">mailEnabled</span></span>
* <span data-ttu-id="514a0-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="514a0-114">mailNickname</span></span>
* <span data-ttu-id="514a0-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="514a0-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="514a0-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="514a0-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="514a0-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="514a0-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="514a0-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="514a0-118">proxyAddresses</span></span>
* <span data-ttu-id="514a0-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="514a0-119">securityEnabled</span></span>
* <span data-ttu-id="514a0-120">visibility</span><span class="sxs-lookup"><span data-stu-id="514a0-120">visibility</span></span>

<span data-ttu-id="514a0-121">默认情况下，不返回下列组属性：</span><span class="sxs-lookup"><span data-stu-id="514a0-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="514a0-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="514a0-122">allowExternalSenders</span></span>
* <span data-ttu-id="514a0-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="514a0-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="514a0-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="514a0-124">isSubscribedByMail</span></span>
* <span data-ttu-id="514a0-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="514a0-125">unseenCount</span></span>

<span data-ttu-id="514a0-p102">若要获取这些属性，请使用 **$select** 查询参数。示例如下：</span><span class="sxs-lookup"><span data-stu-id="514a0-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="514a0-128">权限</span><span class="sxs-lookup"><span data-stu-id="514a0-128">Permissions</span></span>
<span data-ttu-id="514a0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="514a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="514a0-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="514a0-131">Permission type</span></span>      | <span data-ttu-id="514a0-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="514a0-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="514a0-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="514a0-133">Delegated (work or school account)</span></span> | <span data-ttu-id="514a0-134">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514a0-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="514a0-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="514a0-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="514a0-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="514a0-136">Not supported.</span></span>    |
|<span data-ttu-id="514a0-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="514a0-137">Application</span></span> | <span data-ttu-id="514a0-138">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="514a0-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="514a0-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="514a0-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="514a0-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="514a0-140">Optional query parameters</span></span>
<span data-ttu-id="514a0-141">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="514a0-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="514a0-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="514a0-142">Request headers</span></span>
| <span data-ttu-id="514a0-143">名称</span><span class="sxs-lookup"><span data-stu-id="514a0-143">Name</span></span>       | <span data-ttu-id="514a0-144">类型</span><span class="sxs-lookup"><span data-stu-id="514a0-144">Type</span></span> | <span data-ttu-id="514a0-145">说明</span><span class="sxs-lookup"><span data-stu-id="514a0-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="514a0-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="514a0-146">Authorization</span></span>  | <span data-ttu-id="514a0-147">string</span><span class="sxs-lookup"><span data-stu-id="514a0-147">string</span></span>  | <span data-ttu-id="514a0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="514a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="514a0-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="514a0-150">Request body</span></span>
<span data-ttu-id="514a0-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="514a0-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="514a0-152">响应</span><span class="sxs-lookup"><span data-stu-id="514a0-152">Response</span></span>
<span data-ttu-id="514a0-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="514a0-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="514a0-154">示例</span><span class="sxs-lookup"><span data-stu-id="514a0-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="514a0-155">请求</span><span class="sxs-lookup"><span data-stu-id="514a0-155">Request</span></span>
<span data-ttu-id="514a0-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="514a0-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="514a0-157">响应</span><span class="sxs-lookup"><span data-stu-id="514a0-157">Response</span></span>
<span data-ttu-id="514a0-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="514a0-158">The following is an example of the response.</span></span>

><span data-ttu-id="514a0-159">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="514a0-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="514a0-160">如上所述，默认属性将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="514a0-160">The default properties will be returned from an actual call, as described before.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
