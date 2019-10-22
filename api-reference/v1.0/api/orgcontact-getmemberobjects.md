---
title: orgContact： getMemberObjects
description: 返回此组织联系人所属的所有组。 检查是可传递的。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 204858fbd6bcc08c6f7385e098173387c9182e14
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622600"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="c03fd-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c03fd-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="c03fd-105">返回此[组织联系人](../resources/orgcontact.md)所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="c03fd-105">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="c03fd-106">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="c03fd-106">The check is transitive.</span></span> <span data-ttu-id="c03fd-107">组织联系人不能是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="c03fd-107">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="c03fd-108">将不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="c03fd-108">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c03fd-109">权限</span><span class="sxs-lookup"><span data-stu-id="c03fd-109">Permissions</span></span>
<span data-ttu-id="c03fd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c03fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c03fd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c03fd-112">Permission type</span></span>      | <span data-ttu-id="c03fd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c03fd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c03fd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c03fd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c03fd-115">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="c03fd-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="c03fd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c03fd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c03fd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c03fd-117">Not supported.</span></span>    |
|<span data-ttu-id="c03fd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c03fd-118">Application</span></span> | <span data-ttu-id="c03fd-119">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="c03fd-119">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c03fd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c03fd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="c03fd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c03fd-121">Request headers</span></span>
| <span data-ttu-id="c03fd-122">标头</span><span class="sxs-lookup"><span data-stu-id="c03fd-122">Header</span></span>       | <span data-ttu-id="c03fd-123">值</span><span class="sxs-lookup"><span data-stu-id="c03fd-123">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c03fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c03fd-124">Authorization</span></span>  | <span data-ttu-id="c03fd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c03fd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c03fd-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="c03fd-127">Content-type</span></span>   | <span data-ttu-id="c03fd-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c03fd-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c03fd-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c03fd-130">Request body</span></span>
<span data-ttu-id="c03fd-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c03fd-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c03fd-132">参数</span><span class="sxs-lookup"><span data-stu-id="c03fd-132">Parameter</span></span>    | <span data-ttu-id="c03fd-133">类型</span><span class="sxs-lookup"><span data-stu-id="c03fd-133">Type</span></span>   |<span data-ttu-id="c03fd-134">说明</span><span class="sxs-lookup"><span data-stu-id="c03fd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c03fd-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c03fd-135">securityEnabledOnly</span></span>|<span data-ttu-id="c03fd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c03fd-136">Boolean</span></span>|<span data-ttu-id="c03fd-137">设置为`false`。</span><span class="sxs-lookup"><span data-stu-id="c03fd-137">Set to `false`.</span></span> <span data-ttu-id="c03fd-138">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="c03fd-138">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="c03fd-139">响应</span><span class="sxs-lookup"><span data-stu-id="c03fd-139">Response</span></span>

<span data-ttu-id="c03fd-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="c03fd-140">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c03fd-141">示例</span><span class="sxs-lookup"><span data-stu-id="c03fd-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c03fd-142">请求</span><span class="sxs-lookup"><span data-stu-id="c03fd-142">Request</span></span>
<span data-ttu-id="c03fd-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c03fd-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

##### <a name="response"></a><span data-ttu-id="c03fd-144">响应</span><span class="sxs-lookup"><span data-stu-id="c03fd-144">Response</span></span>
<span data-ttu-id="c03fd-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c03fd-145">The following is an example of the response.</span></span>
><span data-ttu-id="c03fd-146">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c03fd-146">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
