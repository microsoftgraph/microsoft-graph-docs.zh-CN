---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02e56eac0d0e3ac8b2b0132f321098f0ea45b0de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435449"
---
# <a name="get-deleted-item"></a><span data-ttu-id="3a758-103">获取已删除项目</span><span class="sxs-lookup"><span data-stu-id="3a758-103">Get deleted item</span></span>

<span data-ttu-id="3a758-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3a758-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a758-105">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="3a758-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="3a758-106">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="3a758-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a758-107">权限</span><span class="sxs-lookup"><span data-stu-id="3a758-107">Permissions</span></span>
<span data-ttu-id="3a758-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a758-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="3a758-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="3a758-110">For applications:</span></span>

|<span data-ttu-id="3a758-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a758-111">Permission type</span></span>      | <span data-ttu-id="3a758-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a758-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a758-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a758-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a758-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a758-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a758-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a758-116">Not supported.</span></span>    |
|<span data-ttu-id="3a758-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a758-117">Application</span></span> | <span data-ttu-id="3a758-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a758-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="3a758-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="3a758-119">For users:</span></span>

|<span data-ttu-id="3a758-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a758-120">Permission type</span></span>      | <span data-ttu-id="3a758-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a758-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a758-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-122">Delegated (work or school account)</span></span> | <span data-ttu-id="3a758-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a758-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="3a758-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a758-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a758-125">Not supported.</span></span> |
|<span data-ttu-id="3a758-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a758-126">Application</span></span> | <span data-ttu-id="3a758-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a758-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="3a758-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="3a758-128">For groups:</span></span>

|<span data-ttu-id="3a758-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a758-129">Permission type</span></span>      | <span data-ttu-id="3a758-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a758-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a758-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-131">Delegated (work or school account)</span></span> | <span data-ttu-id="3a758-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a758-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3a758-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a758-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a758-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a758-134">Not supported.</span></span>    |
|<span data-ttu-id="3a758-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a758-135">Application</span></span> | <span data-ttu-id="3a758-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a758-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a758-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a758-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a758-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3a758-138">Optional query parameters</span></span>
<span data-ttu-id="3a758-139">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3a758-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a758-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a758-140">Request headers</span></span>
| <span data-ttu-id="3a758-141">名称</span><span class="sxs-lookup"><span data-stu-id="3a758-141">Name</span></span>      |<span data-ttu-id="3a758-142">说明</span><span class="sxs-lookup"><span data-stu-id="3a758-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a758-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a758-143">Authorization</span></span>  | <span data-ttu-id="3a758-144">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="3a758-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="3a758-145">接受</span><span class="sxs-lookup"><span data-stu-id="3a758-145">Accept</span></span>  | <span data-ttu-id="3a758-146">application/json</span><span class="sxs-lookup"><span data-stu-id="3a758-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a758-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a758-147">Request body</span></span>
<span data-ttu-id="3a758-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3a758-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a758-149">响应</span><span class="sxs-lookup"><span data-stu-id="3a758-149">Response</span></span>

<span data-ttu-id="3a758-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a758-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a758-151">示例</span><span class="sxs-lookup"><span data-stu-id="3a758-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a758-152">请求</span><span class="sxs-lookup"><span data-stu-id="3a758-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3a758-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a758-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="c"></a>[<span data-ttu-id="3a758-154">C#</span><span class="sxs-lookup"><span data-stu-id="3a758-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a758-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a758-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a758-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a758-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3a758-157">响应</span><span class="sxs-lookup"><span data-stu-id="3a758-157">Response</span></span>
<span data-ttu-id="3a758-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a758-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
