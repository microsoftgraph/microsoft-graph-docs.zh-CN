---
title: 获取 ID 列表中的目录对象
description: 选择查询选项不适用于此操作。
ms.openlocfilehash: e6f987a3269b209c5df71b4961cf73081286a76d
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222444"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="04fbb-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="04fbb-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="04fbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04fbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04fbb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04fbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04fbb-p102">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="04fbb-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="04fbb-109">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="04fbb-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="04fbb-110">将返回 ID 集合的函数（例如 [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) 或 [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="04fbb-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="04fbb-111">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="04fbb-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="04fbb-112">权限</span><span class="sxs-lookup"><span data-stu-id="04fbb-112">Permissions</span></span>

<span data-ttu-id="04fbb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04fbb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04fbb-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="04fbb-115">Permission type</span></span>      | <span data-ttu-id="04fbb-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04fbb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04fbb-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04fbb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="04fbb-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="04fbb-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="04fbb-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04fbb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04fbb-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="04fbb-120">Not supported.</span></span>    |
|<span data-ttu-id="04fbb-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="04fbb-121">Application</span></span> | <span data-ttu-id="04fbb-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="04fbb-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04fbb-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04fbb-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="04fbb-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="04fbb-124">Request headers</span></span>

| <span data-ttu-id="04fbb-125">Name</span><span class="sxs-lookup"><span data-stu-id="04fbb-125">Name</span></span>       | <span data-ttu-id="04fbb-126">类型</span><span class="sxs-lookup"><span data-stu-id="04fbb-126">Type</span></span> | <span data-ttu-id="04fbb-127">说明</span><span class="sxs-lookup"><span data-stu-id="04fbb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04fbb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="04fbb-128">Authorization</span></span>  | <span data-ttu-id="04fbb-129">string</span><span class="sxs-lookup"><span data-stu-id="04fbb-129">string</span></span>  | <span data-ttu-id="04fbb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04fbb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04fbb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04fbb-132">Content-Type</span></span>  | <span data-ttu-id="04fbb-133">application/json</span><span class="sxs-lookup"><span data-stu-id="04fbb-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04fbb-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="04fbb-134">Request body</span></span>

<span data-ttu-id="04fbb-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="04fbb-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04fbb-136">参数</span><span class="sxs-lookup"><span data-stu-id="04fbb-136">Parameter</span></span>   | <span data-ttu-id="04fbb-137">类型</span><span class="sxs-lookup"><span data-stu-id="04fbb-137">Type</span></span> |<span data-ttu-id="04fbb-138">说明</span><span class="sxs-lookup"><span data-stu-id="04fbb-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04fbb-139">ids</span><span class="sxs-lookup"><span data-stu-id="04fbb-139">ids</span></span>|<span data-ttu-id="04fbb-140">String collection</span><span class="sxs-lookup"><span data-stu-id="04fbb-140">String collection</span></span>| <span data-ttu-id="04fbb-p105">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="04fbb-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="04fbb-143">types</span><span class="sxs-lookup"><span data-stu-id="04fbb-143">types</span></span>|<span data-ttu-id="04fbb-144">String collection</span><span class="sxs-lookup"><span data-stu-id="04fbb-144">String collection</span></span>| <span data-ttu-id="04fbb-145">指定一组资源集搜索的资源类型的集合。</span><span class="sxs-lookup"><span data-stu-id="04fbb-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="04fbb-146">如果未指定，则默认为[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其中包含所有目录中定义的资源类型。</span><span class="sxs-lookup"><span data-stu-id="04fbb-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="04fbb-147">可能集合中的指定派生自[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)任何对象例如：[用户](/graph/api/resources/user?view=graph-rest-beta)、[组](/graph/api/resources/group?view=graph-rest-beta)、[设备](/graph/api/resources/device?view=graph-rest-beta)，等等。</span><span class="sxs-lookup"><span data-stu-id="04fbb-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="04fbb-148">若要搜索引用[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="04fbb-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="04fbb-149">如果未指定，则默认为[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)，其中包含所有目录，除引用[云解决方案提供商](https://partner.microsoft.com/en-us/cloud-solution-provider)合作伙伴组织中定义的资源类型。</span><span class="sxs-lookup"><span data-stu-id="04fbb-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="04fbb-150">值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="04fbb-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="04fbb-151">响应</span><span class="sxs-lookup"><span data-stu-id="04fbb-151">Response</span></span>

<span data-ttu-id="04fbb-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="04fbb-152">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04fbb-153">示例</span><span class="sxs-lookup"><span data-stu-id="04fbb-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04fbb-154">请求</span><span class="sxs-lookup"><span data-stu-id="04fbb-154">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="04fbb-155">响应</span><span class="sxs-lookup"><span data-stu-id="04fbb-155">Response</span></span>

<span data-ttu-id="04fbb-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04fbb-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
