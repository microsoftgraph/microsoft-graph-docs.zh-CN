---
title: 组：checkMemberGroups
description: 检查指定组的列表中的成员身份。 从列表中返回这些的组
author: dkershaw10
ms.openlocfilehash: 0868f8ed2b0b1bb1afaeb8741a8e7156608c6388
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348025"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="f87c7-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f87c7-104">group: checkMemberGroups</span></span>

> <span data-ttu-id="f87c7-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f87c7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f87c7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f87c7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f87c7-p103">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="f87c7-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="f87c7-p104">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="f87c7-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="f87c7-113">权限</span><span class="sxs-lookup"><span data-stu-id="f87c7-113">Permissions</span></span>

<span data-ttu-id="f87c7-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f87c7-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f87c7-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="f87c7-116">Permission type</span></span>                        | <span data-ttu-id="f87c7-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f87c7-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f87c7-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f87c7-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="f87c7-119">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f87c7-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f87c7-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f87c7-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f87c7-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="f87c7-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="f87c7-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="f87c7-122">Application</span></span>                            | <span data-ttu-id="f87c7-123">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87c7-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="f87c7-124">**注意：** 此 API 目前需要`Directory.Read.All`权限或更高版本。</span><span class="sxs-lookup"><span data-stu-id="f87c7-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="f87c7-125">使用`Group.Read.All`权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="f87c7-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="f87c7-126">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="f87c7-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="f87c7-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f87c7-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="f87c7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="f87c7-128">Request headers</span></span>

| <span data-ttu-id="f87c7-129">Name</span><span class="sxs-lookup"><span data-stu-id="f87c7-129">Name</span></span>          | <span data-ttu-id="f87c7-130">类型</span><span class="sxs-lookup"><span data-stu-id="f87c7-130">Type</span></span>   | <span data-ttu-id="f87c7-131">说明</span><span class="sxs-lookup"><span data-stu-id="f87c7-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f87c7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f87c7-132">Authorization</span></span> | <span data-ttu-id="f87c7-133">string</span><span class="sxs-lookup"><span data-stu-id="f87c7-133">string</span></span> | <span data-ttu-id="f87c7-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f87c7-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f87c7-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="f87c7-136">Request body</span></span>

<span data-ttu-id="f87c7-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f87c7-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f87c7-138">参数</span><span class="sxs-lookup"><span data-stu-id="f87c7-138">Parameter</span></span> | <span data-ttu-id="f87c7-139">Type</span><span class="sxs-lookup"><span data-stu-id="f87c7-139">Type</span></span>   | <span data-ttu-id="f87c7-140">说明</span><span class="sxs-lookup"><span data-stu-id="f87c7-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="f87c7-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="f87c7-141">groupIds</span></span>  | <span data-ttu-id="f87c7-142">String</span><span class="sxs-lookup"><span data-stu-id="f87c7-142">String</span></span> | <span data-ttu-id="f87c7-143">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="f87c7-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="f87c7-144">响应</span><span class="sxs-lookup"><span data-stu-id="f87c7-144">Response</span></span>

<span data-ttu-id="f87c7-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="f87c7-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f87c7-146">示例</span><span class="sxs-lookup"><span data-stu-id="f87c7-146">Example</span></span>

<span data-ttu-id="f87c7-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f87c7-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f87c7-148">请求</span><span class="sxs-lookup"><span data-stu-id="f87c7-148">Request</span></span>

<span data-ttu-id="f87c7-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f87c7-149">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f87c7-150">响应</span><span class="sxs-lookup"><span data-stu-id="f87c7-150">Response</span></span>

<span data-ttu-id="f87c7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f87c7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
