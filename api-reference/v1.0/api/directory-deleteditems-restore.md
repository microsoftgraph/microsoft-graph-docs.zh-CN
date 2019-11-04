---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 11151e543a973b003334ee360c6eebcbc0c27063
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938798"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="9fc2c-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="9fc2c-103">Restore deleted item</span></span>

<span data-ttu-id="9fc2c-104">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="9fc2c-105">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="9fc2c-106">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="9fc2c-107">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="9fc2c-108">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc2c-109">权限</span><span class="sxs-lookup"><span data-stu-id="9fc2c-109">Permissions</span></span>
<span data-ttu-id="9fc2c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="9fc2c-112">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="9fc2c-112">For applications:</span></span>

|<span data-ttu-id="9fc2c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fc2c-113">Permission type</span></span>      | <span data-ttu-id="9fc2c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc2c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc2c-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9fc2c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc2c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-118">Not supported.</span></span>    |
|<span data-ttu-id="9fc2c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fc2c-119">Application</span></span> | <span data-ttu-id="9fc2c-120">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-120">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |


### <a name="for-users"></a><span data-ttu-id="9fc2c-121">对于用户：</span><span class="sxs-lookup"><span data-stu-id="9fc2c-121">For users:</span></span>

|<span data-ttu-id="9fc2c-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fc2c-122">Permission type</span></span>      | <span data-ttu-id="9fc2c-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc2c-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-124">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc2c-125">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-125">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9fc2c-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc2c-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-127">Not supported.</span></span> |
|<span data-ttu-id="9fc2c-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fc2c-128">Application</span></span> | <span data-ttu-id="9fc2c-129">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-129">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="9fc2c-130">对于组：</span><span class="sxs-lookup"><span data-stu-id="9fc2c-130">For groups:</span></span>

|<span data-ttu-id="9fc2c-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fc2c-131">Permission type</span></span>      | <span data-ttu-id="9fc2c-132">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc2c-133">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-133">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc2c-134">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-134">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9fc2c-135">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc2c-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc2c-136">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-136">Not supported.</span></span>    |
|<span data-ttu-id="9fc2c-137">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fc2c-137">Application</span></span> | <span data-ttu-id="9fc2c-138">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc2c-138">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fc2c-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fc2c-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="9fc2c-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fc2c-140">Request headers</span></span>
| <span data-ttu-id="9fc2c-141">名称</span><span class="sxs-lookup"><span data-stu-id="9fc2c-141">Name</span></span>       | <span data-ttu-id="9fc2c-142">说明</span><span class="sxs-lookup"><span data-stu-id="9fc2c-142">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9fc2c-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc2c-143">Authorization</span></span>  | <span data-ttu-id="9fc2c-144">必需&lt;的&gt; \*\* 持有者令牌</span><span class="sxs-lookup"><span data-stu-id="9fc2c-144">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="9fc2c-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="9fc2c-145">Content-type</span></span> | <span data-ttu-id="9fc2c-146">application/json</span><span class="sxs-lookup"><span data-stu-id="9fc2c-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc2c-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fc2c-147">Request body</span></span>
<span data-ttu-id="9fc2c-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fc2c-149">响应</span><span class="sxs-lookup"><span data-stu-id="9fc2c-149">Response</span></span>

<span data-ttu-id="9fc2c-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-150">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc2c-151">示例</span><span class="sxs-lookup"><span data-stu-id="9fc2c-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fc2c-152">请求</span><span class="sxs-lookup"><span data-stu-id="9fc2c-152">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9fc2c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc2c-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fc2c-154">C#</span><span class="sxs-lookup"><span data-stu-id="9fc2c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fc2c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fc2c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fc2c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fc2c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9fc2c-157">Java</span><span class="sxs-lookup"><span data-stu-id="9fc2c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9fc2c-158">响应</span><span class="sxs-lookup"><span data-stu-id="9fc2c-158">Response</span></span>
<span data-ttu-id="9fc2c-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fc2c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.type":"#microsoft.graph.group",
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
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
