---
title: 组： assignLicense
description: 在组中添加或删除许可证。 分配给该组的许可证将被分配给组中的所有用户。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9d8a4632f95e321f37583ac7df62f953694e3756
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403141"
---
# <a name="group-assignlicense"></a><span data-ttu-id="edd10-104">组： assignLicense</span><span class="sxs-lookup"><span data-stu-id="edd10-104">group: assignLicense</span></span>

<span data-ttu-id="edd10-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd10-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd10-106">在组中添加或删除许可证。</span><span class="sxs-lookup"><span data-stu-id="edd10-106">Add or remove licenses on the group.</span></span> <span data-ttu-id="edd10-107">分配给该组的许可证将被分配给组中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="edd10-107">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="edd10-108">若要了解有关基于组的许可的详细信息，请参阅 [什么是 Azure Active Directory 中的基于组的许可](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="edd10-108">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="edd10-109">若要获取目录中可用的订阅，请执行 [Get subscribedsku 请求](subscribedsku-list.md)。</span><span class="sxs-lookup"><span data-stu-id="edd10-109">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](subscribedsku-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="edd10-110">权限</span><span class="sxs-lookup"><span data-stu-id="edd10-110">Permissions</span></span>
<span data-ttu-id="edd10-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edd10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edd10-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="edd10-113">Permission type</span></span>      | <span data-ttu-id="edd10-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edd10-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd10-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edd10-115">Delegated (work or school account)</span></span> | <span data-ttu-id="edd10-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edd10-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="edd10-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edd10-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edd10-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="edd10-118">Not supported.</span></span>    |
|<span data-ttu-id="edd10-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="edd10-119">Application</span></span> | <span data-ttu-id="edd10-120">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edd10-120">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="edd10-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edd10-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="edd10-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="edd10-122">Request headers</span></span>
| <span data-ttu-id="edd10-123">标头</span><span class="sxs-lookup"><span data-stu-id="edd10-123">Header</span></span>       | <span data-ttu-id="edd10-124">值</span><span class="sxs-lookup"><span data-stu-id="edd10-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edd10-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="edd10-125">Authorization</span></span>  | <span data-ttu-id="edd10-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="edd10-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edd10-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edd10-128">Content-Type</span></span>  | <span data-ttu-id="edd10-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="edd10-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edd10-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="edd10-131">Request body</span></span>
<span data-ttu-id="edd10-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="edd10-133">参数</span><span class="sxs-lookup"><span data-stu-id="edd10-133">Parameter</span></span>    | <span data-ttu-id="edd10-134">类型</span><span class="sxs-lookup"><span data-stu-id="edd10-134">Type</span></span>   |<span data-ttu-id="edd10-135">说明</span><span class="sxs-lookup"><span data-stu-id="edd10-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edd10-136">addLicenses</span><span class="sxs-lookup"><span data-stu-id="edd10-136">addLicenses</span></span>|<span data-ttu-id="edd10-137">[assignedLicense](../resources/assignedlicense.md) 集合</span><span class="sxs-lookup"><span data-stu-id="edd10-137">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="edd10-138">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="edd10-138">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="edd10-139">您可以通过在[assignedLicense](../resources/assignedlicense.md)对象上设置**disabledPlans**属性来禁用与许可证关联的 servicePlans。</span><span class="sxs-lookup"><span data-stu-id="edd10-139">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="edd10-140">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="edd10-140">removeLicenses</span></span>|<span data-ttu-id="edd10-141">GUID 集合</span><span class="sxs-lookup"><span data-stu-id="edd10-141">GUID collection</span></span>|<span data-ttu-id="edd10-142">标识要删除的许可证的 skuIds 的集合。</span><span class="sxs-lookup"><span data-stu-id="edd10-142">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="edd10-143">响应</span><span class="sxs-lookup"><span data-stu-id="edd10-143">Response</span></span>

<span data-ttu-id="edd10-144">如果成功，此方法 `202 Accepted` 在响应正文中返回响应代码和目标 [组](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-144">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="edd10-145">示例</span><span class="sxs-lookup"><span data-stu-id="edd10-145">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="edd10-146">示例1：向组添加许可证</span><span class="sxs-lookup"><span data-stu-id="edd10-146">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="edd10-147">下面的示例将许可证添加到组中。</span><span class="sxs-lookup"><span data-stu-id="edd10-147">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="edd10-148">请求</span><span class="sxs-lookup"><span data-stu-id="edd10-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="edd10-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd10-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
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
# <a name="c"></a>[<span data-ttu-id="edd10-150">C#</span><span class="sxs-lookup"><span data-stu-id="edd10-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd10-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd10-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd10-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd10-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="edd10-153">响应</span><span class="sxs-lookup"><span data-stu-id="edd10-153">Response</span></span>
<span data-ttu-id="edd10-154">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-154">The response is the updated group object.</span></span>

><span data-ttu-id="edd10-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="edd10-156">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="edd10-156">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="edd10-157">示例2：从组中删除许可证</span><span class="sxs-lookup"><span data-stu-id="edd10-157">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="edd10-158">下面的示例从组中删除许可证。</span><span class="sxs-lookup"><span data-stu-id="edd10-158">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="edd10-159">请求</span><span class="sxs-lookup"><span data-stu-id="edd10-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="edd10-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd10-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense
Content-type: application/json


{
  "addLicenses": [],
  "removeLicenses": ["skuId-value-1", "skuId-value-2"]
}
```
# <a name="c"></a>[<span data-ttu-id="edd10-161">C#</span><span class="sxs-lookup"><span data-stu-id="edd10-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd10-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd10-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd10-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd10-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="edd10-164">响应</span><span class="sxs-lookup"><span data-stu-id="edd10-164">Response</span></span>
<span data-ttu-id="edd10-165">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-165">The response is the updated group object.</span></span>

><span data-ttu-id="edd10-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="edd10-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="edd10-167">将从实际调用中返回所有属性。。</span><span class="sxs-lookup"><span data-stu-id="edd10-167">All the properties will be returned from an actual call..</span></span>
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