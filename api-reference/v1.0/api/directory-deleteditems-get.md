---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de025535058c8b796b591b5bcac2f91f4d3397e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932326"
---
# <a name="get-deleted-item"></a><span data-ttu-id="1b513-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="1b513-103">Get deleted item</span></span>

<span data-ttu-id="1b513-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="1b513-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1b513-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="1b513-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b513-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b513-106">Permissions</span></span>
<span data-ttu-id="1b513-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="1b513-109">对于用户：</span><span class="sxs-lookup"><span data-stu-id="1b513-109">For users:</span></span>

|<span data-ttu-id="1b513-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b513-110">Permission type</span></span>      | <span data-ttu-id="1b513-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b513-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b513-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b513-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b513-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b513-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="1b513-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b513-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b513-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b513-115">Not supported.</span></span> |
|<span data-ttu-id="1b513-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b513-116">Application</span></span> | <span data-ttu-id="1b513-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b513-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="1b513-118">对于组：</span><span class="sxs-lookup"><span data-stu-id="1b513-118">For groups:</span></span>

|<span data-ttu-id="1b513-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b513-119">Permission type</span></span>      | <span data-ttu-id="1b513-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b513-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b513-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b513-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1b513-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b513-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1b513-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b513-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b513-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b513-124">Not supported.</span></span>    |
|<span data-ttu-id="1b513-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b513-125">Application</span></span> | <span data-ttu-id="1b513-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b513-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b513-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b513-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b513-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b513-128">Optional query parameters</span></span>
<span data-ttu-id="1b513-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b513-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b513-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b513-130">Request headers</span></span>
| <span data-ttu-id="1b513-131">名称</span><span class="sxs-lookup"><span data-stu-id="1b513-131">Name</span></span>      |<span data-ttu-id="1b513-132">说明</span><span class="sxs-lookup"><span data-stu-id="1b513-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b513-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b513-133">Authorization</span></span>  | <span data-ttu-id="1b513-134">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="1b513-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1b513-135">Accept</span><span class="sxs-lookup"><span data-stu-id="1b513-135">Accept</span></span>  | <span data-ttu-id="1b513-136">application/json</span><span class="sxs-lookup"><span data-stu-id="1b513-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b513-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b513-137">Request body</span></span>
<span data-ttu-id="1b513-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b513-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b513-139">响应</span><span class="sxs-lookup"><span data-stu-id="1b513-139">Response</span></span>

<span data-ttu-id="1b513-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b513-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b513-141">示例</span><span class="sxs-lookup"><span data-stu-id="1b513-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b513-142">请求</span><span class="sxs-lookup"><span data-stu-id="1b513-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="1b513-143">响应</span><span class="sxs-lookup"><span data-stu-id="1b513-143">Response</span></span>
<span data-ttu-id="1b513-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b513-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
