---
title: 'orgContact: getMemberObjects'
description: >
  需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅权限。
localization_priority: Normal
ms.openlocfilehash: ac6c8fddf4cedae156ec25933ea8d9f95bf8020a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856572"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="33946-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="33946-104">orgContact: getMemberObjects</span></span>

> <span data-ttu-id="33946-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="33946-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33946-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="33946-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="33946-107">权限</span><span class="sxs-lookup"><span data-stu-id="33946-107">Permissions</span></span>
<span data-ttu-id="33946-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33946-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33946-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="33946-110">Permission type</span></span>      | <span data-ttu-id="33946-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33946-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33946-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33946-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33946-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33946-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33946-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33946-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33946-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="33946-115">Not supported.</span></span>    |
|<span data-ttu-id="33946-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="33946-116">Application</span></span> | <span data-ttu-id="33946-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33946-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33946-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33946-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="33946-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="33946-119">Request headers</span></span>
| <span data-ttu-id="33946-120">名称</span><span class="sxs-lookup"><span data-stu-id="33946-120">Name</span></span>       | <span data-ttu-id="33946-121">类型</span><span class="sxs-lookup"><span data-stu-id="33946-121">Type</span></span> | <span data-ttu-id="33946-122">说明</span><span class="sxs-lookup"><span data-stu-id="33946-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33946-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="33946-123">Authorization</span></span>  | <span data-ttu-id="33946-124">string</span><span class="sxs-lookup"><span data-stu-id="33946-124">string</span></span>  | <span data-ttu-id="33946-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33946-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33946-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="33946-127">Request body</span></span>
<span data-ttu-id="33946-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="33946-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33946-129">参数</span><span class="sxs-lookup"><span data-stu-id="33946-129">Parameter</span></span>    | <span data-ttu-id="33946-130">类型</span><span class="sxs-lookup"><span data-stu-id="33946-130">Type</span></span>   |<span data-ttu-id="33946-131">说明</span><span class="sxs-lookup"><span data-stu-id="33946-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33946-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="33946-132">securityEnabledOnly</span></span>|<span data-ttu-id="33946-133">布尔</span><span class="sxs-lookup"><span data-stu-id="33946-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="33946-134">响应</span><span class="sxs-lookup"><span data-stu-id="33946-134">Response</span></span>

<span data-ttu-id="33946-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="33946-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33946-136">示例</span><span class="sxs-lookup"><span data-stu-id="33946-136">Example</span></span>
<span data-ttu-id="33946-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="33946-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33946-138">请求</span><span class="sxs-lookup"><span data-stu-id="33946-138">Request</span></span>
<span data-ttu-id="33946-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33946-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="33946-140">响应</span><span class="sxs-lookup"><span data-stu-id="33946-140">Response</span></span>
<span data-ttu-id="33946-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33946-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
