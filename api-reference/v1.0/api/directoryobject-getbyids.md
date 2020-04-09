---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: keylimesoda
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ff81002804a445ab102b3df0bac2b57332fec2b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181928"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="b87ed-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="b87ed-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="b87ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b87ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b87ed-105">返回 ID 列表中指定的目录对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-105">Returns the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="b87ed-106">返回的目录对象是包含其所有属性的完整对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-106">The directory objects returned are the full objects containing all their properties.</span></span> <span data-ttu-id="b87ed-107">`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="b87ed-107">The `$select` query option is not available for this operation.</span></span>

>[!NOTE]
><span data-ttu-id="b87ed-108">此 API 存在一个[已知问题](/graph/known-issues#incomplete-objects-when-using-getbyids-request)。</span><span class="sxs-lookup"><span data-stu-id="b87ed-108">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="b87ed-109">返回的目录对象并非都是包含其所有属性的完整对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-109">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="b87ed-110">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="b87ed-110">Some common uses for this function are to:</span></span>

* <span data-ttu-id="b87ed-111">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-111">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="b87ed-112">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-112">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b87ed-113">权限</span><span class="sxs-lookup"><span data-stu-id="b87ed-113">Permissions</span></span>

<span data-ttu-id="b87ed-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b87ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b87ed-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="b87ed-116">Permission type</span></span>      | <span data-ttu-id="b87ed-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b87ed-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b87ed-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b87ed-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b87ed-119">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b87ed-119">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b87ed-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b87ed-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b87ed-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b87ed-121">Not supported.</span></span>    |
|<span data-ttu-id="b87ed-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="b87ed-122">Application</span></span> | <span data-ttu-id="b87ed-123">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b87ed-123">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b87ed-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b87ed-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="b87ed-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b87ed-125">Request headers</span></span>

| <span data-ttu-id="b87ed-126">名称</span><span class="sxs-lookup"><span data-stu-id="b87ed-126">Name</span></span>       | <span data-ttu-id="b87ed-127">类型</span><span class="sxs-lookup"><span data-stu-id="b87ed-127">Type</span></span> | <span data-ttu-id="b87ed-128">说明</span><span class="sxs-lookup"><span data-stu-id="b87ed-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b87ed-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b87ed-129">Authorization</span></span>  | <span data-ttu-id="b87ed-130">string</span><span class="sxs-lookup"><span data-stu-id="b87ed-130">string</span></span>  | <span data-ttu-id="b87ed-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b87ed-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b87ed-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b87ed-133">Content-Type</span></span>  | <span data-ttu-id="b87ed-134">string</span><span class="sxs-lookup"><span data-stu-id="b87ed-134">string</span></span> | <span data-ttu-id="b87ed-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b87ed-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b87ed-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b87ed-136">Request body</span></span>

<span data-ttu-id="b87ed-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b87ed-138">参数</span><span class="sxs-lookup"><span data-stu-id="b87ed-138">Parameter</span></span>   | <span data-ttu-id="b87ed-139">类型</span><span class="sxs-lookup"><span data-stu-id="b87ed-139">Type</span></span> |<span data-ttu-id="b87ed-140">说明</span><span class="sxs-lookup"><span data-stu-id="b87ed-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b87ed-141">ids</span><span class="sxs-lookup"><span data-stu-id="b87ed-141">ids</span></span>|<span data-ttu-id="b87ed-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b87ed-142">String collection</span></span>| <span data-ttu-id="b87ed-143">要返回其对象的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="b87ed-143">A collection of IDs for which to return objects.</span></span> <span data-ttu-id="b87ed-144">最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="b87ed-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="b87ed-145">types</span><span class="sxs-lookup"><span data-stu-id="b87ed-145">types</span></span>|<span data-ttu-id="b87ed-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b87ed-146">String collection</span></span>| <span data-ttu-id="b87ed-147">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="b87ed-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="b87ed-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="b87ed-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="b87ed-149">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="b87ed-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="b87ed-150">若要搜索对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="b87ed-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="b87ed-151">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="b87ed-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="b87ed-152">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="b87ed-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="b87ed-153">响应</span><span class="sxs-lookup"><span data-stu-id="b87ed-153">Response</span></span>

<span data-ttu-id="b87ed-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b87ed-154">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b87ed-155">示例</span><span class="sxs-lookup"><span data-stu-id="b87ed-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b87ed-156">请求</span><span class="sxs-lookup"><span data-stu-id="b87ed-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b87ed-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b87ed-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b87ed-158">C#</span><span class="sxs-lookup"><span data-stu-id="b87ed-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b87ed-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b87ed-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b87ed-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b87ed-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b87ed-161">Java</span><span class="sxs-lookup"><span data-stu-id="b87ed-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b87ed-162">响应</span><span class="sxs-lookup"><span data-stu-id="b87ed-162">Response</span></span>

<span data-ttu-id="b87ed-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b87ed-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
