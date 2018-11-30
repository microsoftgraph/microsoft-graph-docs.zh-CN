---
title: 'user: getMemberObjects'
description: 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。
ms.openlocfilehash: 337bf806be40b5e0af3600ea5fbeab5e94c079b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041265"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="a0b1b-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a0b1b-104">user: getMemberObjects</span></span>

> <span data-ttu-id="a0b1b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0b1b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0b1b-p103">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0b1b-109">权限</span><span class="sxs-lookup"><span data-stu-id="a0b1b-109">Permissions</span></span>
<span data-ttu-id="a0b1b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a0b1b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0b1b-112">Permission type</span></span>      | <span data-ttu-id="a0b1b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0b1b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0b1b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0b1b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a0b1b-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0b1b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0b1b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0b1b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0b1b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-117">Not supported.</span></span>    |
|<span data-ttu-id="a0b1b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0b1b-118">Application</span></span> | <span data-ttu-id="a0b1b-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0b1b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0b1b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0b1b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="a0b1b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0b1b-121">Request headers</span></span>
| <span data-ttu-id="a0b1b-122">标头</span><span class="sxs-lookup"><span data-stu-id="a0b1b-122">Header</span></span>       | <span data-ttu-id="a0b1b-123">值</span><span class="sxs-lookup"><span data-stu-id="a0b1b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0b1b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0b1b-124">Authorization</span></span>  | <span data-ttu-id="a0b1b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0b1b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0b1b-127">Content-Type</span></span>  | <span data-ttu-id="a0b1b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a0b1b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0b1b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0b1b-129">Request body</span></span>
<span data-ttu-id="a0b1b-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a0b1b-131">参数</span><span class="sxs-lookup"><span data-stu-id="a0b1b-131">Parameter</span></span>    | <span data-ttu-id="a0b1b-132">类型</span><span class="sxs-lookup"><span data-stu-id="a0b1b-132">Type</span></span>   |<span data-ttu-id="a0b1b-133">说明</span><span class="sxs-lookup"><span data-stu-id="a0b1b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0b1b-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a0b1b-134">securityEnabledOnly</span></span>|<span data-ttu-id="a0b1b-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b1b-135">Boolean</span></span>|<span data-ttu-id="a0b1b-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="a0b1b-138">响应</span><span class="sxs-lookup"><span data-stu-id="a0b1b-138">Response</span></span>

<span data-ttu-id="a0b1b-139">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200 OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a0b1b-140">示例</span><span class="sxs-lookup"><span data-stu-id="a0b1b-140">Example</span></span>
<span data-ttu-id="a0b1b-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a0b1b-142">请求</span><span class="sxs-lookup"><span data-stu-id="a0b1b-142">Request</span></span>
<span data-ttu-id="a0b1b-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a0b1b-144">响应</span><span class="sxs-lookup"><span data-stu-id="a0b1b-144">Response</span></span>
<span data-ttu-id="a0b1b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0b1b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
