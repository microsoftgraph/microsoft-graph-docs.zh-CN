---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1815f187a25eaddbd3b1757fde5e7e4e9c74f650
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329620"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="50281-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="50281-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50281-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="50281-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="50281-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="50281-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="50281-111">权限</span><span class="sxs-lookup"><span data-stu-id="50281-111">Permissions</span></span>

<span data-ttu-id="50281-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50281-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50281-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="50281-114">Permission type</span></span>                        | <span data-ttu-id="50281-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50281-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="50281-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50281-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="50281-117">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50281-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="50281-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50281-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50281-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="50281-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="50281-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="50281-120">Application</span></span>                            | <span data-ttu-id="50281-121">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50281-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="50281-122">**注意：** 此 API 当前需要 `Directory.Read.All` 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="50281-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="50281-123">使用 `Group.Read.All` 权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="50281-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="50281-124">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="50281-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="50281-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50281-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="50281-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="50281-126">Request headers</span></span>

| <span data-ttu-id="50281-127">名称</span><span class="sxs-lookup"><span data-stu-id="50281-127">Name</span></span>          | <span data-ttu-id="50281-128">类型</span><span class="sxs-lookup"><span data-stu-id="50281-128">Type</span></span>   | <span data-ttu-id="50281-129">说明</span><span class="sxs-lookup"><span data-stu-id="50281-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="50281-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="50281-130">Authorization</span></span> | <span data-ttu-id="50281-131">string</span><span class="sxs-lookup"><span data-stu-id="50281-131">string</span></span> | <span data-ttu-id="50281-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50281-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50281-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="50281-134">Request body</span></span>

<span data-ttu-id="50281-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="50281-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50281-136">参数</span><span class="sxs-lookup"><span data-stu-id="50281-136">Parameter</span></span> | <span data-ttu-id="50281-137">类型</span><span class="sxs-lookup"><span data-stu-id="50281-137">Type</span></span>   | <span data-ttu-id="50281-138">说明</span><span class="sxs-lookup"><span data-stu-id="50281-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="50281-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="50281-139">groupIds</span></span>  | <span data-ttu-id="50281-140">String collection</span><span class="sxs-lookup"><span data-stu-id="50281-140">String collection</span></span> | <span data-ttu-id="50281-141">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="50281-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="50281-142">响应</span><span class="sxs-lookup"><span data-stu-id="50281-142">Response</span></span>

<span data-ttu-id="50281-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="50281-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50281-144">示例</span><span class="sxs-lookup"><span data-stu-id="50281-144">Example</span></span>

<span data-ttu-id="50281-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="50281-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="50281-146">请求</span><span class="sxs-lookup"><span data-stu-id="50281-146">Request</span></span>

<span data-ttu-id="50281-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50281-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="50281-148">响应</span><span class="sxs-lookup"><span data-stu-id="50281-148">Response</span></span>

<span data-ttu-id="50281-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50281-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
