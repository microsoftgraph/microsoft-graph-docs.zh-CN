---
title: servicePrincipal： getMemberGroups
description: 获取此服务主体所属的组列表。  检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e22f89f0ee909ab28fe65d8c67837d125b701280
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291256"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="1b134-104">servicePrincipal： getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1b134-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="1b134-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b134-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b134-106">获取此[servicePrincipal](../resources/serviceprincipal.md)所属组的列表。</span><span class="sxs-lookup"><span data-stu-id="1b134-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="1b134-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="1b134-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b134-108">权限</span><span class="sxs-lookup"><span data-stu-id="1b134-108">Permissions</span></span>
<span data-ttu-id="1b134-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b134-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1b134-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b134-111">Permission type</span></span>      | <span data-ttu-id="1b134-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b134-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b134-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b134-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1b134-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b134-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b134-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b134-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b134-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b134-116">Not supported.</span></span>    |
|<span data-ttu-id="1b134-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b134-117">Application</span></span> | <span data-ttu-id="1b134-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b134-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b134-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b134-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="1b134-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b134-120">Request headers</span></span>
| <span data-ttu-id="1b134-121">名称</span><span class="sxs-lookup"><span data-stu-id="1b134-121">Name</span></span>       | <span data-ttu-id="1b134-122">说明</span><span class="sxs-lookup"><span data-stu-id="1b134-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="1b134-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b134-123">Authorization</span></span> | <span data-ttu-id="1b134-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b134-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b134-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b134-126">Content-type</span></span> | <span data-ttu-id="1b134-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1b134-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b134-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b134-129">Request body</span></span>
<span data-ttu-id="1b134-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1b134-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1b134-131">参数</span><span class="sxs-lookup"><span data-stu-id="1b134-131">Parameter</span></span>    | <span data-ttu-id="1b134-132">类型</span><span class="sxs-lookup"><span data-stu-id="1b134-132">Type</span></span>   |<span data-ttu-id="1b134-133">说明</span><span class="sxs-lookup"><span data-stu-id="1b134-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b134-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1b134-134">securityEnabledOnly</span></span>|<span data-ttu-id="1b134-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b134-135">Boolean</span></span>|<span data-ttu-id="1b134-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="1b134-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="1b134-138">响应</span><span class="sxs-lookup"><span data-stu-id="1b134-138">Response</span></span>

<span data-ttu-id="1b134-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="1b134-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b134-140">示例</span><span class="sxs-lookup"><span data-stu-id="1b134-140">Examples</span></span>
<span data-ttu-id="1b134-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1b134-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="1b134-142">请求</span><span class="sxs-lookup"><span data-stu-id="1b134-142">Request</span></span>
<span data-ttu-id="1b134-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b134-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b134-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b134-144">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="1b134-145">响应</span><span class="sxs-lookup"><span data-stu-id="1b134-145">Response</span></span>
<span data-ttu-id="1b134-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1b134-146">Here is an example of the response.</span></span> 
><span data-ttu-id="1b134-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b134-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
