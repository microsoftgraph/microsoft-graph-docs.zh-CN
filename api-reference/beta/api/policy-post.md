---
title: 创建策略
description: 通过指定显示名称、策略类型和策略说明来创建新的 policy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2e13ef2bdcf424d68d94d97412487708022386cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455499"
---
# <a name="create-policy"></a><span data-ttu-id="c6dd6-103">创建策略</span><span class="sxs-lookup"><span data-stu-id="c6dd6-103">Create Policy</span></span>

<span data-ttu-id="c6dd6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c6dd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6dd6-105">通过指定显示名称、策略类型和策略说明来创建新的[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-105">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="c6dd6-106">注意：将在存储策略详细信息之前对其进行验证。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-106">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="c6dd6-107">如果它未通过验证，将返回400个错误的请求。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-107">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6dd6-108">权限</span><span class="sxs-lookup"><span data-stu-id="c6dd6-108">Permissions</span></span>
<span data-ttu-id="c6dd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6dd6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6dd6-111">Permission type</span></span>      | <span data-ttu-id="c6dd6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6dd6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6dd6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6dd6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6dd6-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6dd6-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6dd6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6dd6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6dd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-116">Not supported.</span></span>    |
|<span data-ttu-id="c6dd6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6dd6-117">Application</span></span> | <span data-ttu-id="c6dd6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6dd6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6dd6-119">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="c6dd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6dd6-120">Request headers</span></span>
| <span data-ttu-id="c6dd6-121">名称</span><span class="sxs-lookup"><span data-stu-id="c6dd6-121">Name</span></span>       | <span data-ttu-id="c6dd6-122">类型</span><span class="sxs-lookup"><span data-stu-id="c6dd6-122">Type</span></span> | <span data-ttu-id="c6dd6-123">说明</span><span class="sxs-lookup"><span data-stu-id="c6dd6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6dd6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6dd6-124">Authorization</span></span>  | <span data-ttu-id="c6dd6-125">string</span><span class="sxs-lookup"><span data-stu-id="c6dd6-125">string</span></span>  | <span data-ttu-id="c6dd6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6dd6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6dd6-128">Content-Type</span></span> | <span data-ttu-id="c6dd6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c6dd6-129">application/json</span></span>  | <span data-ttu-id="c6dd6-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6dd6-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6dd6-132">Request body</span></span>
<span data-ttu-id="c6dd6-133">在请求正文中，提供[policy](../resources/policy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-133">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="c6dd6-134">下表显示创建策略时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-134">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="c6dd6-135">参数</span><span class="sxs-lookup"><span data-stu-id="c6dd6-135">Parameter</span></span>    | <span data-ttu-id="c6dd6-136">类型</span><span class="sxs-lookup"><span data-stu-id="c6dd6-136">Type</span></span>   |<span data-ttu-id="c6dd6-137">说明</span><span class="sxs-lookup"><span data-stu-id="c6dd6-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6dd6-138">定义</span><span class="sxs-lookup"><span data-stu-id="c6dd6-138">definition</span></span>|<span data-ttu-id="c6dd6-139">String</span><span class="sxs-lookup"><span data-stu-id="c6dd6-139">String</span></span>|<span data-ttu-id="c6dd6-140">[Policy](../resources/policy.md)对象的字符串版本。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-140">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="c6dd6-141">displayName</span><span class="sxs-lookup"><span data-stu-id="c6dd6-141">displayName</span></span>|<span data-ttu-id="c6dd6-142">String</span><span class="sxs-lookup"><span data-stu-id="c6dd6-142">String</span></span>|<span data-ttu-id="c6dd6-143">策略的自定义名称。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-143">A custom name for the policy.</span></span>|
|<span data-ttu-id="c6dd6-144">type</span><span class="sxs-lookup"><span data-stu-id="c6dd6-144">type</span></span>|<span data-ttu-id="c6dd6-145">String</span><span class="sxs-lookup"><span data-stu-id="c6dd6-145">String</span></span>|<span data-ttu-id="c6dd6-146">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-146">Specifies the type of policy.</span></span> <span data-ttu-id="c6dd6-147">当前必须是 "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="c6dd6-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="c6dd6-148">响应</span><span class="sxs-lookup"><span data-stu-id="c6dd6-148">Response</span></span>

<span data-ttu-id="c6dd6-149">如果成功，此方法在`201 Created`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-149">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="c6dd6-150">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="c6dd6-151">示例</span><span class="sxs-lookup"><span data-stu-id="c6dd6-151">Example</span></span>
<span data-ttu-id="c6dd6-152">下面的示例创建一个新的令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-152">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="c6dd6-153">请注意，字符串定义参数中包含转义双引号。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-153">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="c6dd6-154">请求</span><span class="sxs-lookup"><span data-stu-id="c6dd6-154">Request</span></span>
<span data-ttu-id="c6dd6-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-155">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="c6dd6-156">响应</span><span class="sxs-lookup"><span data-stu-id="c6dd6-156">Response</span></span>
<span data-ttu-id="c6dd6-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6dd6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
