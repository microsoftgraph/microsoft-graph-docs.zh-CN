---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12b1970601bf2e938ecaee8ff63a1ce9f1ada90d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583548"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="7449d-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="7449d-103">Permanently delete item</span></span>

<span data-ttu-id="7449d-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="7449d-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="7449d-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="7449d-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="7449d-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="7449d-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="7449d-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="7449d-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="7449d-108">权限</span><span class="sxs-lookup"><span data-stu-id="7449d-108">Permissions</span></span>
<span data-ttu-id="7449d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7449d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="7449d-111">对于用户：</span><span class="sxs-lookup"><span data-stu-id="7449d-111">For users:</span></span>

|<span data-ttu-id="7449d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7449d-112">Permission type</span></span>      | <span data-ttu-id="7449d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7449d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7449d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7449d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7449d-115">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7449d-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7449d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7449d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7449d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7449d-117">Not supported.</span></span> |
|<span data-ttu-id="7449d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7449d-118">Application</span></span> | <span data-ttu-id="7449d-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7449d-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="7449d-120">对于组：</span><span class="sxs-lookup"><span data-stu-id="7449d-120">For groups:</span></span>

|<span data-ttu-id="7449d-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="7449d-121">Permission type</span></span>      | <span data-ttu-id="7449d-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7449d-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7449d-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7449d-123">Delegated (work or school account)</span></span> | <span data-ttu-id="7449d-124">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7449d-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7449d-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7449d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7449d-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="7449d-126">Not supported.</span></span>    |
|<span data-ttu-id="7449d-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="7449d-127">Application</span></span> | <span data-ttu-id="7449d-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7449d-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7449d-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7449d-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7449d-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="7449d-130">Request headers</span></span>
| <span data-ttu-id="7449d-131">名称</span><span class="sxs-lookup"><span data-stu-id="7449d-131">Name</span></span>       | <span data-ttu-id="7449d-132">说明</span><span class="sxs-lookup"><span data-stu-id="7449d-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7449d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7449d-133">Authorization</span></span>  | <span data-ttu-id="7449d-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="7449d-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="7449d-135">接受</span><span class="sxs-lookup"><span data-stu-id="7449d-135">Accept</span></span>  | <span data-ttu-id="7449d-136">application/json</span><span class="sxs-lookup"><span data-stu-id="7449d-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7449d-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="7449d-137">Request body</span></span>
<span data-ttu-id="7449d-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7449d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7449d-139">响应</span><span class="sxs-lookup"><span data-stu-id="7449d-139">Response</span></span>

<span data-ttu-id="7449d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7449d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7449d-142">示例</span><span class="sxs-lookup"><span data-stu-id="7449d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7449d-143">请求</span><span class="sxs-lookup"><span data-stu-id="7449d-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="7449d-144">响应</span><span class="sxs-lookup"><span data-stu-id="7449d-144">Response</span></span>
<span data-ttu-id="7449d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7449d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
