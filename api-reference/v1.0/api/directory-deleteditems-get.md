---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d84fe777cb5e99727dcf8168d03ff8f2ac25451
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656802"
---
# <a name="get-deleted-item"></a><span data-ttu-id="530db-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="530db-103">Get deleted item</span></span>

<span data-ttu-id="530db-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="530db-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="530db-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="530db-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="530db-106">权限</span><span class="sxs-lookup"><span data-stu-id="530db-106">Permissions</span></span>
<span data-ttu-id="530db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="530db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="530db-109">对于用户：</span><span class="sxs-lookup"><span data-stu-id="530db-109">For users:</span></span>

|<span data-ttu-id="530db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="530db-110">Permission type</span></span>      | <span data-ttu-id="530db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="530db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="530db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="530db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="530db-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="530db-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="530db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="530db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="530db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="530db-115">Not supported.</span></span> |
|<span data-ttu-id="530db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="530db-116">Application</span></span> | <span data-ttu-id="530db-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="530db-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="530db-118">对于组：</span><span class="sxs-lookup"><span data-stu-id="530db-118">For groups:</span></span>

|<span data-ttu-id="530db-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="530db-119">Permission type</span></span>      | <span data-ttu-id="530db-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="530db-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="530db-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="530db-121">Delegated (work or school account)</span></span> | <span data-ttu-id="530db-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="530db-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="530db-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="530db-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="530db-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="530db-124">Not supported.</span></span>    |
|<span data-ttu-id="530db-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="530db-125">Application</span></span> | <span data-ttu-id="530db-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="530db-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="530db-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="530db-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="530db-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="530db-128">Optional query parameters</span></span>
<span data-ttu-id="530db-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="530db-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="530db-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="530db-130">Request headers</span></span>
| <span data-ttu-id="530db-131">名称</span><span class="sxs-lookup"><span data-stu-id="530db-131">Name</span></span>      |<span data-ttu-id="530db-132">说明</span><span class="sxs-lookup"><span data-stu-id="530db-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="530db-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="530db-133">Authorization</span></span>  | <span data-ttu-id="530db-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="530db-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="530db-135">接受</span><span class="sxs-lookup"><span data-stu-id="530db-135">Accept</span></span>  | <span data-ttu-id="530db-136">application/json</span><span class="sxs-lookup"><span data-stu-id="530db-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="530db-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="530db-137">Request body</span></span>
<span data-ttu-id="530db-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="530db-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="530db-139">响应</span><span class="sxs-lookup"><span data-stu-id="530db-139">Response</span></span>

<span data-ttu-id="530db-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="530db-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="530db-141">示例</span><span class="sxs-lookup"><span data-stu-id="530db-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="530db-142">请求</span><span class="sxs-lookup"><span data-stu-id="530db-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="530db-143">响应</span><span class="sxs-lookup"><span data-stu-id="530db-143">Response</span></span>
<span data-ttu-id="530db-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="530db-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="530db-146">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="530db-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="530db-147">C#</span><span class="sxs-lookup"><span data-stu-id="530db-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="530db-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="530db-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
