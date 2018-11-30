---
title: 'orgContact: checkMemberGroups'
description: 需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅权限。
ms.openlocfilehash: d064775772bb05963e3cd789346e32bf80b7587c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045387"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="8a7c0-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8a7c0-104">orgContact: checkMemberGroups</span></span>

> <span data-ttu-id="8a7c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a7c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a7c0-107">权限</span><span class="sxs-lookup"><span data-stu-id="8a7c0-107">Permissions</span></span>
<span data-ttu-id="8a7c0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a7c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a7c0-110">Permission type</span></span>      | <span data-ttu-id="8a7c0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a7c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a7c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a7c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a7c0-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a7c0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a7c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a7c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a7c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-115">Not supported.</span></span>    |
|<span data-ttu-id="8a7c0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a7c0-116">Application</span></span> | <span data-ttu-id="8a7c0-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7c0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a7c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a7c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="8a7c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a7c0-119">Request headers</span></span>
| <span data-ttu-id="8a7c0-120">名称</span><span class="sxs-lookup"><span data-stu-id="8a7c0-120">Name</span></span>       | <span data-ttu-id="8a7c0-121">类型</span><span class="sxs-lookup"><span data-stu-id="8a7c0-121">Type</span></span> | <span data-ttu-id="8a7c0-122">说明</span><span class="sxs-lookup"><span data-stu-id="8a7c0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8a7c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a7c0-123">Authorization</span></span>  | <span data-ttu-id="8a7c0-124">string</span><span class="sxs-lookup"><span data-stu-id="8a7c0-124">string</span></span>  | <span data-ttu-id="8a7c0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a7c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a7c0-127">Request body</span></span>
<span data-ttu-id="8a7c0-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8a7c0-129">参数</span><span class="sxs-lookup"><span data-stu-id="8a7c0-129">Parameter</span></span>    | <span data-ttu-id="8a7c0-130">类型</span><span class="sxs-lookup"><span data-stu-id="8a7c0-130">Type</span></span>   |<span data-ttu-id="8a7c0-131">说明</span><span class="sxs-lookup"><span data-stu-id="8a7c0-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a7c0-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="8a7c0-132">groupIds</span></span>|<span data-ttu-id="8a7c0-133">String</span><span class="sxs-lookup"><span data-stu-id="8a7c0-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="8a7c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="8a7c0-134">Response</span></span>

<span data-ttu-id="8a7c0-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a7c0-136">示例</span><span class="sxs-lookup"><span data-stu-id="8a7c0-136">Example</span></span>
<span data-ttu-id="8a7c0-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a7c0-138">请求</span><span class="sxs-lookup"><span data-stu-id="8a7c0-138">Request</span></span>
<span data-ttu-id="8a7c0-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8a7c0-140">响应</span><span class="sxs-lookup"><span data-stu-id="8a7c0-140">Response</span></span>
<span data-ttu-id="8a7c0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a7c0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->