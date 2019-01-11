---
title: 'servicePrincipal: checkMemberGroups'
description: >
  需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅权限。
localization_priority: Normal
ms.openlocfilehash: f9eb06fdb871c2466dec753e3c3deb9c8f1b1590
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852498"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="dc4dd-104">servicePrincipal: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="dc4dd-104">servicePrincipal: checkMemberGroups</span></span>

> <span data-ttu-id="dc4dd-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc4dd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc4dd-107">权限</span><span class="sxs-lookup"><span data-stu-id="dc4dd-107">Permissions</span></span>
<span data-ttu-id="dc4dd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc4dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc4dd-110">Permission type</span></span>      | <span data-ttu-id="dc4dd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc4dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc4dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4dd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dc4dd-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc4dd-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc4dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4dd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc4dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-115">Not supported.</span></span>    |
|<span data-ttu-id="dc4dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc4dd-116">Application</span></span> | <span data-ttu-id="dc4dd-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4dd-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc4dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc4dd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="dc4dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc4dd-119">Request headers</span></span>
| <span data-ttu-id="dc4dd-120">名称</span><span class="sxs-lookup"><span data-stu-id="dc4dd-120">Name</span></span>       | <span data-ttu-id="dc4dd-121">类型</span><span class="sxs-lookup"><span data-stu-id="dc4dd-121">Type</span></span> | <span data-ttu-id="dc4dd-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc4dd-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc4dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc4dd-123">Authorization</span></span>  | <span data-ttu-id="dc4dd-124">string</span><span class="sxs-lookup"><span data-stu-id="dc4dd-124">string</span></span>  | <span data-ttu-id="dc4dd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc4dd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc4dd-127">Request body</span></span>
<span data-ttu-id="dc4dd-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc4dd-129">参数</span><span class="sxs-lookup"><span data-stu-id="dc4dd-129">Parameter</span></span>    | <span data-ttu-id="dc4dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="dc4dd-130">Type</span></span>   |<span data-ttu-id="dc4dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc4dd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc4dd-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="dc4dd-132">groupIds</span></span>|<span data-ttu-id="dc4dd-133">String</span><span class="sxs-lookup"><span data-stu-id="dc4dd-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="dc4dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="dc4dd-134">Response</span></span>

<span data-ttu-id="dc4dd-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc4dd-136">示例</span><span class="sxs-lookup"><span data-stu-id="dc4dd-136">Example</span></span>
<span data-ttu-id="dc4dd-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc4dd-138">请求</span><span class="sxs-lookup"><span data-stu-id="dc4dd-138">Request</span></span>
<span data-ttu-id="dc4dd-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="dc4dd-140">响应</span><span class="sxs-lookup"><span data-stu-id="dc4dd-140">Response</span></span>
<span data-ttu-id="dc4dd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc4dd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
