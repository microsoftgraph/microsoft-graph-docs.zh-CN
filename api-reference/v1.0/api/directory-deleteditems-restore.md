---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
ms.openlocfilehash: 3fa47d269cefaf54994b57f8f06a92a8ac8fc4b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010012"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="5d116-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="5d116-103">Restore deleted item</span></span>

<span data-ttu-id="5d116-104">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="5d116-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="5d116-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="5d116-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="5d116-106">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="5d116-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="5d116-107">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="5d116-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="5d116-108">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="5d116-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d116-109">权限</span><span class="sxs-lookup"><span data-stu-id="5d116-109">Permissions</span></span>
<span data-ttu-id="5d116-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d116-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="5d116-112">对于用户：</span><span class="sxs-lookup"><span data-stu-id="5d116-112">For users:</span></span>

|<span data-ttu-id="5d116-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d116-113">Permission type</span></span>      | <span data-ttu-id="5d116-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d116-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d116-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d116-115">Delegated (work or school account)</span></span> | <span data-ttu-id="5d116-116">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d116-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5d116-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d116-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d116-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d116-118">Not supported.</span></span> |
|<span data-ttu-id="5d116-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d116-119">Application</span></span> | <span data-ttu-id="5d116-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d116-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="5d116-121">对于组：</span><span class="sxs-lookup"><span data-stu-id="5d116-121">For groups:</span></span>

|<span data-ttu-id="5d116-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d116-122">Permission type</span></span>      | <span data-ttu-id="5d116-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d116-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d116-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d116-124">Delegated (work or school account)</span></span> | <span data-ttu-id="5d116-125">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d116-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5d116-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d116-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d116-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d116-127">Not supported.</span></span>    |
|<span data-ttu-id="5d116-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d116-128">Application</span></span> | <span data-ttu-id="5d116-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d116-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d116-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d116-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="5d116-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d116-131">Request headers</span></span>
| <span data-ttu-id="5d116-132">名称</span><span class="sxs-lookup"><span data-stu-id="5d116-132">Name</span></span>       | <span data-ttu-id="5d116-133">说明</span><span class="sxs-lookup"><span data-stu-id="5d116-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5d116-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d116-134">Authorization</span></span>  | <span data-ttu-id="5d116-135">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="5d116-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="5d116-136">Accept</span><span class="sxs-lookup"><span data-stu-id="5d116-136">Accept</span></span> | <span data-ttu-id="5d116-137">application/json</span><span class="sxs-lookup"><span data-stu-id="5d116-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d116-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d116-138">Request body</span></span>
<span data-ttu-id="5d116-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d116-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d116-140">响应</span><span class="sxs-lookup"><span data-stu-id="5d116-140">Response</span></span>

<span data-ttu-id="5d116-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d116-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d116-142">示例</span><span class="sxs-lookup"><span data-stu-id="5d116-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d116-143">请求</span><span class="sxs-lookup"><span data-stu-id="5d116-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="5d116-144">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d116-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5d116-145">响应</span><span class="sxs-lookup"><span data-stu-id="5d116-145">Response</span></span>
<span data-ttu-id="5d116-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d116-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->