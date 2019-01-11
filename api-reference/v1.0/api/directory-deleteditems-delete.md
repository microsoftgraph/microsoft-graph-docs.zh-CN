---
title: 永久删除项目
description: 永久删除已删除的项目中的项目
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 00f44be1c89b35b81f3665d4bd568939ed309e22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805185"
---
# <a name="permanently-delete-item"></a><span data-ttu-id="f776e-103">永久删除项目</span><span class="sxs-lookup"><span data-stu-id="f776e-103">Permanently delete item</span></span>

<span data-ttu-id="f776e-104">永久删除[已删除的项目](../resources/directory.md)中的项目</span><span class="sxs-lookup"><span data-stu-id="f776e-104">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f776e-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="f776e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f776e-106">可以永久删除“已删除的项目”中的项目。</span><span class="sxs-lookup"><span data-stu-id="f776e-106">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="f776e-107">但当某个项目永久删除后，将**无法**还原。</span><span class="sxs-lookup"><span data-stu-id="f776e-107">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="f776e-108">权限</span><span class="sxs-lookup"><span data-stu-id="f776e-108">Permissions</span></span>
<span data-ttu-id="f776e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f776e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="f776e-111">对于用户：</span><span class="sxs-lookup"><span data-stu-id="f776e-111">For users:</span></span>

|<span data-ttu-id="f776e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f776e-112">Permission type</span></span>      | <span data-ttu-id="f776e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f776e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f776e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f776e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f776e-115">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f776e-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f776e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f776e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f776e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f776e-117">Not supported.</span></span> |
|<span data-ttu-id="f776e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f776e-118">Application</span></span> | <span data-ttu-id="f776e-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f776e-119">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="f776e-120">对于组：</span><span class="sxs-lookup"><span data-stu-id="f776e-120">For groups:</span></span>

|<span data-ttu-id="f776e-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="f776e-121">Permission type</span></span>      | <span data-ttu-id="f776e-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f776e-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f776e-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f776e-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f776e-124">Group.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f776e-124">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f776e-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f776e-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f776e-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="f776e-126">Not supported.</span></span>    |
|<span data-ttu-id="f776e-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="f776e-127">Application</span></span> | <span data-ttu-id="f776e-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f776e-128">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f776e-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f776e-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deletedItems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f776e-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="f776e-130">Request headers</span></span>
| <span data-ttu-id="f776e-131">名称</span><span class="sxs-lookup"><span data-stu-id="f776e-131">Name</span></span>       | <span data-ttu-id="f776e-132">说明</span><span class="sxs-lookup"><span data-stu-id="f776e-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f776e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="f776e-133">Authorization</span></span>  | <span data-ttu-id="f776e-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="f776e-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f776e-135">Accept</span><span class="sxs-lookup"><span data-stu-id="f776e-135">Accept</span></span>  | <span data-ttu-id="f776e-136">application/json</span><span class="sxs-lookup"><span data-stu-id="f776e-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f776e-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="f776e-137">Request body</span></span>
<span data-ttu-id="f776e-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f776e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f776e-139">响应</span><span class="sxs-lookup"><span data-stu-id="f776e-139">Response</span></span>

<span data-ttu-id="f776e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f776e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f776e-142">示例</span><span class="sxs-lookup"><span data-stu-id="f776e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f776e-143">请求</span><span class="sxs-lookup"><span data-stu-id="f776e-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="f776e-144">响应</span><span class="sxs-lookup"><span data-stu-id="f776e-144">Response</span></span>
<span data-ttu-id="f776e-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f776e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
