---
title: 检索最近删除的项的属性
description: 检索已删除的项目中最近删除项目的属性。
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3d6764ab3801ffa9afe42d2300db8ecc49e1ac3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966259"
---
# <a name="get-deleted-item"></a><span data-ttu-id="ec28f-103">获取已删除项目</span><span class="sxs-lookup"><span data-stu-id="ec28f-103">Get deleted item</span></span>

<span data-ttu-id="ec28f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec28f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec28f-105">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="ec28f-105">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ec28f-106">目前，仅支持 [应用程序](../resources/application.md)、 [组](../resources/group.md) 和 [用户](../resources/user.md) 资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="ec28f-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec28f-107">权限</span><span class="sxs-lookup"><span data-stu-id="ec28f-107">Permissions</span></span>
<span data-ttu-id="ec28f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec28f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="ec28f-110">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="ec28f-110">For applications:</span></span>

|<span data-ttu-id="ec28f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec28f-111">Permission type</span></span>      | <span data-ttu-id="ec28f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec28f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec28f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ec28f-114">Application.Read.All、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec28f-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec28f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec28f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec28f-116">Not supported.</span></span>    |
|<span data-ttu-id="ec28f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec28f-117">Application</span></span> | <span data-ttu-id="ec28f-118">"Application.readwrite.ownedby"、"全部"、"ReadWrite"、"全部"、"全部"、"全部读取"。</span><span class="sxs-lookup"><span data-stu-id="ec28f-118">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="ec28f-119">对于用户：</span><span class="sxs-lookup"><span data-stu-id="ec28f-119">For users:</span></span>

|<span data-ttu-id="ec28f-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec28f-120">Permission type</span></span>      | <span data-ttu-id="ec28f-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec28f-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec28f-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-122">Delegated (work or school account)</span></span> | <span data-ttu-id="ec28f-123">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec28f-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="ec28f-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec28f-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec28f-125">Not supported.</span></span> |
|<span data-ttu-id="ec28f-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec28f-126">Application</span></span> | <span data-ttu-id="ec28f-127">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec28f-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ec28f-128">对于组：</span><span class="sxs-lookup"><span data-stu-id="ec28f-128">For groups:</span></span>

|<span data-ttu-id="ec28f-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec28f-129">Permission type</span></span>      | <span data-ttu-id="ec28f-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec28f-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec28f-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-131">Delegated (work or school account)</span></span> | <span data-ttu-id="ec28f-132">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec28f-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ec28f-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec28f-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec28f-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec28f-134">Not supported.</span></span>    |
|<span data-ttu-id="ec28f-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec28f-135">Application</span></span> | <span data-ttu-id="ec28f-136">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec28f-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec28f-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec28f-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec28f-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec28f-138">Optional query parameters</span></span>
<span data-ttu-id="ec28f-139">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec28f-139">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec28f-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec28f-140">Request headers</span></span>
| <span data-ttu-id="ec28f-141">名称</span><span class="sxs-lookup"><span data-stu-id="ec28f-141">Name</span></span>      |<span data-ttu-id="ec28f-142">说明</span><span class="sxs-lookup"><span data-stu-id="ec28f-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec28f-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec28f-143">Authorization</span></span>  | <span data-ttu-id="ec28f-144">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="ec28f-144">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ec28f-145">接受</span><span class="sxs-lookup"><span data-stu-id="ec28f-145">Accept</span></span>  | <span data-ttu-id="ec28f-146">application/json</span><span class="sxs-lookup"><span data-stu-id="ec28f-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec28f-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec28f-147">Request body</span></span>
<span data-ttu-id="ec28f-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec28f-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec28f-149">响应</span><span class="sxs-lookup"><span data-stu-id="ec28f-149">Response</span></span>

<span data-ttu-id="ec28f-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec28f-150">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec28f-151">示例</span><span class="sxs-lookup"><span data-stu-id="ec28f-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec28f-152">请求</span><span class="sxs-lookup"><span data-stu-id="ec28f-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec28f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec28f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="c"></a>[<span data-ttu-id="ec28f-154">C#</span><span class="sxs-lookup"><span data-stu-id="ec28f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec28f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec28f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec28f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec28f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec28f-157">Java</span><span class="sxs-lookup"><span data-stu-id="ec28f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec28f-158">响应</span><span class="sxs-lookup"><span data-stu-id="ec28f-158">Response</span></span>
<span data-ttu-id="ec28f-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec28f-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

