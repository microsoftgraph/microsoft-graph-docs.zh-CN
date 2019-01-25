---
title: checkMemberGroups
description: 检查指定组的列表中的成员身份。 从列表中返回这些的组
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d7452795cb0a8ffdf3a966a3e350a8634b2a7ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516894"
---
# <a name="checkmembergroups"></a><span data-ttu-id="585f5-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="585f5-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585f5-p102">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="585f5-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="585f5-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="585f5-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="585f5-111">权限</span><span class="sxs-lookup"><span data-stu-id="585f5-111">Permissions</span></span>

<span data-ttu-id="585f5-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="585f5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="585f5-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="585f5-114">Permission type</span></span>                        | <span data-ttu-id="585f5-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="585f5-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="585f5-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="585f5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="585f5-117">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="585f5-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="585f5-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="585f5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="585f5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="585f5-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="585f5-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="585f5-120">Application</span></span>                            | <span data-ttu-id="585f5-121">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="585f5-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="585f5-122">**注意：** 此 API 当前需要 `Directory.Read.All` 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="585f5-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="585f5-123">使用`User.Read.All`或`User.ReadWrite.All`权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="585f5-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="585f5-124">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="585f5-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="585f5-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="585f5-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="585f5-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="585f5-126">Request headers</span></span>

| <span data-ttu-id="585f5-127">标头</span><span class="sxs-lookup"><span data-stu-id="585f5-127">Header</span></span>        | <span data-ttu-id="585f5-128">值</span><span class="sxs-lookup"><span data-stu-id="585f5-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="585f5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="585f5-129">Authorization</span></span> | <span data-ttu-id="585f5-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="585f5-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="585f5-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="585f5-132">Content-Type</span></span>  | <span data-ttu-id="585f5-133">application/json</span><span class="sxs-lookup"><span data-stu-id="585f5-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="585f5-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="585f5-134">Request body</span></span>

<span data-ttu-id="585f5-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="585f5-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="585f5-136">参数</span><span class="sxs-lookup"><span data-stu-id="585f5-136">Parameter</span></span> | <span data-ttu-id="585f5-137">类型</span><span class="sxs-lookup"><span data-stu-id="585f5-137">Type</span></span>   | <span data-ttu-id="585f5-138">说明</span><span class="sxs-lookup"><span data-stu-id="585f5-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="585f5-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="585f5-139">groupIds</span></span>  | <span data-ttu-id="585f5-140">String</span><span class="sxs-lookup"><span data-stu-id="585f5-140">String</span></span> | <span data-ttu-id="585f5-141">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="585f5-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="585f5-142">响应</span><span class="sxs-lookup"><span data-stu-id="585f5-142">Response</span></span>

<span data-ttu-id="585f5-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="585f5-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="585f5-144">示例</span><span class="sxs-lookup"><span data-stu-id="585f5-144">Example</span></span>

<span data-ttu-id="585f5-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="585f5-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="585f5-146">请求</span><span class="sxs-lookup"><span data-stu-id="585f5-146">Request</span></span>

<span data-ttu-id="585f5-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="585f5-147">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="585f5-148">响应</span><span class="sxs-lookup"><span data-stu-id="585f5-148">Response</span></span>

<span data-ttu-id="585f5-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="585f5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
