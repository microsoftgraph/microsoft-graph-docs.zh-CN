---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e263d8693b277156d96dc6668945699466979fa0
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176548"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="0101d-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="0101d-103">Restore deleted item</span></span>

<span data-ttu-id="0101d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0101d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0101d-105">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="0101d-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="0101d-106">目前，仅应用程序、组和用户资源支持还原[已删除的项目功能](../resources/user.md)。 [](../resources/group.md) [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="0101d-106">Currently, restore deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md), and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="0101d-107">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="0101d-107">If an item was accidentally deleted, you can fully restore the item.</span></span> <span data-ttu-id="0101d-108">这不适用于永久删除的安全组。</span><span class="sxs-lookup"><span data-stu-id="0101d-108">This is not applicable to Security groups which are deleted permanently.</span></span>

<span data-ttu-id="0101d-109">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="0101d-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="0101d-110">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="0101d-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0101d-111">权限</span><span class="sxs-lookup"><span data-stu-id="0101d-111">Permissions</span></span>
<span data-ttu-id="0101d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0101d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="0101d-114">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="0101d-114">For applications:</span></span>

|<span data-ttu-id="0101d-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="0101d-115">Permission type</span></span>      | <span data-ttu-id="0101d-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0101d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0101d-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0101d-118">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0101d-118">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0101d-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0101d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0101d-120">Not supported.</span></span>    |
|<span data-ttu-id="0101d-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="0101d-121">Application</span></span> | <span data-ttu-id="0101d-122">Application.ReadWrite.All、 Application.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="0101d-122">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |


### <a name="for-users"></a><span data-ttu-id="0101d-123">对于用户：</span><span class="sxs-lookup"><span data-stu-id="0101d-123">For users:</span></span>

|<span data-ttu-id="0101d-124">权限类型</span><span class="sxs-lookup"><span data-stu-id="0101d-124">Permission type</span></span>      | <span data-ttu-id="0101d-125">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0101d-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0101d-126">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-126">Delegated (work or school account)</span></span> | <span data-ttu-id="0101d-127">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0101d-127">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0101d-128">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0101d-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="0101d-129">Not supported.</span></span> |
|<span data-ttu-id="0101d-130">应用程序</span><span class="sxs-lookup"><span data-stu-id="0101d-130">Application</span></span> | <span data-ttu-id="0101d-131">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0101d-131">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="0101d-132">对于组：</span><span class="sxs-lookup"><span data-stu-id="0101d-132">For groups:</span></span>

|<span data-ttu-id="0101d-133">权限类型</span><span class="sxs-lookup"><span data-stu-id="0101d-133">Permission type</span></span>      | <span data-ttu-id="0101d-134">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0101d-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0101d-135">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-135">Delegated (work or school account)</span></span> | <span data-ttu-id="0101d-136">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0101d-136">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0101d-137">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0101d-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0101d-138">不支持。</span><span class="sxs-lookup"><span data-stu-id="0101d-138">Not supported.</span></span>    |
|<span data-ttu-id="0101d-139">应用程序</span><span class="sxs-lookup"><span data-stu-id="0101d-139">Application</span></span> | <span data-ttu-id="0101d-140">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0101d-140">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0101d-141">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0101d-141">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="0101d-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="0101d-142">Request headers</span></span>
| <span data-ttu-id="0101d-143">名称</span><span class="sxs-lookup"><span data-stu-id="0101d-143">Name</span></span>       | <span data-ttu-id="0101d-144">说明</span><span class="sxs-lookup"><span data-stu-id="0101d-144">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0101d-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="0101d-145">Authorization</span></span>  | <span data-ttu-id="0101d-146">需要记 &lt; 名 &gt; *令牌*</span><span class="sxs-lookup"><span data-stu-id="0101d-146">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="0101d-147">Content-type</span><span class="sxs-lookup"><span data-stu-id="0101d-147">Content-type</span></span> | <span data-ttu-id="0101d-148">application/json</span><span class="sxs-lookup"><span data-stu-id="0101d-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0101d-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="0101d-149">Request body</span></span>
<span data-ttu-id="0101d-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0101d-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0101d-151">响应</span><span class="sxs-lookup"><span data-stu-id="0101d-151">Response</span></span>

<span data-ttu-id="0101d-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0101d-152">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0101d-153">示例</span><span class="sxs-lookup"><span data-stu-id="0101d-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="0101d-154">请求</span><span class="sxs-lookup"><span data-stu-id="0101d-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0101d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="0101d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="0101d-156">C#</span><span class="sxs-lookup"><span data-stu-id="0101d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0101d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0101d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0101d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0101d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0101d-159">Java</span><span class="sxs-lookup"><span data-stu-id="0101d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0101d-160">响应</span><span class="sxs-lookup"><span data-stu-id="0101d-160">Response</span></span>
<span data-ttu-id="0101d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0101d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


