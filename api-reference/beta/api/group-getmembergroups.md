---
title: 'group: getMemberGroups'
description: 返回指定组所属的所有组。检查是可传递的，这和读取 memberOf 导航属性不同，后者仅返回该组是其直接成员的组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e485c80a06fc2d124dec728ab3ffcdfb8dcce105
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921533"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="3e82c-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3e82c-104">group: getMemberGroups</span></span>

> <span data-ttu-id="3e82c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e82c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e82c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e82c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e82c-p103">返回指定组所属的所有组。检查是可传递的，这和读取 [memberOf](../api/group-list-memberof.md) 导航属性不同，后者仅返回该组是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p103">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="3e82c-p104">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e82c-113">权限</span><span class="sxs-lookup"><span data-stu-id="3e82c-113">Permissions</span></span>

<span data-ttu-id="3e82c-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e82c-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-116">Permission type</span></span>                        | <span data-ttu-id="3e82c-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e82c-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="3e82c-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e82c-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e82c-119">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3e82c-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="3e82c-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e82c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e82c-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e82c-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="3e82c-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e82c-122">Application</span></span>                            | <span data-ttu-id="3e82c-123">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e82c-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="3e82c-124">**注意：** 此 API 目前需要`Directory.Read.All`权限或更高版本。</span><span class="sxs-lookup"><span data-stu-id="3e82c-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="3e82c-125">使用`Group.Read.All`权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="3e82c-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="3e82c-126">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="3e82c-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e82c-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e82c-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="3e82c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e82c-128">Request headers</span></span>

| <span data-ttu-id="3e82c-129">名称</span><span class="sxs-lookup"><span data-stu-id="3e82c-129">Name</span></span>          | <span data-ttu-id="3e82c-130">类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-130">Type</span></span>   | <span data-ttu-id="3e82c-131">说明</span><span class="sxs-lookup"><span data-stu-id="3e82c-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3e82c-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e82c-132">Authorization</span></span> | <span data-ttu-id="3e82c-133">string</span><span class="sxs-lookup"><span data-stu-id="3e82c-133">string</span></span> | <span data-ttu-id="3e82c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e82c-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e82c-136">Request body</span></span>

<span data-ttu-id="3e82c-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3e82c-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e82c-138">参数</span><span class="sxs-lookup"><span data-stu-id="3e82c-138">Parameter</span></span>           | <span data-ttu-id="3e82c-139">类型</span><span class="sxs-lookup"><span data-stu-id="3e82c-139">Type</span></span>    | <span data-ttu-id="3e82c-140">说明</span><span class="sxs-lookup"><span data-stu-id="3e82c-140">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="3e82c-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="3e82c-141">securityEnabledOnly</span></span> | <span data-ttu-id="3e82c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e82c-142">Boolean</span></span> | <span data-ttu-id="3e82c-p108">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p108">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="3e82c-145">响应</span><span class="sxs-lookup"><span data-stu-id="3e82c-145">Response</span></span>

<span data-ttu-id="3e82c-146">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="3e82c-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="3e82c-147">示例</span><span class="sxs-lookup"><span data-stu-id="3e82c-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3e82c-148">请求</span><span class="sxs-lookup"><span data-stu-id="3e82c-148">Request</span></span>

<span data-ttu-id="3e82c-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e82c-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="3e82c-150">响应</span><span class="sxs-lookup"><span data-stu-id="3e82c-150">Response</span></span>

<span data-ttu-id="3e82c-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e82c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="3e82c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3e82c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
