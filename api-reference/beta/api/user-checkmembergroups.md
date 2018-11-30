---
title: checkMemberGroups
description: 检查指定组的列表中的成员身份。 从列表中返回这些的组
ms.openlocfilehash: c6e232a6c34c0bbffdb41695a51694a688fecc7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041867"
---
# <a name="checkmembergroups"></a><span data-ttu-id="b1874-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b1874-104">checkMemberGroups</span></span>

> <span data-ttu-id="b1874-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1874-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1874-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1874-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1874-p103">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="b1874-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="b1874-p104">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="b1874-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1874-113">权限</span><span class="sxs-lookup"><span data-stu-id="b1874-113">Permissions</span></span>

<span data-ttu-id="b1874-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1874-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1874-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1874-116">Permission type</span></span>                        | <span data-ttu-id="b1874-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1874-117">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b1874-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1874-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1874-119">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b1874-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b1874-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1874-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1874-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1874-121">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="b1874-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1874-122">Application</span></span>                            | <span data-ttu-id="b1874-123">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1874-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="b1874-124">**注意：** 此 API 目前需要`Directory.Read.All`权限或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b1874-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="b1874-125">使用`User.Read.All`或`User.ReadWrite.All`权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="b1874-125">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="b1874-126">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="b1874-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1874-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1874-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="b1874-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1874-128">Request headers</span></span>

| <span data-ttu-id="b1874-129">标头</span><span class="sxs-lookup"><span data-stu-id="b1874-129">Header</span></span>        | <span data-ttu-id="b1874-130">值</span><span class="sxs-lookup"><span data-stu-id="b1874-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="b1874-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1874-131">Authorization</span></span> | <span data-ttu-id="b1874-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1874-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1874-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1874-134">Content-Type</span></span>  | <span data-ttu-id="b1874-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b1874-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="b1874-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1874-136">Request body</span></span>

<span data-ttu-id="b1874-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b1874-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1874-138">参数</span><span class="sxs-lookup"><span data-stu-id="b1874-138">Parameter</span></span> | <span data-ttu-id="b1874-139">类型</span><span class="sxs-lookup"><span data-stu-id="b1874-139">Type</span></span>   | <span data-ttu-id="b1874-140">说明</span><span class="sxs-lookup"><span data-stu-id="b1874-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="b1874-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="b1874-141">groupIds</span></span>  | <span data-ttu-id="b1874-142">String</span><span class="sxs-lookup"><span data-stu-id="b1874-142">String</span></span> | <span data-ttu-id="b1874-143">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="b1874-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="b1874-144">响应</span><span class="sxs-lookup"><span data-stu-id="b1874-144">Response</span></span>

<span data-ttu-id="b1874-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b1874-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1874-146">示例</span><span class="sxs-lookup"><span data-stu-id="b1874-146">Example</span></span>

<span data-ttu-id="b1874-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b1874-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b1874-148">请求</span><span class="sxs-lookup"><span data-stu-id="b1874-148">Request</span></span>

<span data-ttu-id="b1874-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1874-149">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b1874-150">响应</span><span class="sxs-lookup"><span data-stu-id="b1874-150">Response</span></span>

<span data-ttu-id="b1874-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1874-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
