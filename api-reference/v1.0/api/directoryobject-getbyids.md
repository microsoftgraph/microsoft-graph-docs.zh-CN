---
title: 'directoryObject: getByIds'
description: 返回 ID 列表中指定的目录对象。
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bcd1e20de65f6ddefc08310572ff596865d438da
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051492"
---
# <a name="directoryobject-getbyids"></a><span data-ttu-id="43931-103">directoryObject: getByIds</span><span class="sxs-lookup"><span data-stu-id="43931-103">directoryObject: getByIds</span></span>

<span data-ttu-id="43931-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43931-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43931-105">返回 ID 列表中指定的目录对象。</span><span class="sxs-lookup"><span data-stu-id="43931-105">Return the directory objects specified in a list of IDs.</span></span>

>[!NOTE]
><span data-ttu-id="43931-106">此 API 存在一个[已知问题](/graph/known-issues#incomplete-objects-when-using-getbyids-request)。</span><span class="sxs-lookup"><span data-stu-id="43931-106">This API has a [known issue](/graph/known-issues#incomplete-objects-when-using-getbyids-request).</span></span> <span data-ttu-id="43931-107">返回的目录对象并非都是包含其所有属性的完整对象。</span><span class="sxs-lookup"><span data-stu-id="43931-107">Not all directory objects returned are the full objects containing all their properties.</span></span>

<span data-ttu-id="43931-108">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="43931-108">Some common uses for this function are to:</span></span>

* <span data-ttu-id="43931-109">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="43931-109">Resolve IDs returned by functions (that return collections of IDs) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="43931-110">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="43931-110">Resolve IDs persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="43931-111">权限</span><span class="sxs-lookup"><span data-stu-id="43931-111">Permissions</span></span>

<span data-ttu-id="43931-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43931-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="43931-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="43931-114">Permission type</span></span>      | <span data-ttu-id="43931-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43931-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43931-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43931-116">Delegated (work or school account)</span></span> | <span data-ttu-id="43931-117">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43931-117">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43931-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43931-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43931-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="43931-119">Not supported.</span></span>    |
|<span data-ttu-id="43931-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="43931-120">Application</span></span> | <span data-ttu-id="43931-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="43931-121">Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="43931-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43931-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="43931-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="43931-123">Request headers</span></span>

| <span data-ttu-id="43931-124">名称</span><span class="sxs-lookup"><span data-stu-id="43931-124">Name</span></span>       | <span data-ttu-id="43931-125">类型</span><span class="sxs-lookup"><span data-stu-id="43931-125">Type</span></span> | <span data-ttu-id="43931-126">说明</span><span class="sxs-lookup"><span data-stu-id="43931-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="43931-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="43931-127">Authorization</span></span>  | <span data-ttu-id="43931-128">string</span><span class="sxs-lookup"><span data-stu-id="43931-128">string</span></span>  | <span data-ttu-id="43931-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43931-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43931-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="43931-131">Content-type</span></span>  | <span data-ttu-id="43931-132">string</span><span class="sxs-lookup"><span data-stu-id="43931-132">string</span></span> | <span data-ttu-id="43931-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="43931-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="43931-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="43931-135">Request body</span></span>

<span data-ttu-id="43931-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="43931-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="43931-137">参数</span><span class="sxs-lookup"><span data-stu-id="43931-137">Parameter</span></span>   | <span data-ttu-id="43931-138">类型</span><span class="sxs-lookup"><span data-stu-id="43931-138">Type</span></span> |<span data-ttu-id="43931-139">说明</span><span class="sxs-lookup"><span data-stu-id="43931-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43931-140">ids</span><span class="sxs-lookup"><span data-stu-id="43931-140">ids</span></span>|<span data-ttu-id="43931-141">String collection</span><span class="sxs-lookup"><span data-stu-id="43931-141">String collection</span></span>| <span data-ttu-id="43931-142">要返回其对象的 ID 集合。</span><span class="sxs-lookup"><span data-stu-id="43931-142">A collection of IDs for which to return objects.</span></span>  <span data-ttu-id="43931-143">ID 是 GUID，由字符串表示。</span><span class="sxs-lookup"><span data-stu-id="43931-143">The IDs are GUIDs, represented as strings.</span></span>  <span data-ttu-id="43931-144">最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="43931-144">You can specify up to 1000 IDs.</span></span> |
|<span data-ttu-id="43931-145">types</span><span class="sxs-lookup"><span data-stu-id="43931-145">types</span></span>|<span data-ttu-id="43931-146">String collection</span><span class="sxs-lookup"><span data-stu-id="43931-146">String collection</span></span>| <span data-ttu-id="43931-147">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="43931-147">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="43931-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="43931-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="43931-149">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="43931-149">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="43931-150">若要搜索对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="43931-150">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="43931-151">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="43931-151">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="43931-152">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="43931-152">The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="43931-153">响应</span><span class="sxs-lookup"><span data-stu-id="43931-153">Response</span></span>

<span data-ttu-id="43931-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="43931-154">If successful, this method returns a `200 OK` response code and a string collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43931-155">示例</span><span class="sxs-lookup"><span data-stu-id="43931-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="43931-156">请求</span><span class="sxs-lookup"><span data-stu-id="43931-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="43931-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="43931-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43931-158">C#</span><span class="sxs-lookup"><span data-stu-id="43931-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43931-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43931-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43931-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43931-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43931-161">Java</span><span class="sxs-lookup"><span data-stu-id="43931-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43931-162">响应</span><span class="sxs-lookup"><span data-stu-id="43931-162">Response</span></span>

><span data-ttu-id="43931-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="43931-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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

