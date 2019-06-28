---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9804a2395205e34f6371534b167a9de1efb29a2b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272378"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c5168-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="c5168-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="c5168-p101">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="c5168-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c5168-107">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="c5168-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c5168-108">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="c5168-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="c5168-109">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="c5168-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5168-110">权限</span><span class="sxs-lookup"><span data-stu-id="c5168-110">Permissions</span></span>

<span data-ttu-id="c5168-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5168-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c5168-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5168-113">Permission type</span></span>      | <span data-ttu-id="c5168-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5168-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5168-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5168-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c5168-116">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5168-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5168-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5168-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5168-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5168-118">Not supported.</span></span>    |
|<span data-ttu-id="c5168-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5168-119">Application</span></span> | <span data-ttu-id="c5168-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5168-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5168-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5168-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c5168-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5168-122">Request headers</span></span>

| <span data-ttu-id="c5168-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5168-123">Name</span></span>       | <span data-ttu-id="c5168-124">类型</span><span class="sxs-lookup"><span data-stu-id="c5168-124">Type</span></span> | <span data-ttu-id="c5168-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5168-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5168-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5168-126">Authorization</span></span>  | <span data-ttu-id="c5168-127">string</span><span class="sxs-lookup"><span data-stu-id="c5168-127">string</span></span>  | <span data-ttu-id="c5168-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5168-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5168-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5168-130">Content-Type</span></span>  | <span data-ttu-id="c5168-131">string</span><span class="sxs-lookup"><span data-stu-id="c5168-131">string</span></span> | <span data-ttu-id="c5168-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c5168-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5168-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5168-133">Request body</span></span>

<span data-ttu-id="c5168-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c5168-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5168-135">参数</span><span class="sxs-lookup"><span data-stu-id="c5168-135">Parameter</span></span>   | <span data-ttu-id="c5168-136">类型</span><span class="sxs-lookup"><span data-stu-id="c5168-136">Type</span></span> |<span data-ttu-id="c5168-137">说明</span><span class="sxs-lookup"><span data-stu-id="c5168-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5168-138">ids</span><span class="sxs-lookup"><span data-stu-id="c5168-138">ids</span></span>|<span data-ttu-id="c5168-139">String collection</span><span class="sxs-lookup"><span data-stu-id="c5168-139">String collection</span></span>| <span data-ttu-id="c5168-p104">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="c5168-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c5168-142">types</span><span class="sxs-lookup"><span data-stu-id="c5168-142">types</span></span>|<span data-ttu-id="c5168-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c5168-143">String collection</span></span>| <span data-ttu-id="c5168-144">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="c5168-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c5168-145">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="c5168-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c5168-146">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="c5168-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="c5168-147">若要搜索对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="c5168-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="c5168-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="c5168-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="c5168-149">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c5168-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c5168-150">响应</span><span class="sxs-lookup"><span data-stu-id="c5168-150">Response</span></span>

<span data-ttu-id="c5168-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c5168-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5168-152">示例</span><span class="sxs-lookup"><span data-stu-id="c5168-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5168-153">请求</span><span class="sxs-lookup"><span data-stu-id="c5168-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c5168-154">响应</span><span class="sxs-lookup"><span data-stu-id="c5168-154">Response</span></span>

<span data-ttu-id="c5168-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5168-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5168-157">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c5168-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5168-158">C#</span><span class="sxs-lookup"><span data-stu-id="c5168-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5168-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5168-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c5168-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5168-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getById-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
