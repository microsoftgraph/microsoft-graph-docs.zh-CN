---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57037df3121a101caa4ee8e55ecf763b2a562e1a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869940"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="1a8dc-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="1a8dc-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="1a8dc-104">返回 ID 列表中指定的目录对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-104">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="1a8dc-105">返回的目录对象是包含其所有属性的完整对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-105">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="1a8dc-106">`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-106">The `$select` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="1a8dc-107">此 API 存在一个[已知问题](/graph/known-issues#incomplete-objects-when-using-getbyids-request)。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-107">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="1a8dc-108">返回的目录对象并非都是包含其所有属性的完整对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-108">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="1a8dc-109">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="1a8dc-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="1a8dc-110">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-110">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="1a8dc-111">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a8dc-112">权限</span><span class="sxs-lookup"><span data-stu-id="1a8dc-112">Permissions</span></span>

<span data-ttu-id="1a8dc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a8dc-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a8dc-115">Permission type</span></span>      | <span data-ttu-id="1a8dc-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a8dc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8dc-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a8dc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="1a8dc-118">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a8dc-118">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a8dc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a8dc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a8dc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-120">Not supported.</span></span>    |
|<span data-ttu-id="1a8dc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a8dc-121">Application</span></span> | <span data-ttu-id="1a8dc-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a8dc-122">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1a8dc-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a8dc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="1a8dc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a8dc-124">Request headers</span></span>

| <span data-ttu-id="1a8dc-125">名称</span><span class="sxs-lookup"><span data-stu-id="1a8dc-125">Name</span></span>       | <span data-ttu-id="1a8dc-126">类型</span><span class="sxs-lookup"><span data-stu-id="1a8dc-126">Type</span></span> | <span data-ttu-id="1a8dc-127">说明</span><span class="sxs-lookup"><span data-stu-id="1a8dc-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1a8dc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a8dc-128">Authorization</span></span>  | <span data-ttu-id="1a8dc-129">string</span><span class="sxs-lookup"><span data-stu-id="1a8dc-129">string</span></span>  | <span data-ttu-id="1a8dc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a8dc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a8dc-132">Content-Type</span></span>  | <span data-ttu-id="1a8dc-133">string</span><span class="sxs-lookup"><span data-stu-id="1a8dc-133">string</span></span> | <span data-ttu-id="1a8dc-134">application/json</span><span class="sxs-lookup"><span data-stu-id="1a8dc-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a8dc-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a8dc-135">Request body</span></span>

<span data-ttu-id="1a8dc-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a8dc-137">参数</span><span class="sxs-lookup"><span data-stu-id="1a8dc-137">Parameter</span></span>   | <span data-ttu-id="1a8dc-138">类型</span><span class="sxs-lookup"><span data-stu-id="1a8dc-138">Type</span></span> |<span data-ttu-id="1a8dc-139">说明</span><span class="sxs-lookup"><span data-stu-id="1a8dc-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a8dc-140">ids</span><span class="sxs-lookup"><span data-stu-id="1a8dc-140">ids</span></span>|<span data-ttu-id="1a8dc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1a8dc-141">String collection</span></span>| <span data-ttu-id="1a8dc-142">要返回其对象的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-142">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="1a8dc-143">最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-143">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="1a8dc-144">types</span><span class="sxs-lookup"><span data-stu-id="1a8dc-144">types</span></span>|<span data-ttu-id="1a8dc-145">String collection</span><span class="sxs-lookup"><span data-stu-id="1a8dc-145">String collection</span></span>| <span data-ttu-id="1a8dc-146">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-146">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="1a8dc-147">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-147">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="1a8dc-148">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-148">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="1a8dc-149">若要搜索对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-149">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="1a8dc-150">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-150">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="1a8dc-151">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-151">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="1a8dc-152">响应</span><span class="sxs-lookup"><span data-stu-id="1a8dc-152">Response</span></span>

<span data-ttu-id="1a8dc-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-153">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a8dc-154">示例</span><span class="sxs-lookup"><span data-stu-id="1a8dc-154">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1a8dc-155">请求</span><span class="sxs-lookup"><span data-stu-id="1a8dc-155">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1a8dc-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a8dc-156">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a8dc-157">C#</span><span class="sxs-lookup"><span data-stu-id="1a8dc-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a8dc-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a8dc-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a8dc-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a8dc-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a8dc-160">Java</span><span class="sxs-lookup"><span data-stu-id="1a8dc-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1a8dc-161">响应</span><span class="sxs-lookup"><span data-stu-id="1a8dc-161">Response</span></span>

<span data-ttu-id="1a8dc-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a8dc-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
