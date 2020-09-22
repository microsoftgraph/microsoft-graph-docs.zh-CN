---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a425563e3cdf45fa8b01c14935939b3ef0f66012
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008965"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="375db-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="375db-103">Restore deleted item</span></span>

<span data-ttu-id="375db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="375db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="375db-105">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="375db-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="375db-106">目前，仅支持 [应用程序](../resources/application.md)、 [组](../resources/group.md) 和 [用户](../resources/user.md) 资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="375db-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="375db-107">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="375db-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="375db-108">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="375db-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="375db-109">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="375db-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="375db-110">权限</span><span class="sxs-lookup"><span data-stu-id="375db-110">Permissions</span></span>
<span data-ttu-id="375db-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="375db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="375db-113">对于应用程序：</span><span class="sxs-lookup"><span data-stu-id="375db-113">For applications:</span></span>

|<span data-ttu-id="375db-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="375db-114">Permission type</span></span>      | <span data-ttu-id="375db-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="375db-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="375db-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-116">Delegated (work or school account)</span></span> | <span data-ttu-id="375db-117">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="375db-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="375db-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375db-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="375db-119">Not supported.</span></span>    |
|<span data-ttu-id="375db-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="375db-120">Application</span></span> | <span data-ttu-id="375db-121">Application.readwrite.ownedby 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="375db-121">Application.ReadWrite.All, Application.ReadWrite.OwnedBy</span></span> |


### <a name="for-users"></a><span data-ttu-id="375db-122">对于用户：</span><span class="sxs-lookup"><span data-stu-id="375db-122">For users:</span></span>

|<span data-ttu-id="375db-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="375db-123">Permission type</span></span>      | <span data-ttu-id="375db-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="375db-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="375db-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-125">Delegated (work or school account)</span></span> | <span data-ttu-id="375db-126">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="375db-126">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="375db-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375db-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="375db-128">Not supported.</span></span> |
|<span data-ttu-id="375db-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="375db-129">Application</span></span> | <span data-ttu-id="375db-130">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="375db-130">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="375db-131">对于组：</span><span class="sxs-lookup"><span data-stu-id="375db-131">For groups:</span></span>

|<span data-ttu-id="375db-132">权限类型</span><span class="sxs-lookup"><span data-stu-id="375db-132">Permission type</span></span>      | <span data-ttu-id="375db-133">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="375db-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="375db-134">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-134">Delegated (work or school account)</span></span> | <span data-ttu-id="375db-135">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="375db-135">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="375db-136">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="375db-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375db-137">不支持。</span><span class="sxs-lookup"><span data-stu-id="375db-137">Not supported.</span></span>    |
|<span data-ttu-id="375db-138">应用程序</span><span class="sxs-lookup"><span data-stu-id="375db-138">Application</span></span> | <span data-ttu-id="375db-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="375db-139">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="375db-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="375db-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="375db-141">请求标头</span><span class="sxs-lookup"><span data-stu-id="375db-141">Request headers</span></span>
| <span data-ttu-id="375db-142">名称</span><span class="sxs-lookup"><span data-stu-id="375db-142">Name</span></span>       | <span data-ttu-id="375db-143">说明</span><span class="sxs-lookup"><span data-stu-id="375db-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="375db-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="375db-144">Authorization</span></span>  | <span data-ttu-id="375db-145">必需的持有者 &lt; 令牌 &gt; *Required*</span><span class="sxs-lookup"><span data-stu-id="375db-145">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="375db-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="375db-146">Content-type</span></span> | <span data-ttu-id="375db-147">application/json</span><span class="sxs-lookup"><span data-stu-id="375db-147">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="375db-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="375db-148">Request body</span></span>
<span data-ttu-id="375db-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="375db-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="375db-150">响应</span><span class="sxs-lookup"><span data-stu-id="375db-150">Response</span></span>

<span data-ttu-id="375db-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="375db-151">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="375db-152">示例</span><span class="sxs-lookup"><span data-stu-id="375db-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="375db-153">请求</span><span class="sxs-lookup"><span data-stu-id="375db-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="375db-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="375db-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="375db-155">C#</span><span class="sxs-lookup"><span data-stu-id="375db-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="375db-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="375db-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="375db-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="375db-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="375db-158">响应</span><span class="sxs-lookup"><span data-stu-id="375db-158">Response</span></span>
<span data-ttu-id="375db-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="375db-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


