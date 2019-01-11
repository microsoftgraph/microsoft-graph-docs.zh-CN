---
title: 'servicePrincipal: getMemberObjects'
description: 获取组和目录角色的成员的此服务主体的列表。  可传递此检查。
localization_priority: Normal
ms.openlocfilehash: 46c23e18d2484b3dff38ed8791f203e823c4cc9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842117"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="1fc5b-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="1fc5b-104">servicePrincipal: getMemberObjects</span></span>

> <span data-ttu-id="1fc5b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fc5b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fc5b-107">获取组和目录角色的成员的此服务主体的列表。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-107">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="1fc5b-108">可传递此检查。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-108">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fc5b-109">权限</span><span class="sxs-lookup"><span data-stu-id="1fc5b-109">Permissions</span></span>
<span data-ttu-id="1fc5b-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc5b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fc5b-112">Permission type</span></span>      | <span data-ttu-id="1fc5b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fc5b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1fc5b-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fc5b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fc5b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fc5b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-117">Not supported.</span></span>    |
|<span data-ttu-id="1fc5b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fc5b-118">Application</span></span> | <span data-ttu-id="1fc5b-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc5b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fc5b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fc5b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="1fc5b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fc5b-121">Request headers</span></span>
| <span data-ttu-id="1fc5b-122">名称</span><span class="sxs-lookup"><span data-stu-id="1fc5b-122">Name</span></span>       | <span data-ttu-id="1fc5b-123">类型</span><span class="sxs-lookup"><span data-stu-id="1fc5b-123">Type</span></span> | <span data-ttu-id="1fc5b-124">说明</span><span class="sxs-lookup"><span data-stu-id="1fc5b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fc5b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fc5b-125">Authorization</span></span>  | <span data-ttu-id="1fc5b-126">string</span><span class="sxs-lookup"><span data-stu-id="1fc5b-126">string</span></span>  | <span data-ttu-id="1fc5b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fc5b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fc5b-129">Request body</span></span>
<span data-ttu-id="1fc5b-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1fc5b-131">参数</span><span class="sxs-lookup"><span data-stu-id="1fc5b-131">Parameter</span></span>    | <span data-ttu-id="1fc5b-132">类型</span><span class="sxs-lookup"><span data-stu-id="1fc5b-132">Type</span></span>   |<span data-ttu-id="1fc5b-133">说明</span><span class="sxs-lookup"><span data-stu-id="1fc5b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fc5b-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1fc5b-134">securityEnabledOnly</span></span>|<span data-ttu-id="1fc5b-135">布尔</span><span class="sxs-lookup"><span data-stu-id="1fc5b-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="1fc5b-136">响应</span><span class="sxs-lookup"><span data-stu-id="1fc5b-136">Response</span></span>

<span data-ttu-id="1fc5b-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fc5b-138">示例</span><span class="sxs-lookup"><span data-stu-id="1fc5b-138">Example</span></span>
<span data-ttu-id="1fc5b-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1fc5b-140">请求</span><span class="sxs-lookup"><span data-stu-id="1fc5b-140">Request</span></span>
<span data-ttu-id="1fc5b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="1fc5b-142">响应</span><span class="sxs-lookup"><span data-stu-id="1fc5b-142">Response</span></span>
<span data-ttu-id="1fc5b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
