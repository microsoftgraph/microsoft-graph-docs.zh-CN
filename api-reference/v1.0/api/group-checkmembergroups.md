---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Priority
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b2ad7dd8e98c88ed428f9a61287027b49f5a73c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517227"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="3c16e-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3c16e-104">group: checkMemberGroups</span></span>

<span data-ttu-id="3c16e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c16e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c16e-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="3c16e-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c16e-112">权限</span><span class="sxs-lookup"><span data-stu-id="3c16e-112">Permissions</span></span>

<span data-ttu-id="3c16e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c16e-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c16e-115">Permission type</span></span>                        | <span data-ttu-id="3c16e-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c16e-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="3c16e-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c16e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c16e-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c16e-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="3c16e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c16e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c16e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c16e-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="3c16e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c16e-121">Application</span></span>                            | <span data-ttu-id="3c16e-122">GroupMember.Read.All、Group.Read.All、Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="3c16e-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="3c16e-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c16e-123">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="3c16e-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c16e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="3c16e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c16e-125">Request headers</span></span>

| <span data-ttu-id="3c16e-126">名称</span><span class="sxs-lookup"><span data-stu-id="3c16e-126">Name</span></span>          | <span data-ttu-id="3c16e-127">类型</span><span class="sxs-lookup"><span data-stu-id="3c16e-127">Type</span></span>   | <span data-ttu-id="3c16e-128">说明</span><span class="sxs-lookup"><span data-stu-id="3c16e-128">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3c16e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c16e-129">Authorization</span></span> | <span data-ttu-id="3c16e-130">string</span><span class="sxs-lookup"><span data-stu-id="3c16e-130">string</span></span> | <span data-ttu-id="3c16e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c16e-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c16e-133">Request body</span></span>

<span data-ttu-id="3c16e-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3c16e-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c16e-135">参数</span><span class="sxs-lookup"><span data-stu-id="3c16e-135">Parameter</span></span> | <span data-ttu-id="3c16e-136">类型</span><span class="sxs-lookup"><span data-stu-id="3c16e-136">Type</span></span>              | <span data-ttu-id="3c16e-137">说明</span><span class="sxs-lookup"><span data-stu-id="3c16e-137">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="3c16e-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="3c16e-138">groupIds</span></span>  | <span data-ttu-id="3c16e-139">String collection</span><span class="sxs-lookup"><span data-stu-id="3c16e-139">String collection</span></span> | <span data-ttu-id="3c16e-140">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="3c16e-140">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="3c16e-141">响应</span><span class="sxs-lookup"><span data-stu-id="3c16e-141">Response</span></span>

<span data-ttu-id="3c16e-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="3c16e-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c16e-143">示例</span><span class="sxs-lookup"><span data-stu-id="3c16e-143">Example</span></span>

<span data-ttu-id="3c16e-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3c16e-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3c16e-145">请求</span><span class="sxs-lookup"><span data-stu-id="3c16e-145">Request</span></span>

<span data-ttu-id="3c16e-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c16e-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c16e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c16e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3c16e-148">C#</span><span class="sxs-lookup"><span data-stu-id="3c16e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c16e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c16e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c16e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c16e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c16e-151">Java</span><span class="sxs-lookup"><span data-stu-id="3c16e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c16e-152">响应</span><span class="sxs-lookup"><span data-stu-id="3c16e-152">Response</span></span>

<span data-ttu-id="3c16e-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
