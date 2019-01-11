---
title: 'user: getMemberObjects'
description: 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。
localization_priority: Normal
ms.openlocfilehash: 68475bd93343a8be2d104891ecbc1cc7bed06482
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825744"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="e34e6-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e34e6-104">user: getMemberObjects</span></span>

> <span data-ttu-id="e34e6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e34e6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e34e6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e34e6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e34e6-p103">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="e34e6-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e34e6-109">权限</span><span class="sxs-lookup"><span data-stu-id="e34e6-109">Permissions</span></span>
<span data-ttu-id="e34e6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e34e6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e34e6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e34e6-112">Permission type</span></span>      | <span data-ttu-id="e34e6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e34e6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e34e6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e34e6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e34e6-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e34e6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e34e6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e34e6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e34e6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e34e6-117">Not supported.</span></span>    |
|<span data-ttu-id="e34e6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e34e6-118">Application</span></span> | <span data-ttu-id="e34e6-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e34e6-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e34e6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e34e6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="e34e6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e34e6-121">Request headers</span></span>
| <span data-ttu-id="e34e6-122">标头</span><span class="sxs-lookup"><span data-stu-id="e34e6-122">Header</span></span>       | <span data-ttu-id="e34e6-123">值</span><span class="sxs-lookup"><span data-stu-id="e34e6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e34e6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e34e6-124">Authorization</span></span>  | <span data-ttu-id="e34e6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e34e6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e34e6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e34e6-127">Content-Type</span></span>  | <span data-ttu-id="e34e6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e34e6-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e34e6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e34e6-129">Request body</span></span>
<span data-ttu-id="e34e6-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e34e6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e34e6-131">参数</span><span class="sxs-lookup"><span data-stu-id="e34e6-131">Parameter</span></span>    | <span data-ttu-id="e34e6-132">类型</span><span class="sxs-lookup"><span data-stu-id="e34e6-132">Type</span></span>   |<span data-ttu-id="e34e6-133">说明</span><span class="sxs-lookup"><span data-stu-id="e34e6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e34e6-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e34e6-134">securityEnabledOnly</span></span>|<span data-ttu-id="e34e6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e34e6-135">Boolean</span></span>|<span data-ttu-id="e34e6-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="e34e6-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="e34e6-138">响应</span><span class="sxs-lookup"><span data-stu-id="e34e6-138">Response</span></span>

<span data-ttu-id="e34e6-139">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200 OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="e34e6-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="e34e6-140">示例</span><span class="sxs-lookup"><span data-stu-id="e34e6-140">Example</span></span>
<span data-ttu-id="e34e6-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e34e6-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e34e6-142">请求</span><span class="sxs-lookup"><span data-stu-id="e34e6-142">Request</span></span>
<span data-ttu-id="e34e6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e34e6-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="e34e6-144">响应</span><span class="sxs-lookup"><span data-stu-id="e34e6-144">Response</span></span>
<span data-ttu-id="e34e6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e34e6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
