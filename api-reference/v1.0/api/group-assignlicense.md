---
title: group： assignLicense
description: 在组上添加或删除许可证。 分配给该组的许可证将分配给该组中的所有用户。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e3a23cfe70a578392dc4fa4d75dfa6af414a1427
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679846"
---
# <a name="group-assignlicense"></a><span data-ttu-id="a0cb8-104">group： assignLicense</span><span class="sxs-lookup"><span data-stu-id="a0cb8-104">group: assignLicense</span></span>

<span data-ttu-id="a0cb8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0cb8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0cb8-106">在组上添加或删除许可证。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="a0cb8-107">分配给该组的许可证将分配给该组中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="a0cb8-108">若要了解有关基于组的许可，请参阅什么是基于组的许可[Azure Active Directory。](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="a0cb8-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="a0cb8-109">若要获取目录中可用的订阅，请执行 [GET subscribedSkus 请求](../resources/subscribedsku.md)。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0cb8-110">权限</span><span class="sxs-lookup"><span data-stu-id="a0cb8-110">Permissions</span></span>
<span data-ttu-id="a0cb8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0cb8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0cb8-113">Permission type</span></span>      | <span data-ttu-id="a0cb8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0cb8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0cb8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cb8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a0cb8-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0cb8-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0cb8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cb8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0cb8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-118">Not supported.</span></span>    |
|<span data-ttu-id="a0cb8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0cb8-119">Application</span></span> | <span data-ttu-id="a0cb8-120">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0cb8-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0cb8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0cb8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="a0cb8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0cb8-122">Request headers</span></span>
| <span data-ttu-id="a0cb8-123">标头</span><span class="sxs-lookup"><span data-stu-id="a0cb8-123">Header</span></span>       | <span data-ttu-id="a0cb8-124">值</span><span class="sxs-lookup"><span data-stu-id="a0cb8-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0cb8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0cb8-125">Authorization</span></span>  | <span data-ttu-id="a0cb8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0cb8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0cb8-128">Content-Type</span></span>  | <span data-ttu-id="a0cb8-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a0cb8-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0cb8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0cb8-131">Request body</span></span>
<span data-ttu-id="a0cb8-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a0cb8-133">参数</span><span class="sxs-lookup"><span data-stu-id="a0cb8-133">Parameter</span></span>    | <span data-ttu-id="a0cb8-134">类型</span><span class="sxs-lookup"><span data-stu-id="a0cb8-134">Type</span></span>   |<span data-ttu-id="a0cb8-135">说明</span><span class="sxs-lookup"><span data-stu-id="a0cb8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0cb8-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="a0cb8-136">addLicenses</span></span>|<span data-ttu-id="a0cb8-137">[assignedLicense](../resources/assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0cb8-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="a0cb8-138">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="a0cb8-139">可以通过在 assignedLicense 对象上设置 **disabledPlans** 属性来禁用 [与许可证关联的 servicePlans。](../resources/assignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a0cb8-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="a0cb8-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="a0cb8-140">removeLicenses</span></span>|<span data-ttu-id="a0cb8-141">GUID 集合</span><span class="sxs-lookup"><span data-stu-id="a0cb8-141">GUID collection</span></span>|<span data-ttu-id="a0cb8-142">标识要删除的许可证的 skuIds 集合。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="a0cb8-143">响应</span><span class="sxs-lookup"><span data-stu-id="a0cb8-143">Response</span></span>

<span data-ttu-id="a0cb8-144">如果成功，此方法在响应 `202 Accepted` 正文中返回 响应代码和目标 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0cb8-145">示例</span><span class="sxs-lookup"><span data-stu-id="a0cb8-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="a0cb8-146">示例 1：向组添加许可证</span><span class="sxs-lookup"><span data-stu-id="a0cb8-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="a0cb8-147">以下示例向组添加许可证。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="a0cb8-148">请求</span><span class="sxs-lookup"><span data-stu-id="a0cb8-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a0cb8-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0cb8-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [
    {
      "disabledPlans": [ "11b0131d-43c8-4bbb-b2c8-e80f9a50834a" ],
      "skuId": "skuId-value-1"
    },
    {
      "disabledPlans": [ "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235" ],
      "skuId": "skuId-value-2"
    }
  ],
  "removeLicenses": []
}
```
# <a name="c"></a>[<span data-ttu-id="a0cb8-150">C#</span><span class="sxs-lookup"><span data-stu-id="a0cb8-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0cb8-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0cb8-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0cb8-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0cb8-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0cb8-153">Java</span><span class="sxs-lookup"><span data-stu-id="a0cb8-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0cb8-154">响应</span><span class="sxs-lookup"><span data-stu-id="a0cb8-154">Response</span></span>

<span data-ttu-id="a0cb8-155">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-155">The response is the updated group object.</span></span>

><span data-ttu-id="a0cb8-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group

{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="a0cb8-157">示例 2：从组中删除许可证</span><span class="sxs-lookup"><span data-stu-id="a0cb8-157">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="a0cb8-158">以下示例从组中删除许可证。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-158">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="a0cb8-159">请求</span><span class="sxs-lookup"><span data-stu-id="a0cb8-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a0cb8-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0cb8-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="c"></a>[<span data-ttu-id="a0cb8-161">C#</span><span class="sxs-lookup"><span data-stu-id="a0cb8-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0cb8-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0cb8-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0cb8-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0cb8-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0cb8-164">Java</span><span class="sxs-lookup"><span data-stu-id="a0cb8-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0cb8-165">响应</span><span class="sxs-lookup"><span data-stu-id="a0cb8-165">Response</span></span>

<span data-ttu-id="a0cb8-166">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-166">The response is the updated group object.</span></span>

><span data-ttu-id="a0cb8-167">**注意：** 为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0cb8-167">**Note:** The response object shown here might be shortened for readability..</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/d056d009-17b3-4106-8173-cd3978ada898/directoryObjects/1ad75eeb-7e5a-4367-a493-9214d90d54d0/Microsoft.DirectoryServices.Group


{
  "id": "1ad75eeb-7e5a-4367-a493-9214d90d54d0",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-04-18T22:05:03Z",
  "securityEnabled": true,

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

