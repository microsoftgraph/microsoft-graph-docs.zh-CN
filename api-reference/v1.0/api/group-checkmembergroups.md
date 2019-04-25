---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 8abac44bf6c97e0ebbd8235ec246f19f0c73e920
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524181"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="60af7-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="60af7-104">group: checkMemberGroups</span></span>

<span data-ttu-id="60af7-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="60af7-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="60af7-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="60af7-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="60af7-111">权限</span><span class="sxs-lookup"><span data-stu-id="60af7-111">Permissions</span></span>

<span data-ttu-id="60af7-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60af7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60af7-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="60af7-114">Permission type</span></span>                        | <span data-ttu-id="60af7-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60af7-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="60af7-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60af7-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="60af7-117">~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60af7-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="60af7-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60af7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60af7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="60af7-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="60af7-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="60af7-120">Application</span></span>                            | <span data-ttu-id="60af7-121">_Group.Read.All_, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="60af7-121">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span> <span data-ttu-id="60af7-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60af7-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="60af7-123">**注意：** 此 API 当前需要 `Directory.Read.All` 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="60af7-123">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="60af7-124">使用 `Group.Read.All` 权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="60af7-124">Using the Group.Read.All permission will return an error.</span></span> <span data-ttu-id="60af7-125">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="60af7-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="60af7-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60af7-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="60af7-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="60af7-127">Request headers</span></span>

| <span data-ttu-id="60af7-128">名称</span><span class="sxs-lookup"><span data-stu-id="60af7-128">Name</span></span>          | <span data-ttu-id="60af7-129">类型</span><span class="sxs-lookup"><span data-stu-id="60af7-129">Type</span></span>   | <span data-ttu-id="60af7-130">说明</span><span class="sxs-lookup"><span data-stu-id="60af7-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="60af7-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="60af7-131">Authorization</span></span> | <span data-ttu-id="60af7-132">string</span><span class="sxs-lookup"><span data-stu-id="60af7-132">string</span></span> | <span data-ttu-id="60af7-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60af7-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60af7-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="60af7-135">Request body</span></span>

<span data-ttu-id="60af7-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="60af7-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60af7-137">参数</span><span class="sxs-lookup"><span data-stu-id="60af7-137">Parameter</span></span> | <span data-ttu-id="60af7-138">类型</span><span class="sxs-lookup"><span data-stu-id="60af7-138">Type</span></span>              | <span data-ttu-id="60af7-139">说明</span><span class="sxs-lookup"><span data-stu-id="60af7-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="60af7-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="60af7-140">groupIds</span></span>  | <span data-ttu-id="60af7-141">String collection</span><span class="sxs-lookup"><span data-stu-id="60af7-141">String collection</span></span> | <span data-ttu-id="60af7-142">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="60af7-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="60af7-143">响应</span><span class="sxs-lookup"><span data-stu-id="60af7-143">Response</span></span>

<span data-ttu-id="60af7-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="60af7-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60af7-145">示例</span><span class="sxs-lookup"><span data-stu-id="60af7-145">Example</span></span>

<span data-ttu-id="60af7-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="60af7-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="60af7-147">请求</span><span class="sxs-lookup"><span data-stu-id="60af7-147">Request</span></span>

<span data-ttu-id="60af7-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60af7-148">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="60af7-149">响应</span><span class="sxs-lookup"><span data-stu-id="60af7-149">Response</span></span>

<span data-ttu-id="60af7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60af7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
