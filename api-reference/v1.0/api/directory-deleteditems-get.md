---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd511a85349012dbd8ea7c5230a7e74cd22be7b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373852"
---
# <a name="get-deleted-item"></a><span data-ttu-id="31f1c-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="31f1c-103">Get deleted item</span></span>

<span data-ttu-id="31f1c-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="31f1c-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="31f1c-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="31f1c-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="31f1c-106">权限</span><span class="sxs-lookup"><span data-stu-id="31f1c-106">Permissions</span></span>
<span data-ttu-id="31f1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="31f1c-109">对于用户：</span><span class="sxs-lookup"><span data-stu-id="31f1c-109">For users:</span></span>

|<span data-ttu-id="31f1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="31f1c-110">Permission type</span></span>      | <span data-ttu-id="31f1c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31f1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31f1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31f1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="31f1c-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31f1c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="31f1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31f1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31f1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31f1c-115">Not supported.</span></span> |
|<span data-ttu-id="31f1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="31f1c-116">Application</span></span> | <span data-ttu-id="31f1c-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f1c-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="31f1c-118">对于组：</span><span class="sxs-lookup"><span data-stu-id="31f1c-118">For groups:</span></span>

|<span data-ttu-id="31f1c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="31f1c-119">Permission type</span></span>      | <span data-ttu-id="31f1c-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31f1c-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31f1c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31f1c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="31f1c-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31f1c-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="31f1c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31f1c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31f1c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="31f1c-124">Not supported.</span></span>    |
|<span data-ttu-id="31f1c-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="31f1c-125">Application</span></span> | <span data-ttu-id="31f1c-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31f1c-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31f1c-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31f1c-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31f1c-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31f1c-128">Optional query parameters</span></span>
<span data-ttu-id="31f1c-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31f1c-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31f1c-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="31f1c-130">Request headers</span></span>
| <span data-ttu-id="31f1c-131">名称</span><span class="sxs-lookup"><span data-stu-id="31f1c-131">Name</span></span>      |<span data-ttu-id="31f1c-132">说明</span><span class="sxs-lookup"><span data-stu-id="31f1c-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31f1c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="31f1c-133">Authorization</span></span>  | <span data-ttu-id="31f1c-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="31f1c-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="31f1c-135">接受</span><span class="sxs-lookup"><span data-stu-id="31f1c-135">Accept</span></span>  | <span data-ttu-id="31f1c-136">application/json</span><span class="sxs-lookup"><span data-stu-id="31f1c-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="31f1c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="31f1c-137">Request body</span></span>
<span data-ttu-id="31f1c-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31f1c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31f1c-139">响应</span><span class="sxs-lookup"><span data-stu-id="31f1c-139">Response</span></span>

<span data-ttu-id="31f1c-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31f1c-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31f1c-141">示例</span><span class="sxs-lookup"><span data-stu-id="31f1c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31f1c-142">请求</span><span class="sxs-lookup"><span data-stu-id="31f1c-142">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="31f1c-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="31f1c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="31f1c-144">C#</span><span class="sxs-lookup"><span data-stu-id="31f1c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31f1c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31f1c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="31f1c-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="31f1c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="31f1c-147">Java</span><span class="sxs-lookup"><span data-stu-id="31f1c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31f1c-148">响应</span><span class="sxs-lookup"><span data-stu-id="31f1c-148">Response</span></span>
<span data-ttu-id="31f1c-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31f1c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
