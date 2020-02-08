---
title: 组： assignLicense
description: 在组中添加或删除许可证。 分配给该组的许可证将被分配给组中的所有用户。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43fa0a9346ccecc704c49ffc7528b71a58763fbc
ms.sourcegitcommit: cea768f767cf27a938b72bb26892d70e3dedaf2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2020
ms.locfileid: "41865769"
---
# <a name="group-assignlicense"></a><span data-ttu-id="49ebf-104">组： assignLicense</span><span class="sxs-lookup"><span data-stu-id="49ebf-104">group: assignLicense</span></span>

<span data-ttu-id="49ebf-105">在组中添加或删除许可证。</span><span class="sxs-lookup"><span data-stu-id="49ebf-105">Add or remove licenses on the group.</span></span> <span data-ttu-id="49ebf-106">分配给该组的许可证将被分配给组中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="49ebf-106">Licenses assigned to the group will be assigned to all users in the group.</span></span> <span data-ttu-id="49ebf-107">若要了解有关基于组的许可的详细信息，请参阅[什么是 Azure Active Directory 中的基于组的许可](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="49ebf-107">To learn more about group-based licensing, see [What is group-based licensing in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).</span></span>

<span data-ttu-id="49ebf-108">若要获取目录中可用的订阅，请执行[Get subscribedsku 请求](../resources/subscribedsku.md)。</span><span class="sxs-lookup"><span data-stu-id="49ebf-108">To get the subscriptions available in the directory, perform a [GET subscribedSkus request](../resources/subscribedsku.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49ebf-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="49ebf-109">Permissions</span></span>
<span data-ttu-id="49ebf-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49ebf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49ebf-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="49ebf-112">Permission type</span></span>      | <span data-ttu-id="49ebf-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49ebf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ebf-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49ebf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49ebf-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ebf-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="49ebf-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49ebf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ebf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="49ebf-117">Not supported.</span></span>    |
|<span data-ttu-id="49ebf-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="49ebf-118">Application</span></span> | <span data-ttu-id="49ebf-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ebf-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ebf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49ebf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/assignLicense
```
## <a name="request-headers"></a><span data-ttu-id="49ebf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="49ebf-121">Request headers</span></span>
| <span data-ttu-id="49ebf-122">标头</span><span class="sxs-lookup"><span data-stu-id="49ebf-122">Header</span></span>       | <span data-ttu-id="49ebf-123">值</span><span class="sxs-lookup"><span data-stu-id="49ebf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49ebf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49ebf-124">Authorization</span></span>  | <span data-ttu-id="49ebf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49ebf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49ebf-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49ebf-127">Content-Type</span></span>  | <span data-ttu-id="49ebf-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="49ebf-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49ebf-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="49ebf-130">Request body</span></span>
<span data-ttu-id="49ebf-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49ebf-132">参数</span><span class="sxs-lookup"><span data-stu-id="49ebf-132">Parameter</span></span>    | <span data-ttu-id="49ebf-133">类型</span><span class="sxs-lookup"><span data-stu-id="49ebf-133">Type</span></span>   |<span data-ttu-id="49ebf-134">说明</span><span class="sxs-lookup"><span data-stu-id="49ebf-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49ebf-135">addLicenses</span><span class="sxs-lookup"><span data-stu-id="49ebf-135">addLicenses</span></span>|<span data-ttu-id="49ebf-136">[assignedLicense](../resources/assignedlicense.md) 集合</span><span class="sxs-lookup"><span data-stu-id="49ebf-136">[assignedLicense](../resources/assignedlicense.md) collection</span></span>|<span data-ttu-id="49ebf-137">用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="49ebf-137">A collection of [assignedLicense](../resources/assignedlicense.md) objects that specify the licenses to add.</span></span> <span data-ttu-id="49ebf-138">您可以通过在[assignedLicense](../resources/assignedlicense.md)对象上设置**disabledPlans**属性来禁用与许可证关联的 servicePlans。</span><span class="sxs-lookup"><span data-stu-id="49ebf-138">You can disable servicePlans associated with a license by setting the **disabledPlans** property on an [assignedLicense](../resources/assignedlicense.md) object.</span></span>|
|<span data-ttu-id="49ebf-139">removeLicenses</span><span class="sxs-lookup"><span data-stu-id="49ebf-139">removeLicenses</span></span>|<span data-ttu-id="49ebf-140">GUID 集合</span><span class="sxs-lookup"><span data-stu-id="49ebf-140">GUID collection</span></span>|<span data-ttu-id="49ebf-141">标识要删除的许可证的 skuIds 的集合。</span><span class="sxs-lookup"><span data-stu-id="49ebf-141">A collection of skuIds that identify the licenses to remove.</span></span>|

## <a name="response"></a><span data-ttu-id="49ebf-142">响应</span><span class="sxs-lookup"><span data-stu-id="49ebf-142">Response</span></span>

<span data-ttu-id="49ebf-143">如果成功，此方法在响应`202 Accepted`正文中返回响应代码和目标[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-143">If successful, this method returns a `202 Accepted` response code and a target [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49ebf-144">示例</span><span class="sxs-lookup"><span data-stu-id="49ebf-144">Examples</span></span>

### <a name="example-1-add-licenses-to-the-group"></a><span data-ttu-id="49ebf-145">示例1：向组添加许可证</span><span class="sxs-lookup"><span data-stu-id="49ebf-145">Example 1: Add licenses to the group</span></span>
<span data-ttu-id="49ebf-146">下面的示例将许可证添加到组中。</span><span class="sxs-lookup"><span data-stu-id="49ebf-146">The following example adds licenses to the group.</span></span>
#### <a name="request"></a><span data-ttu-id="49ebf-147">请求</span><span class="sxs-lookup"><span data-stu-id="49ebf-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49ebf-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="49ebf-148">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="49ebf-149">响应</span><span class="sxs-lookup"><span data-stu-id="49ebf-149">Response</span></span>

<span data-ttu-id="49ebf-150">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-150">The response is the updated group object.</span></span>

><span data-ttu-id="49ebf-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49ebf-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49ebf-152">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-remove-licenses-from-the-group"></a><span data-ttu-id="49ebf-153">示例2：从组中删除许可证</span><span class="sxs-lookup"><span data-stu-id="49ebf-153">Example 2: Remove licenses from the group</span></span>
<span data-ttu-id="49ebf-154">下面的示例从组中删除许可证。</span><span class="sxs-lookup"><span data-stu-id="49ebf-154">The following example removes licenses from the group.</span></span>

#### <a name="request"></a><span data-ttu-id="49ebf-155">请求</span><span class="sxs-lookup"><span data-stu-id="49ebf-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="49ebf-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="49ebf-156">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="49ebf-157">响应</span><span class="sxs-lookup"><span data-stu-id="49ebf-157">Response</span></span>

<span data-ttu-id="49ebf-158">响应是更新的 group 对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-158">The response is the updated group object.</span></span>

><span data-ttu-id="49ebf-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49ebf-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49ebf-160">将从实际调用中返回所有属性。。</span><span class="sxs-lookup"><span data-stu-id="49ebf-160">All the properties will be returned from an actual call..</span></span>
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
