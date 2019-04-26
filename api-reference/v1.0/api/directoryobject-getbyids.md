---
title: 获取 ID 列表中的目录对象
description: select` 查询选项不适用于此操作。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a209d391c72edd453bbfe9232b7d02121ca98128
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572008"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c7cae-103">获取 ID 列表中的目录对象</span><span class="sxs-lookup"><span data-stu-id="c7cae-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="c7cae-p101">返回 ID 列表中指定的目录对象。注意：返回的目录对象是包含其**所有**属性的完整对象。`$select` 查询选项不适用于此操作。</span><span class="sxs-lookup"><span data-stu-id="c7cae-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c7cae-107">该函数的一些常见用途是：</span><span class="sxs-lookup"><span data-stu-id="c7cae-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c7cae-108">将返回 ID 集合的函数（例如 [getMemberObjects](directoryobject-getmemberobjects.md) 或 [getMemberGroups](directoryobject-getmembergroups.md)）返回的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="c7cae-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="c7cae-109">将应用程序保存在外部存储中的 ID 解析到其后备目录对象。</span><span class="sxs-lookup"><span data-stu-id="c7cae-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7cae-110">权限</span><span class="sxs-lookup"><span data-stu-id="c7cae-110">Permissions</span></span>

<span data-ttu-id="c7cae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7cae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c7cae-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7cae-113">Permission type</span></span>      | <span data-ttu-id="c7cae-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7cae-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7cae-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7cae-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c7cae-116">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7cae-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7cae-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7cae-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7cae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7cae-118">Not supported.</span></span>    |
|<span data-ttu-id="c7cae-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7cae-119">Application</span></span> | <span data-ttu-id="c7cae-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7cae-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7cae-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7cae-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c7cae-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7cae-122">Request headers</span></span>

| <span data-ttu-id="c7cae-123">名称</span><span class="sxs-lookup"><span data-stu-id="c7cae-123">Name</span></span>       | <span data-ttu-id="c7cae-124">类型</span><span class="sxs-lookup"><span data-stu-id="c7cae-124">Type</span></span> | <span data-ttu-id="c7cae-125">说明</span><span class="sxs-lookup"><span data-stu-id="c7cae-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c7cae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7cae-126">Authorization</span></span>  | <span data-ttu-id="c7cae-127">string</span><span class="sxs-lookup"><span data-stu-id="c7cae-127">string</span></span>  | <span data-ttu-id="c7cae-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7cae-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7cae-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7cae-130">Content-Type</span></span>  | <span data-ttu-id="c7cae-131">string</span><span class="sxs-lookup"><span data-stu-id="c7cae-131">string</span></span> | <span data-ttu-id="c7cae-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c7cae-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c7cae-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7cae-133">Request body</span></span>

<span data-ttu-id="c7cae-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c7cae-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c7cae-135">参数</span><span class="sxs-lookup"><span data-stu-id="c7cae-135">Parameter</span></span>   | <span data-ttu-id="c7cae-136">类型</span><span class="sxs-lookup"><span data-stu-id="c7cae-136">Type</span></span> |<span data-ttu-id="c7cae-137">说明</span><span class="sxs-lookup"><span data-stu-id="c7cae-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7cae-138">ids</span><span class="sxs-lookup"><span data-stu-id="c7cae-138">ids</span></span>|<span data-ttu-id="c7cae-139">String collection</span><span class="sxs-lookup"><span data-stu-id="c7cae-139">String collection</span></span>| <span data-ttu-id="c7cae-p104">要返回其对象的 ID 集合。最多可以指定 1000 个 ID。</span><span class="sxs-lookup"><span data-stu-id="c7cae-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c7cae-142">types</span><span class="sxs-lookup"><span data-stu-id="c7cae-142">types</span></span>|<span data-ttu-id="c7cae-143">String collection</span><span class="sxs-lookup"><span data-stu-id="c7cae-143">String collection</span></span>| <span data-ttu-id="c7cae-144">指定要搜索的资源集合集的资源类型集合。</span><span class="sxs-lookup"><span data-stu-id="c7cae-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c7cae-145">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型。</span><span class="sxs-lookup"><span data-stu-id="c7cae-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c7cae-146">可以在该集合中指定派生自 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) 的任何对象，例如：[user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) 等。</span><span class="sxs-lookup"><span data-stu-id="c7cae-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="c7cae-147">若要搜索对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用 ，请指定[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0)。</span><span class="sxs-lookup"><span data-stu-id="c7cae-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="c7cae-148">如果未指定，则默认为 [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0)，其包含目录中定义的所有资源类型，对[云解决方案提供商](https://partner.microsoft.com/zh-CN/cloud-solution-provider)合作伙伴组织的引用除外。</span><span class="sxs-lookup"><span data-stu-id="c7cae-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/zh-CN/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="c7cae-149">这些值不区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c7cae-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c7cae-150">响应</span><span class="sxs-lookup"><span data-stu-id="c7cae-150">Response</span></span>

<span data-ttu-id="c7cae-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c7cae-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7cae-152">示例</span><span class="sxs-lookup"><span data-stu-id="c7cae-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c7cae-153">请求</span><span class="sxs-lookup"><span data-stu-id="c7cae-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c7cae-154">响应</span><span class="sxs-lookup"><span data-stu-id="c7cae-154">Response</span></span>

<span data-ttu-id="c7cae-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7cae-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
