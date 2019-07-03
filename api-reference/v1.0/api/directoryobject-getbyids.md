---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d99c54f9faca15505dc4b6e20ad01badee86304
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445595"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="53e3f-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="53e3f-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="53e3f-p101">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="53e3f-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="53e3f-107">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="53e3f-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="53e3f-108">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="53e3f-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="53e3f-109">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="53e3f-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="53e3f-110">权限</span><span class="sxs-lookup"><span data-stu-id="53e3f-110">Permissions</span></span>

<span data-ttu-id="53e3f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53e3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="53e3f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="53e3f-113">Permission type</span></span>      | <span data-ttu-id="53e3f-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53e3f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53e3f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53e3f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="53e3f-116">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53e3f-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53e3f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53e3f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53e3f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="53e3f-118">Not supported.</span></span>    |
|<span data-ttu-id="53e3f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="53e3f-119">Application</span></span> | <span data-ttu-id="53e3f-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="53e3f-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53e3f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53e3f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="53e3f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="53e3f-122">Request headers</span></span>

| <span data-ttu-id="53e3f-123">名称</span><span class="sxs-lookup"><span data-stu-id="53e3f-123">Name</span></span>       | <span data-ttu-id="53e3f-124">类型</span><span class="sxs-lookup"><span data-stu-id="53e3f-124">Type</span></span> | <span data-ttu-id="53e3f-125">说明</span><span class="sxs-lookup"><span data-stu-id="53e3f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53e3f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="53e3f-126">Authorization</span></span>  | <span data-ttu-id="53e3f-127">string</span><span class="sxs-lookup"><span data-stu-id="53e3f-127">string</span></span>  | <span data-ttu-id="53e3f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53e3f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53e3f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53e3f-130">Content-Type</span></span>  | <span data-ttu-id="53e3f-131">string</span><span class="sxs-lookup"><span data-stu-id="53e3f-131">string</span></span> | <span data-ttu-id="53e3f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="53e3f-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53e3f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="53e3f-133">Request body</span></span>

<span data-ttu-id="53e3f-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53e3f-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53e3f-135">参数</span><span class="sxs-lookup"><span data-stu-id="53e3f-135">Parameter</span></span>   | <span data-ttu-id="53e3f-136">类型</span><span class="sxs-lookup"><span data-stu-id="53e3f-136">Type</span></span> |<span data-ttu-id="53e3f-137">说明</span><span class="sxs-lookup"><span data-stu-id="53e3f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53e3f-138">ids</span><span class="sxs-lookup"><span data-stu-id="53e3f-138">ids</span></span>|<span data-ttu-id="53e3f-139">String collection</span><span class="sxs-lookup"><span data-stu-id="53e3f-139">String collection</span></span>| <span data-ttu-id="53e3f-p104">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="53e3f-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="53e3f-142">types</span><span class="sxs-lookup"><span data-stu-id="53e3f-142">types</span></span>|<span data-ttu-id="53e3f-143">String collection</span><span class="sxs-lookup"><span data-stu-id="53e3f-143">String collection</span></span>| <span data-ttu-id="53e3f-144">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="53e3f-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="53e3f-145">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="53e3f-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="53e3f-146">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="53e3f-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="53e3f-147">若要搜索对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="53e3f-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="53e3f-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="53e3f-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="53e3f-149">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="53e3f-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="53e3f-150">响应</span><span class="sxs-lookup"><span data-stu-id="53e3f-150">Response</span></span>

<span data-ttu-id="53e3f-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="53e3f-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e3f-152">示例</span><span class="sxs-lookup"><span data-stu-id="53e3f-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="53e3f-153">请求</span><span class="sxs-lookup"><span data-stu-id="53e3f-153">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="53e3f-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="53e3f-154">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53e3f-155">C#</span><span class="sxs-lookup"><span data-stu-id="53e3f-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53e3f-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="53e3f-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53e3f-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53e3f-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53e3f-158">响应</span><span class="sxs-lookup"><span data-stu-id="53e3f-158">Response</span></span>

<span data-ttu-id="53e3f-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53e3f-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
