---
title: 'user: getMemberGroups'
description: 返回所有组的成员的用户。 检查，可传递，与阅读不同
ms.openlocfilehash: 4ac810c6102fe848dc551a1c8fe3b754ee226f67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047931"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="2baf1-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2baf1-104">user: getMemberGroups</span></span>

> <span data-ttu-id="2baf1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2baf1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2baf1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2baf1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2baf1-p103">返回用户是其成员的所有组。检查是可传递的，这和读取 [memberOf](../api/user-list-memberof.md) 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p103">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="2baf1-p104">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="2baf1-113">权限</span><span class="sxs-lookup"><span data-stu-id="2baf1-113">Permissions</span></span>

<span data-ttu-id="2baf1-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2baf1-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="2baf1-116">Permission type</span></span>                        | <span data-ttu-id="2baf1-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2baf1-117">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2baf1-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2baf1-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="2baf1-119">~~User.Read 和 Group.Read.All~~、~~User.ReadBasic.All 和 Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2baf1-119">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2baf1-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2baf1-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2baf1-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="2baf1-121">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="2baf1-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="2baf1-122">Application</span></span>                            | <span data-ttu-id="2baf1-123">_Group.Read.All_、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2baf1-123">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="2baf1-124">**注意：** 此 API 目前需要`Directory.Read.All`权限或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2baf1-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="2baf1-125">单独或结合使用 Group.Read.All 权限，`User.`权限，将返回错误。</span><span class="sxs-lookup"><span data-stu-id="2baf1-125">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="2baf1-126">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="2baf1-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="2baf1-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2baf1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="2baf1-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="2baf1-128">Request headers</span></span>

| <span data-ttu-id="2baf1-129">标头</span><span class="sxs-lookup"><span data-stu-id="2baf1-129">Header</span></span>        | <span data-ttu-id="2baf1-130">值</span><span class="sxs-lookup"><span data-stu-id="2baf1-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2baf1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="2baf1-131">Authorization</span></span> | <span data-ttu-id="2baf1-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2baf1-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2baf1-134">Content-Type</span></span>  | <span data-ttu-id="2baf1-135">application/json</span><span class="sxs-lookup"><span data-stu-id="2baf1-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="2baf1-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="2baf1-136">Request body</span></span>

<span data-ttu-id="2baf1-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2baf1-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2baf1-138">参数</span><span class="sxs-lookup"><span data-stu-id="2baf1-138">Parameter</span></span>           | <span data-ttu-id="2baf1-139">类型</span><span class="sxs-lookup"><span data-stu-id="2baf1-139">Type</span></span>    | <span data-ttu-id="2baf1-140">说明</span><span class="sxs-lookup"><span data-stu-id="2baf1-140">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2baf1-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2baf1-141">securityEnabledOnly</span></span> | <span data-ttu-id="2baf1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2baf1-142">Boolean</span></span> | <span data-ttu-id="2baf1-p108">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p108">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="2baf1-145">响应</span><span class="sxs-lookup"><span data-stu-id="2baf1-145">Response</span></span>

<span data-ttu-id="2baf1-146">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="2baf1-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="2baf1-147">示例</span><span class="sxs-lookup"><span data-stu-id="2baf1-147">Example</span></span>

<span data-ttu-id="2baf1-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2baf1-148">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2baf1-149">请求</span><span class="sxs-lookup"><span data-stu-id="2baf1-149">Request</span></span>

<span data-ttu-id="2baf1-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2baf1-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="2baf1-151">响应</span><span class="sxs-lookup"><span data-stu-id="2baf1-151">Response</span></span>

<span data-ttu-id="2baf1-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2baf1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
