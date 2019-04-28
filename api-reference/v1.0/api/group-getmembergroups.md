---
title: 'group: getMemberGroups'
description: 返回指定组是其成员的所有组。 检查是可传递的，这和读取 memberOf 导航属性不同，后者仅返回该组是其直接成员的组。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 578caa1660ee86f24483cff9143a9153ca448526
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575882"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="365b6-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="365b6-104">group: getMemberGroups</span></span>

<span data-ttu-id="365b6-p102">返回指定组所属的所有组。检查是可传递的，这和读取 [memberOf](../api/group-list-memberof.md) 导航属性不同，后者仅返回该组是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="365b6-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="365b6-p103">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="365b6-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="365b6-111">权限</span><span class="sxs-lookup"><span data-stu-id="365b6-111">Permissions</span></span>

<span data-ttu-id="365b6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="365b6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="365b6-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="365b6-114">Permission type</span></span>                        | <span data-ttu-id="365b6-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="365b6-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="365b6-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="365b6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="365b6-117">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="365b6-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="365b6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="365b6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="365b6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="365b6-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="365b6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="365b6-120">Application</span></span>                            | <span data-ttu-id="365b6-121">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="365b6-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="365b6-122">**注意：** 此 API 当前需要 `Directory.Read.All` 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="365b6-122">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="365b6-123">使用 `Group.Read.All` 权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="365b6-123">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="365b6-124">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="365b6-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="365b6-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="365b6-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="365b6-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="365b6-126">Request headers</span></span>

| <span data-ttu-id="365b6-127">名称</span><span class="sxs-lookup"><span data-stu-id="365b6-127">Name</span></span>          | <span data-ttu-id="365b6-128">类型</span><span class="sxs-lookup"><span data-stu-id="365b6-128">Type</span></span>   | <span data-ttu-id="365b6-129">说明</span><span class="sxs-lookup"><span data-stu-id="365b6-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="365b6-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="365b6-130">Authorization</span></span> | <span data-ttu-id="365b6-131">string</span><span class="sxs-lookup"><span data-stu-id="365b6-131">string</span></span> | <span data-ttu-id="365b6-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="365b6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="365b6-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="365b6-134">Request body</span></span>

<span data-ttu-id="365b6-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="365b6-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="365b6-136">参数</span><span class="sxs-lookup"><span data-stu-id="365b6-136">Parameter</span></span>           | <span data-ttu-id="365b6-137">类型</span><span class="sxs-lookup"><span data-stu-id="365b6-137">Type</span></span>    | <span data-ttu-id="365b6-138">说明</span><span class="sxs-lookup"><span data-stu-id="365b6-138">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="365b6-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="365b6-139">securityEnabledOnly</span></span> | <span data-ttu-id="365b6-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="365b6-140">Boolean</span></span> | <span data-ttu-id="365b6-p107">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="365b6-p107">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="365b6-143">响应</span><span class="sxs-lookup"><span data-stu-id="365b6-143">Response</span></span>

<span data-ttu-id="365b6-144">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="365b6-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="365b6-145">示例</span><span class="sxs-lookup"><span data-stu-id="365b6-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="365b6-146">请求</span><span class="sxs-lookup"><span data-stu-id="365b6-146">Request</span></span>

<span data-ttu-id="365b6-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="365b6-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="365b6-148">响应</span><span class="sxs-lookup"><span data-stu-id="365b6-148">Response</span></span>

<span data-ttu-id="365b6-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="365b6-149">The following is an example of the response.</span></span>

> <span data-ttu-id="365b6-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="365b6-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="365b6-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="365b6-151">All the properties will be returned from an actual call.</span></span>

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
