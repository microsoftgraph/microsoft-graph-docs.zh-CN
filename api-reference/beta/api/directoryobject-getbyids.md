---
title: 'directoryObject: getByIds'
description: '返回 ID 列表中指定的目录对象。 '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b4bf049ed135b1dd563d640827360ddf91db0d47
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312869"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="38e1b-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="38e1b-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="38e1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38e1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38e1b-105">返回 ID 列表中指定的目录对象。</span><span class="sxs-lookup"><span data-stu-id="38e1b-105">Return the directory objects specified in a list of IDs.</span></span>

<span data-ttu-id="38e1b-106">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="38e1b-106">Some common uses for this function are to:</span></span>

* <span data-ttu-id="38e1b-107">将返回 ID 集合的函数（例如 [getMemberObjects](./directoryobject-getmemberobjects.md) 或 [getMemberGroups](./directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="38e1b-107">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](./directoryobject-getmemberobjects.md) or [getMemberGroups](./directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="38e1b-108">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="38e1b-108">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="38e1b-109">权限</span><span class="sxs-lookup"><span data-stu-id="38e1b-109">Permissions</span></span>

<span data-ttu-id="38e1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="38e1b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="38e1b-112">Permission type</span></span>      | <span data-ttu-id="38e1b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38e1b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38e1b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38e1b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="38e1b-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="38e1b-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="38e1b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38e1b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38e1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38e1b-117">Not supported.</span></span>    |
|<span data-ttu-id="38e1b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="38e1b-118">Application</span></span> | <span data-ttu-id="38e1b-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="38e1b-119">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="38e1b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38e1b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="38e1b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="38e1b-121">Request headers</span></span>

| <span data-ttu-id="38e1b-122">名称</span><span class="sxs-lookup"><span data-stu-id="38e1b-122">Name</span></span>       | <span data-ttu-id="38e1b-123">类型</span><span class="sxs-lookup"><span data-stu-id="38e1b-123">Type</span></span> | <span data-ttu-id="38e1b-124">说明</span><span class="sxs-lookup"><span data-stu-id="38e1b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38e1b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="38e1b-125">Authorization</span></span>  | <span data-ttu-id="38e1b-126">string</span><span class="sxs-lookup"><span data-stu-id="38e1b-126">string</span></span>  | <span data-ttu-id="38e1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38e1b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38e1b-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="38e1b-129">Content-type</span></span>  | <span data-ttu-id="38e1b-130">string</span><span class="sxs-lookup"><span data-stu-id="38e1b-130">string</span></span> | <span data-ttu-id="38e1b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="38e1b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38e1b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="38e1b-133">Request body</span></span>

<span data-ttu-id="38e1b-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="38e1b-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38e1b-135">参数</span><span class="sxs-lookup"><span data-stu-id="38e1b-135">Parameter</span></span>   | <span data-ttu-id="38e1b-136">类型</span><span class="sxs-lookup"><span data-stu-id="38e1b-136">Type</span></span> |<span data-ttu-id="38e1b-137">说明</span><span class="sxs-lookup"><span data-stu-id="38e1b-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38e1b-138">ids</span><span class="sxs-lookup"><span data-stu-id="38e1b-138">ids</span></span>|<span data-ttu-id="38e1b-139">String collection</span><span class="sxs-lookup"><span data-stu-id="38e1b-139">String collection</span></span>| <span data-ttu-id="38e1b-140">要返回其对象的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="38e1b-140">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="38e1b-141">ID 是 GUID，由字符串表示。</span><span class="sxs-lookup"><span data-stu-id="38e1b-141">The IDs are GUIDs, represented as strings.</span></span> <span data-ttu-id="38e1b-142">最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="38e1b-142">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="38e1b-143">types</span><span class="sxs-lookup"><span data-stu-id="38e1b-143">types</span></span>|<span data-ttu-id="38e1b-144">String collection</span><span class="sxs-lookup"><span data-stu-id="38e1b-144">String collection</span></span>| <span data-ttu-id="38e1b-145">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="38e1b-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="38e1b-146">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="38e1b-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="38e1b-147">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta)、[device](/graph/api/resources/device?view=graph-rest-beta) 等。</span><span class="sxs-lookup"><span data-stu-id="38e1b-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="38e1b-148">若要搜索对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="38e1b-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="38e1b-149">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="38e1b-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="38e1b-150">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="38e1b-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="38e1b-151">响应</span><span class="sxs-lookup"><span data-stu-id="38e1b-151">Response</span></span>

<span data-ttu-id="38e1b-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="38e1b-152">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38e1b-153">示例</span><span class="sxs-lookup"><span data-stu-id="38e1b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="38e1b-154">请求</span><span class="sxs-lookup"><span data-stu-id="38e1b-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="38e1b-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="38e1b-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```
# <a name="c"></a>[<span data-ttu-id="38e1b-156">C#</span><span class="sxs-lookup"><span data-stu-id="38e1b-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38e1b-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38e1b-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38e1b-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38e1b-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38e1b-159">响应</span><span class="sxs-lookup"><span data-stu-id="38e1b-159">Response</span></span>

><span data-ttu-id="38e1b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38e1b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
