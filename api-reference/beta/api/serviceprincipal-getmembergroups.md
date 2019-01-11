---
title: 'servicePrincipal: getMemberGroups'
description: 获取组的成员的此服务主体的列表。  检查是传递的。
localization_priority: Normal
ms.openlocfilehash: 6d552b410da23e5675257340ddc61cb4abbcd5e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817645"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="24fa3-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="24fa3-104">servicePrincipal: getMemberGroups</span></span>

> <span data-ttu-id="24fa3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="24fa3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24fa3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24fa3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24fa3-107">获取组的成员的此服务主体的列表。</span><span class="sxs-lookup"><span data-stu-id="24fa3-107">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="24fa3-108">检查是传递的。</span><span class="sxs-lookup"><span data-stu-id="24fa3-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="24fa3-109">权限</span><span class="sxs-lookup"><span data-stu-id="24fa3-109">Permissions</span></span>
<span data-ttu-id="24fa3-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24fa3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="24fa3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="24fa3-112">Permission type</span></span>      | <span data-ttu-id="24fa3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24fa3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24fa3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24fa3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="24fa3-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24fa3-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24fa3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24fa3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24fa3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="24fa3-117">Not supported.</span></span>    |
|<span data-ttu-id="24fa3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="24fa3-118">Application</span></span> | <span data-ttu-id="24fa3-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fa3-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24fa3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24fa3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="24fa3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="24fa3-121">Request headers</span></span>
| <span data-ttu-id="24fa3-122">名称</span><span class="sxs-lookup"><span data-stu-id="24fa3-122">Name</span></span>       | <span data-ttu-id="24fa3-123">类型</span><span class="sxs-lookup"><span data-stu-id="24fa3-123">Type</span></span> | <span data-ttu-id="24fa3-124">说明</span><span class="sxs-lookup"><span data-stu-id="24fa3-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24fa3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="24fa3-125">Authorization</span></span>  | <span data-ttu-id="24fa3-126">string</span><span class="sxs-lookup"><span data-stu-id="24fa3-126">string</span></span>  | <span data-ttu-id="24fa3-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24fa3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24fa3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="24fa3-129">Request body</span></span>
<span data-ttu-id="24fa3-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="24fa3-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24fa3-131">参数</span><span class="sxs-lookup"><span data-stu-id="24fa3-131">Parameter</span></span>    | <span data-ttu-id="24fa3-132">类型</span><span class="sxs-lookup"><span data-stu-id="24fa3-132">Type</span></span>   |<span data-ttu-id="24fa3-133">说明</span><span class="sxs-lookup"><span data-stu-id="24fa3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24fa3-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="24fa3-134">securityEnabledOnly</span></span>|<span data-ttu-id="24fa3-135">布尔</span><span class="sxs-lookup"><span data-stu-id="24fa3-135">Boolean</span></span>|<span data-ttu-id="24fa3-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="24fa3-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="24fa3-138">响应</span><span class="sxs-lookup"><span data-stu-id="24fa3-138">Response</span></span>

<span data-ttu-id="24fa3-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="24fa3-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fa3-140">示例</span><span class="sxs-lookup"><span data-stu-id="24fa3-140">Example</span></span>
<span data-ttu-id="24fa3-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="24fa3-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24fa3-142">请求</span><span class="sxs-lookup"><span data-stu-id="24fa3-142">Request</span></span>
<span data-ttu-id="24fa3-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24fa3-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="24fa3-144">响应</span><span class="sxs-lookup"><span data-stu-id="24fa3-144">Response</span></span>
<span data-ttu-id="24fa3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24fa3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
