---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 093e39a6d70193c03d0b2ae9d91b61f6bdf5bbbb
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180942"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="2730a-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="2730a-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="2730a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2730a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2730a-p101">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="2730a-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="2730a-108">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="2730a-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="2730a-109">将返回 ID 集合的函数（例如 [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) 或 [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="2730a-109">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="2730a-110">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="2730a-110">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2730a-111">权限</span><span class="sxs-lookup"><span data-stu-id="2730a-111">Permissions</span></span>

<span data-ttu-id="2730a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2730a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2730a-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="2730a-114">Permission type</span></span>      | <span data-ttu-id="2730a-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2730a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2730a-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2730a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="2730a-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2730a-117">Directory.Read.All</span></span>    |
|<span data-ttu-id="2730a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2730a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2730a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2730a-119">Not supported.</span></span>    |
|<span data-ttu-id="2730a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2730a-120">Application</span></span> | <span data-ttu-id="2730a-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2730a-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2730a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2730a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="2730a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2730a-123">Request headers</span></span>

| <span data-ttu-id="2730a-124">名称</span><span class="sxs-lookup"><span data-stu-id="2730a-124">Name</span></span>       | <span data-ttu-id="2730a-125">类型</span><span class="sxs-lookup"><span data-stu-id="2730a-125">Type</span></span> | <span data-ttu-id="2730a-126">说明</span><span class="sxs-lookup"><span data-stu-id="2730a-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2730a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2730a-127">Authorization</span></span>  | <span data-ttu-id="2730a-128">string</span><span class="sxs-lookup"><span data-stu-id="2730a-128">string</span></span>  | <span data-ttu-id="2730a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2730a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2730a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2730a-131">Content-Type</span></span>  | <span data-ttu-id="2730a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2730a-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2730a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2730a-133">Request body</span></span>

<span data-ttu-id="2730a-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2730a-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2730a-135">参数</span><span class="sxs-lookup"><span data-stu-id="2730a-135">Parameter</span></span>   | <span data-ttu-id="2730a-136">类型</span><span class="sxs-lookup"><span data-stu-id="2730a-136">Type</span></span> |<span data-ttu-id="2730a-137">说明</span><span class="sxs-lookup"><span data-stu-id="2730a-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2730a-138">ids</span><span class="sxs-lookup"><span data-stu-id="2730a-138">ids</span></span>|<span data-ttu-id="2730a-139">String collection</span><span class="sxs-lookup"><span data-stu-id="2730a-139">String collection</span></span>| <span data-ttu-id="2730a-p104">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="2730a-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="2730a-142">types</span><span class="sxs-lookup"><span data-stu-id="2730a-142">types</span></span>|<span data-ttu-id="2730a-143">String collection</span><span class="sxs-lookup"><span data-stu-id="2730a-143">String collection</span></span>| <span data-ttu-id="2730a-144">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="2730a-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="2730a-145">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="2730a-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="2730a-146">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta)、[device](/graph/api/resources/device?view=graph-rest-beta) 等。</span><span class="sxs-lookup"><span data-stu-id="2730a-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="2730a-147">若要搜索对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="2730a-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="2730a-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="2730a-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="2730a-149">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2730a-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="2730a-150">响应</span><span class="sxs-lookup"><span data-stu-id="2730a-150">Response</span></span>

<span data-ttu-id="2730a-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2730a-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2730a-152">示例</span><span class="sxs-lookup"><span data-stu-id="2730a-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2730a-153">请求</span><span class="sxs-lookup"><span data-stu-id="2730a-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2730a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="2730a-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2730a-155">C#</span><span class="sxs-lookup"><span data-stu-id="2730a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2730a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2730a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2730a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2730a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2730a-158">响应</span><span class="sxs-lookup"><span data-stu-id="2730a-158">Response</span></span>

<span data-ttu-id="2730a-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2730a-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
