---
title: 获取组
description: 获取组对象的属性和关系。
ms.openlocfilehash: fbae878043580a9c5495b0462290e1da7af3bdd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009586"
---
# <a name="get-group"></a><span data-ttu-id="3a309-103">获取组</span><span class="sxs-lookup"><span data-stu-id="3a309-103">Get group</span></span>
<span data-ttu-id="3a309-104">获取组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a309-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="3a309-105">默认属性</span><span class="sxs-lookup"><span data-stu-id="3a309-105">Default properties</span></span>

<span data-ttu-id="3a309-p101">下面展示了在获取或列出组时返回的一组默认属性。这些默认属性是所有可用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="3a309-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="3a309-108">说明</span><span class="sxs-lookup"><span data-stu-id="3a309-108">description</span></span>
* <span data-ttu-id="3a309-109">displayName</span><span class="sxs-lookup"><span data-stu-id="3a309-109">displayName</span></span>
* <span data-ttu-id="3a309-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="3a309-110">groupTypes</span></span>
* <span data-ttu-id="3a309-111">id</span><span class="sxs-lookup"><span data-stu-id="3a309-111">id</span></span>
* <span data-ttu-id="3a309-112">mail</span><span class="sxs-lookup"><span data-stu-id="3a309-112">mail</span></span>
* <span data-ttu-id="3a309-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="3a309-113">mailEnabled</span></span>
* <span data-ttu-id="3a309-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3a309-114">mailNickname</span></span>
* <span data-ttu-id="3a309-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3a309-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="3a309-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a309-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="3a309-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="3a309-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="3a309-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="3a309-118">proxyAddresses</span></span>
* <span data-ttu-id="3a309-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="3a309-119">securityEnabled</span></span>
* <span data-ttu-id="3a309-120">visibility</span><span class="sxs-lookup"><span data-stu-id="3a309-120">visibility</span></span>

<span data-ttu-id="3a309-121">默认情况下，不返回下列组属性：</span><span class="sxs-lookup"><span data-stu-id="3a309-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="3a309-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="3a309-122">allowExternalSenders</span></span>
* <span data-ttu-id="3a309-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="3a309-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="3a309-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="3a309-124">isSubscribedByMail</span></span>
* <span data-ttu-id="3a309-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="3a309-125">unseenCount</span></span>

<span data-ttu-id="3a309-p102">若要获取这些属性，请使用 **$select** 查询参数。示例如下：</span><span class="sxs-lookup"><span data-stu-id="3a309-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="3a309-128">权限</span><span class="sxs-lookup"><span data-stu-id="3a309-128">Permissions</span></span>
<span data-ttu-id="3a309-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a309-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a309-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a309-131">Permission type</span></span>      | <span data-ttu-id="3a309-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a309-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a309-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a309-133">Delegated (work or school account)</span></span> | <span data-ttu-id="3a309-134">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a309-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a309-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a309-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a309-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a309-136">Not supported.</span></span>    |
|<span data-ttu-id="3a309-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a309-137">Application</span></span> | <span data-ttu-id="3a309-138">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a309-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a309-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a309-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a309-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3a309-140">Optional query parameters</span></span>
<span data-ttu-id="3a309-141">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3a309-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a309-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a309-142">Request headers</span></span>
| <span data-ttu-id="3a309-143">名称</span><span class="sxs-lookup"><span data-stu-id="3a309-143">Name</span></span>       | <span data-ttu-id="3a309-144">类型</span><span class="sxs-lookup"><span data-stu-id="3a309-144">Type</span></span> | <span data-ttu-id="3a309-145">说明</span><span class="sxs-lookup"><span data-stu-id="3a309-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3a309-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a309-146">Authorization</span></span>  | <span data-ttu-id="3a309-147">string</span><span class="sxs-lookup"><span data-stu-id="3a309-147">string</span></span>  | <span data-ttu-id="3a309-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a309-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a309-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a309-150">Request body</span></span>
<span data-ttu-id="3a309-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3a309-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a309-152">响应</span><span class="sxs-lookup"><span data-stu-id="3a309-152">Response</span></span>
<span data-ttu-id="3a309-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a309-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a309-154">示例</span><span class="sxs-lookup"><span data-stu-id="3a309-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3a309-155">请求</span><span class="sxs-lookup"><span data-stu-id="3a309-155">Request</span></span>
<span data-ttu-id="3a309-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3a309-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="3a309-157">响应</span><span class="sxs-lookup"><span data-stu-id="3a309-157">Response</span></span>
<span data-ttu-id="3a309-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3a309-158">The following is an example of the response.</span></span>

><span data-ttu-id="3a309-159">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3a309-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a309-160">如上所述，默认属性将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3a309-160">The default properties will be returned from an actual call, as described before.</span></span>
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
