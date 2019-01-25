---
title: 'user: getMemberGroups'
description: 返回用户是其成员的所有组。 检查是可传递的，这不同于读取
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 292a7e6c9ed0d67ced657dd726d9f41b32eac458
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517594"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="2a8e4-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2a8e4-104">user: getMemberGroups</span></span>

<span data-ttu-id="2a8e4-p102">返回用户是其成员的所有组。检查是可传递的，这和读取 [memberOf](../api/user-list-memberof.md) 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="2a8e4-p103">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a8e4-111">权限</span><span class="sxs-lookup"><span data-stu-id="2a8e4-111">Permissions</span></span>

<span data-ttu-id="2a8e4-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a8e4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a8e4-114">Permission type</span></span>                        | <span data-ttu-id="2a8e4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a8e4-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2a8e4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a8e4-116">Delegated (work or school account)</span></span>     |  <span data-ttu-id="2a8e4-117">User.Read、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a8e4-117">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2a8e4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a8e4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a8e4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="2a8e4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a8e4-120">Application</span></span>                            | <span data-ttu-id="2a8e4-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8e4-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

## <a name="http-request"></a><span data-ttu-id="2a8e4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a8e4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="2a8e4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a8e4-123">Request headers</span></span>

| <span data-ttu-id="2a8e4-124">标头</span><span class="sxs-lookup"><span data-stu-id="2a8e4-124">Header</span></span>        | <span data-ttu-id="2a8e4-125">值</span><span class="sxs-lookup"><span data-stu-id="2a8e4-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2a8e4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a8e4-126">Authorization</span></span> | <span data-ttu-id="2a8e4-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a8e4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a8e4-129">Content-Type</span></span>  | <span data-ttu-id="2a8e4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="2a8e4-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="2a8e4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a8e4-131">Request body</span></span>

<span data-ttu-id="2a8e4-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a8e4-133">参数</span><span class="sxs-lookup"><span data-stu-id="2a8e4-133">Parameter</span></span>           | <span data-ttu-id="2a8e4-134">类型</span><span class="sxs-lookup"><span data-stu-id="2a8e4-134">Type</span></span>    | <span data-ttu-id="2a8e4-135">说明</span><span class="sxs-lookup"><span data-stu-id="2a8e4-135">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2a8e4-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2a8e4-136">securityEnabledOnly</span></span> | <span data-ttu-id="2a8e4-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a8e4-137">Boolean</span></span> | <span data-ttu-id="2a8e4-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="2a8e4-140">响应</span><span class="sxs-lookup"><span data-stu-id="2a8e4-140">Response</span></span>

<span data-ttu-id="2a8e4-141">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="2a8e4-142">示例</span><span class="sxs-lookup"><span data-stu-id="2a8e4-142">Example</span></span>

<span data-ttu-id="2a8e4-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2a8e4-144">请求</span><span class="sxs-lookup"><span data-stu-id="2a8e4-144">Request</span></span>

<span data-ttu-id="2a8e4-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2a8e4-146">响应</span><span class="sxs-lookup"><span data-stu-id="2a8e4-146">Response</span></span>

<span data-ttu-id="2a8e4-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
