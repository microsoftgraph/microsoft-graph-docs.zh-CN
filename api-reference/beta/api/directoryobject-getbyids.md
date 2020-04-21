---
title: directoryObject： getByIds
description: '返回 ID 列表中指定的目录对象。 '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f71233b25d4ede3479960e44a4de2876b4c9a0c7
ms.sourcegitcommit: 24092bd1e38e8adfd314dfe8dfea9b24a5c21da6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43581651"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="8eaaf-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="8eaaf-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="8eaaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eaaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eaaf-105">返回 Id 列表中指定的目录对象。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-105">Return the directory objects specified in a list of IDs.</span></span>  

<span data-ttu-id="8eaaf-106">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="8eaaf-106">Some common uses for this function are to:</span></span>

* <span data-ttu-id="8eaaf-107">将返回 ID 集合的函数（例如 [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) 或 [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-107">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="8eaaf-108">将应用程序保留在外部存储中的 Id 解析为其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-108">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eaaf-109">权限</span><span class="sxs-lookup"><span data-stu-id="8eaaf-109">Permissions</span></span>

<span data-ttu-id="8eaaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8eaaf-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eaaf-112">Permission type</span></span>      | <span data-ttu-id="8eaaf-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8eaaf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eaaf-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eaaf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8eaaf-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eaaf-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="8eaaf-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eaaf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eaaf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-117">Not supported.</span></span>    |
|<span data-ttu-id="8eaaf-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8eaaf-118">Application</span></span> | <span data-ttu-id="8eaaf-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eaaf-119">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8eaaf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eaaf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="8eaaf-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eaaf-121">Request headers</span></span>

| <span data-ttu-id="8eaaf-122">名称</span><span class="sxs-lookup"><span data-stu-id="8eaaf-122">Name</span></span>       | <span data-ttu-id="8eaaf-123">类型</span><span class="sxs-lookup"><span data-stu-id="8eaaf-123">Type</span></span> | <span data-ttu-id="8eaaf-124">说明</span><span class="sxs-lookup"><span data-stu-id="8eaaf-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8eaaf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eaaf-125">Authorization</span></span>  | <span data-ttu-id="8eaaf-126">string</span><span class="sxs-lookup"><span data-stu-id="8eaaf-126">string</span></span>  | <span data-ttu-id="8eaaf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8eaaf-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="8eaaf-129">Content-type</span></span>  | <span data-ttu-id="8eaaf-130">string</span><span class="sxs-lookup"><span data-stu-id="8eaaf-130">string</span></span> | <span data-ttu-id="8eaaf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8eaaf-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8eaaf-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eaaf-133">Request body</span></span>

<span data-ttu-id="8eaaf-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8eaaf-135">参数</span><span class="sxs-lookup"><span data-stu-id="8eaaf-135">Parameter</span></span>   | <span data-ttu-id="8eaaf-136">类型</span><span class="sxs-lookup"><span data-stu-id="8eaaf-136">Type</span></span> |<span data-ttu-id="8eaaf-137">说明</span><span class="sxs-lookup"><span data-stu-id="8eaaf-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eaaf-138">ids</span><span class="sxs-lookup"><span data-stu-id="8eaaf-138">ids</span></span>|<span data-ttu-id="8eaaf-139">String collection</span><span class="sxs-lookup"><span data-stu-id="8eaaf-139">String collection</span></span>| <span data-ttu-id="8eaaf-140">要返回其对象的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-140">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="8eaaf-141">Id 是 Guid，表示为字符串。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-141">The IDs are GUIDs, represented as strings.</span></span> <span data-ttu-id="8eaaf-142">最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-142">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="8eaaf-143">types</span><span class="sxs-lookup"><span data-stu-id="8eaaf-143">types</span></span>|<span data-ttu-id="8eaaf-144">String collection</span><span class="sxs-lookup"><span data-stu-id="8eaaf-144">String collection</span></span>| <span data-ttu-id="8eaaf-145">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="8eaaf-146">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="8eaaf-147">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta)、[device](/graph/api/resources/device?view=graph-rest-beta) 等。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="8eaaf-148">若要搜索对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="8eaaf-149">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="8eaaf-150">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="8eaaf-151">响应</span><span class="sxs-lookup"><span data-stu-id="8eaaf-151">Response</span></span>

<span data-ttu-id="8eaaf-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-152">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eaaf-153">示例</span><span class="sxs-lookup"><span data-stu-id="8eaaf-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eaaf-154">请求</span><span class="sxs-lookup"><span data-stu-id="8eaaf-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8eaaf-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="8eaaf-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8eaaf-156">C#</span><span class="sxs-lookup"><span data-stu-id="8eaaf-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8eaaf-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8eaaf-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8eaaf-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8eaaf-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8eaaf-159">响应</span><span class="sxs-lookup"><span data-stu-id="8eaaf-159">Response</span></span>

><span data-ttu-id="8eaaf-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8eaaf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
