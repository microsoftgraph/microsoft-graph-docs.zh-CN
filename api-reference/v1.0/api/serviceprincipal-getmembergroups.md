---
title: servicePrincipal： getMemberGroups
description: 获取此服务主体所属的组列表。  检查是可传递的。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 5859d7834a54426dc29930b67bf7ed44ee43a431
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290368"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="5e183-104">servicePrincipal： getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5e183-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="5e183-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e183-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e183-106">获取此[servicePrincipal](../resources/serviceprincipal.md)所属组的列表。</span><span class="sxs-lookup"><span data-stu-id="5e183-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="5e183-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="5e183-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e183-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="5e183-108">Permissions</span></span>
<span data-ttu-id="5e183-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e183-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e183-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e183-111">Permission type</span></span>      | <span data-ttu-id="5e183-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e183-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e183-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e183-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5e183-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e183-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e183-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e183-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e183-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e183-116">Not supported.</span></span>    |
|<span data-ttu-id="5e183-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e183-117">Application</span></span> | <span data-ttu-id="5e183-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e183-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e183-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e183-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="5e183-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e183-120">Request headers</span></span>
| <span data-ttu-id="5e183-121">名称</span><span class="sxs-lookup"><span data-stu-id="5e183-121">Name</span></span>       | <span data-ttu-id="5e183-122">说明</span><span class="sxs-lookup"><span data-stu-id="5e183-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5e183-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e183-123">Authorization</span></span> | <span data-ttu-id="5e183-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e183-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e183-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="5e183-126">Content-type</span></span> | <span data-ttu-id="5e183-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5e183-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e183-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e183-129">Request body</span></span>
<span data-ttu-id="5e183-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5e183-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5e183-131">参数</span><span class="sxs-lookup"><span data-stu-id="5e183-131">Parameter</span></span>    | <span data-ttu-id="5e183-132">类型</span><span class="sxs-lookup"><span data-stu-id="5e183-132">Type</span></span>   |<span data-ttu-id="5e183-133">Description</span><span class="sxs-lookup"><span data-stu-id="5e183-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e183-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5e183-134">securityEnabledOnly</span></span>|<span data-ttu-id="5e183-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e183-135">Boolean</span></span>|<span data-ttu-id="5e183-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="5e183-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="5e183-138">响应</span><span class="sxs-lookup"><span data-stu-id="5e183-138">Response</span></span>

<span data-ttu-id="5e183-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="5e183-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e183-140">示例</span><span class="sxs-lookup"><span data-stu-id="5e183-140">Example</span></span>
<span data-ttu-id="5e183-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5e183-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="5e183-142">请求</span><span class="sxs-lookup"><span data-stu-id="5e183-142">Request</span></span>
<span data-ttu-id="5e183-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e183-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

### <a name="response"></a><span data-ttu-id="5e183-144">响应</span><span class="sxs-lookup"><span data-stu-id="5e183-144">Response</span></span>
<span data-ttu-id="5e183-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e183-145">Here is an example of the response.</span></span> 
><span data-ttu-id="5e183-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e183-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
