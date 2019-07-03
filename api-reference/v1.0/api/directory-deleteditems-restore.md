---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 798be2e38bcbb064fac4069ec7e7276bd9ed49d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455964"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="60960-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="60960-103">Restore deleted item</span></span>

<span data-ttu-id="60960-104">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="60960-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="60960-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="60960-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="60960-106">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="60960-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="60960-107">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="60960-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="60960-108">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="60960-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="60960-109">权限</span><span class="sxs-lookup"><span data-stu-id="60960-109">Permissions</span></span>
<span data-ttu-id="60960-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60960-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="60960-112">对于用户：</span><span class="sxs-lookup"><span data-stu-id="60960-112">For users:</span></span>

|<span data-ttu-id="60960-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="60960-113">Permission type</span></span>      | <span data-ttu-id="60960-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60960-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60960-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60960-115">Delegated (work or school account)</span></span> | <span data-ttu-id="60960-116">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60960-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="60960-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60960-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60960-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60960-118">Not supported.</span></span> |
|<span data-ttu-id="60960-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="60960-119">Application</span></span> | <span data-ttu-id="60960-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60960-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="60960-121">对于组：</span><span class="sxs-lookup"><span data-stu-id="60960-121">For groups:</span></span>

|<span data-ttu-id="60960-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="60960-122">Permission type</span></span>      | <span data-ttu-id="60960-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60960-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60960-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60960-124">Delegated (work or school account)</span></span> | <span data-ttu-id="60960-125">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60960-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="60960-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60960-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60960-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="60960-127">Not supported.</span></span>    |
|<span data-ttu-id="60960-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="60960-128">Application</span></span> | <span data-ttu-id="60960-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60960-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60960-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60960-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="60960-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="60960-131">Request headers</span></span>
| <span data-ttu-id="60960-132">名称</span><span class="sxs-lookup"><span data-stu-id="60960-132">Name</span></span>       | <span data-ttu-id="60960-133">说明</span><span class="sxs-lookup"><span data-stu-id="60960-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60960-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="60960-134">Authorization</span></span>  | <span data-ttu-id="60960-135">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="60960-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="60960-136">接受</span><span class="sxs-lookup"><span data-stu-id="60960-136">Accept</span></span> | <span data-ttu-id="60960-137">application/json</span><span class="sxs-lookup"><span data-stu-id="60960-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="60960-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="60960-138">Request body</span></span>
<span data-ttu-id="60960-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60960-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60960-140">响应</span><span class="sxs-lookup"><span data-stu-id="60960-140">Response</span></span>

<span data-ttu-id="60960-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60960-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60960-142">示例</span><span class="sxs-lookup"><span data-stu-id="60960-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60960-143">请求</span><span class="sxs-lookup"><span data-stu-id="60960-143">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60960-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="60960-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60960-145">C#</span><span class="sxs-lookup"><span data-stu-id="60960-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60960-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="60960-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60960-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="60960-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="60960-148">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60960-148">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="60960-149">响应</span><span class="sxs-lookup"><span data-stu-id="60960-149">Response</span></span>
<span data-ttu-id="60960-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60960-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
