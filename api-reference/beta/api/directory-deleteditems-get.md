---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b9df8782ac11daca16a5ffc0533839d46de3381
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937040"
---
# <a name="get-deleted-item"></a><span data-ttu-id="eee27-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="eee27-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eee27-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="eee27-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="eee27-105">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="eee27-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="eee27-106">权限</span><span class="sxs-lookup"><span data-stu-id="eee27-106">Permissions</span></span>
<span data-ttu-id="eee27-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eee27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="eee27-109">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="eee27-109">For applications:</span></span>

|<span data-ttu-id="eee27-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eee27-110">Permission type</span></span>      | <span data-ttu-id="eee27-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eee27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eee27-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eee27-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eee27-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eee27-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee27-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eee27-115">Not supported.</span></span>    |
|<span data-ttu-id="eee27-116">Application</span><span class="sxs-lookup"><span data-stu-id="eee27-116">Application</span></span> | <span data-ttu-id="eee27-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eee27-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="eee27-118">对于用户：</span><span class="sxs-lookup"><span data-stu-id="eee27-118">For users:</span></span>

|<span data-ttu-id="eee27-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="eee27-119">Permission type</span></span>      | <span data-ttu-id="eee27-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eee27-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eee27-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-121">Delegated (work or school account)</span></span> | <span data-ttu-id="eee27-122">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eee27-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="eee27-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee27-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="eee27-124">Not supported.</span></span> |
|<span data-ttu-id="eee27-125">Application</span><span class="sxs-lookup"><span data-stu-id="eee27-125">Application</span></span> | <span data-ttu-id="eee27-126">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eee27-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="eee27-127">对于组：</span><span class="sxs-lookup"><span data-stu-id="eee27-127">For groups:</span></span>

|<span data-ttu-id="eee27-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="eee27-128">Permission type</span></span>      | <span data-ttu-id="eee27-129">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eee27-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eee27-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-130">Delegated (work or school account)</span></span> | <span data-ttu-id="eee27-131">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eee27-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="eee27-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eee27-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eee27-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="eee27-133">Not supported.</span></span>    |
|<span data-ttu-id="eee27-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="eee27-134">Application</span></span> | <span data-ttu-id="eee27-135">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eee27-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eee27-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eee27-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eee27-137">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="eee27-137">Optional query parameters</span></span>
<span data-ttu-id="eee27-138">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eee27-138">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eee27-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="eee27-139">Request headers</span></span>
| <span data-ttu-id="eee27-140">名称</span><span class="sxs-lookup"><span data-stu-id="eee27-140">Name</span></span>      |<span data-ttu-id="eee27-141">说明</span><span class="sxs-lookup"><span data-stu-id="eee27-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eee27-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="eee27-142">Authorization</span></span>  | <span data-ttu-id="eee27-143">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="eee27-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="eee27-144">接受</span><span class="sxs-lookup"><span data-stu-id="eee27-144">Accept</span></span>  | <span data-ttu-id="eee27-145">application/json</span><span class="sxs-lookup"><span data-stu-id="eee27-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eee27-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="eee27-146">Request body</span></span>
<span data-ttu-id="eee27-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eee27-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eee27-148">响应</span><span class="sxs-lookup"><span data-stu-id="eee27-148">Response</span></span>

<span data-ttu-id="eee27-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eee27-149">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eee27-150">示例</span><span class="sxs-lookup"><span data-stu-id="eee27-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eee27-151">请求</span><span class="sxs-lookup"><span data-stu-id="eee27-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eee27-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="eee27-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eee27-153">C#</span><span class="sxs-lookup"><span data-stu-id="eee27-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eee27-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eee27-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eee27-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eee27-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eee27-156">响应</span><span class="sxs-lookup"><span data-stu-id="eee27-156">Response</span></span>
<span data-ttu-id="eee27-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eee27-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
