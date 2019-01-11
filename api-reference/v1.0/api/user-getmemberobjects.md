---
title: 'user: getMemberObjects'
description: 返回用户所属的所有组、目录角色和管理单元。检查是可传递的。
localization_priority: Priority
ms.openlocfilehash: 2d2c28ab41e7f9798ff1f77e1750e6303a52de34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811380"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="a06ba-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a06ba-104">user: getMemberObjects</span></span>
<span data-ttu-id="a06ba-p102">返回用户所属的所有组、目录角色和管理单元。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="a06ba-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a06ba-107">权限</span><span class="sxs-lookup"><span data-stu-id="a06ba-107">Permissions</span></span>
<span data-ttu-id="a06ba-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a06ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a06ba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a06ba-110">Permission type</span></span>      | <span data-ttu-id="a06ba-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a06ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a06ba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a06ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a06ba-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a06ba-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a06ba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a06ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a06ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a06ba-115">Not supported.</span></span>    |
|<span data-ttu-id="a06ba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a06ba-116">Application</span></span> | <span data-ttu-id="a06ba-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06ba-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a06ba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a06ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="a06ba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a06ba-119">Request headers</span></span>
| <span data-ttu-id="a06ba-120">标头</span><span class="sxs-lookup"><span data-stu-id="a06ba-120">Header</span></span>       | <span data-ttu-id="a06ba-121">值</span><span class="sxs-lookup"><span data-stu-id="a06ba-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a06ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a06ba-122">Authorization</span></span>  | <span data-ttu-id="a06ba-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a06ba-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a06ba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a06ba-125">Content-Type</span></span>  | <span data-ttu-id="a06ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a06ba-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a06ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a06ba-127">Request body</span></span>
<span data-ttu-id="a06ba-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a06ba-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a06ba-129">参数</span><span class="sxs-lookup"><span data-stu-id="a06ba-129">Parameter</span></span>    | <span data-ttu-id="a06ba-130">类型</span><span class="sxs-lookup"><span data-stu-id="a06ba-130">Type</span></span>   |<span data-ttu-id="a06ba-131">说明</span><span class="sxs-lookup"><span data-stu-id="a06ba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a06ba-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a06ba-132">securityEnabledOnly</span></span>|<span data-ttu-id="a06ba-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a06ba-133">Boolean</span></span>|<span data-ttu-id="a06ba-p105">**true** 指定仅应返回用户所属的安全组；**false** 指定应返回用户所属的所有组和目录角色。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a06ba-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="a06ba-136">响应</span><span class="sxs-lookup"><span data-stu-id="a06ba-136">Response</span></span>

<span data-ttu-id="a06ba-137">如果成功，此方法将在包含该用户所属组和目录角色 ID 的响应正文中返回 `200 OK` 响应代码和 String 集合。</span><span class="sxs-lookup"><span data-stu-id="a06ba-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a06ba-138">示例</span><span class="sxs-lookup"><span data-stu-id="a06ba-138">Example</span></span>
<span data-ttu-id="a06ba-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a06ba-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a06ba-140">请求</span><span class="sxs-lookup"><span data-stu-id="a06ba-140">Request</span></span>
<span data-ttu-id="a06ba-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a06ba-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a06ba-142">响应</span><span class="sxs-lookup"><span data-stu-id="a06ba-142">Response</span></span>
<span data-ttu-id="a06ba-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a06ba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
