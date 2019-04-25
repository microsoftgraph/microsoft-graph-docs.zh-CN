---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 25012a2437dd24345aebdc57351dea1f4ae1cfa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555134"
---
# <a name="list-deleted-items"></a><span data-ttu-id="6746f-103">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="6746f-103">List deleted items</span></span>

<span data-ttu-id="6746f-104">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="6746f-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="6746f-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="6746f-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="6746f-106">权限</span><span class="sxs-lookup"><span data-stu-id="6746f-106">Permissions</span></span>
<span data-ttu-id="6746f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6746f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="6746f-109">对于用户：</span><span class="sxs-lookup"><span data-stu-id="6746f-109">For users:</span></span>

|<span data-ttu-id="6746f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6746f-110">Permission type</span></span>      | <span data-ttu-id="6746f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6746f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6746f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6746f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6746f-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6746f-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6746f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6746f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6746f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6746f-115">Not supported.</span></span> |
|<span data-ttu-id="6746f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6746f-116">Application</span></span> | <span data-ttu-id="6746f-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6746f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="6746f-118">对于组：</span><span class="sxs-lookup"><span data-stu-id="6746f-118">For groups:</span></span>

|<span data-ttu-id="6746f-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="6746f-119">Permission type</span></span>      | <span data-ttu-id="6746f-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6746f-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6746f-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6746f-121">Delegated (work or school account)</span></span> | <span data-ttu-id="6746f-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6746f-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="6746f-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6746f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6746f-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="6746f-124">Not supported.</span></span>    |
|<span data-ttu-id="6746f-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="6746f-125">Application</span></span> | <span data-ttu-id="6746f-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6746f-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6746f-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6746f-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="6746f-128">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="6746f-128">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="6746f-129">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="6746f-129">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="6746f-130">不支持不使用类型调用 GET/directory/deletedItems。</span><span class="sxs-lookup"><span data-stu-id="6746f-130">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="6746f-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6746f-131">Optional query parameters</span></span>
<span data-ttu-id="6746f-132">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6746f-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6746f-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="6746f-133">Request headers</span></span>
| <span data-ttu-id="6746f-134">名称</span><span class="sxs-lookup"><span data-stu-id="6746f-134">Name</span></span>      |<span data-ttu-id="6746f-135">说明</span><span class="sxs-lookup"><span data-stu-id="6746f-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6746f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6746f-136">Authorization</span></span>  | <span data-ttu-id="6746f-137">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="6746f-137">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="6746f-138">接受</span><span class="sxs-lookup"><span data-stu-id="6746f-138">Accept</span></span>  | <span data-ttu-id="6746f-139">application/json</span><span class="sxs-lookup"><span data-stu-id="6746f-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6746f-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="6746f-140">Request body</span></span>
<span data-ttu-id="6746f-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6746f-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6746f-142">响应</span><span class="sxs-lookup"><span data-stu-id="6746f-142">Response</span></span>

<span data-ttu-id="6746f-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6746f-143">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6746f-144">示例</span><span class="sxs-lookup"><span data-stu-id="6746f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6746f-145">请求</span><span class="sxs-lookup"><span data-stu-id="6746f-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="6746f-146">响应</span><span class="sxs-lookup"><span data-stu-id="6746f-146">Response</span></span>
<span data-ttu-id="6746f-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6746f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
