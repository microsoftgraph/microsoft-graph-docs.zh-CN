---
title: 创建策略
description: 通过指定显示名称、 策略类型和策略说明创建新的策略对象。
ms.openlocfilehash: fca6201d7afa6a78f15da0d37fb611e4114783e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048611"
---
# <a name="create-policy"></a><span data-ttu-id="fe419-103">创建策略</span><span class="sxs-lookup"><span data-stu-id="fe419-103">Create Policy</span></span>

> <span data-ttu-id="fe419-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe419-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe419-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe419-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe419-106">通过指定显示名称、 策略类型和策略说明创建新的[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe419-106">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="fe419-107">注意： 将被存储之前验证策略的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fe419-107">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="fe419-108">如果它未通过验证，400 错误的请求将返回。</span><span class="sxs-lookup"><span data-stu-id="fe419-108">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe419-109">权限</span><span class="sxs-lookup"><span data-stu-id="fe419-109">Permissions</span></span>
<span data-ttu-id="fe419-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe419-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe419-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe419-112">Permission type</span></span>      | <span data-ttu-id="fe419-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe419-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe419-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe419-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fe419-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe419-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe419-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe419-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe419-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe419-117">Not supported.</span></span>    |
|<span data-ttu-id="fe419-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe419-118">Application</span></span> | <span data-ttu-id="fe419-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe419-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe419-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe419-120">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="fe419-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe419-121">Request headers</span></span>
| <span data-ttu-id="fe419-122">名称</span><span class="sxs-lookup"><span data-stu-id="fe419-122">Name</span></span>       | <span data-ttu-id="fe419-123">类型</span><span class="sxs-lookup"><span data-stu-id="fe419-123">Type</span></span> | <span data-ttu-id="fe419-124">说明</span><span class="sxs-lookup"><span data-stu-id="fe419-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe419-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe419-125">Authorization</span></span>  | <span data-ttu-id="fe419-126">string</span><span class="sxs-lookup"><span data-stu-id="fe419-126">string</span></span>  | <span data-ttu-id="fe419-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe419-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe419-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe419-129">Content-Type</span></span> | <span data-ttu-id="fe419-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fe419-130">application/json</span></span>  | <span data-ttu-id="fe419-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="fe419-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe419-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe419-133">Request body</span></span>
<span data-ttu-id="fe419-134">在请求正文中，提供了[策略](../resources/policy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe419-134">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="fe419-135">下表显示当您创建策略时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe419-135">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="fe419-136">参数</span><span class="sxs-lookup"><span data-stu-id="fe419-136">Parameter</span></span>    | <span data-ttu-id="fe419-137">类型</span><span class="sxs-lookup"><span data-stu-id="fe419-137">Type</span></span>   |<span data-ttu-id="fe419-138">说明</span><span class="sxs-lookup"><span data-stu-id="fe419-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe419-139">definition</span><span class="sxs-lookup"><span data-stu-id="fe419-139">definition</span></span>|<span data-ttu-id="fe419-140">字符串</span><span class="sxs-lookup"><span data-stu-id="fe419-140">String</span></span>|<span data-ttu-id="fe419-141">[策略](../resources/policy.md)对象的字符串版本。</span><span class="sxs-lookup"><span data-stu-id="fe419-141">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="fe419-142">displayName</span><span class="sxs-lookup"><span data-stu-id="fe419-142">displayName</span></span>|<span data-ttu-id="fe419-143">字符串</span><span class="sxs-lookup"><span data-stu-id="fe419-143">String</span></span>|<span data-ttu-id="fe419-144">自定义策略名称。</span><span class="sxs-lookup"><span data-stu-id="fe419-144">A custom name for the policy.</span></span>|
|<span data-ttu-id="fe419-145">type</span><span class="sxs-lookup"><span data-stu-id="fe419-145">type</span></span>|<span data-ttu-id="fe419-146">字符串</span><span class="sxs-lookup"><span data-stu-id="fe419-146">String</span></span>|<span data-ttu-id="fe419-147">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="fe419-147">Specifies the type of policy.</span></span> <span data-ttu-id="fe419-148">当前值必须为"TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="fe419-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="fe419-149">响应</span><span class="sxs-lookup"><span data-stu-id="fe419-149">Response</span></span>

<span data-ttu-id="fe419-150">如果成功，此方法返回`201 Created`响应正文中的响应代码和[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe419-150">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="fe419-151">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="fe419-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="fe419-152">示例</span><span class="sxs-lookup"><span data-stu-id="fe419-152">Example</span></span>
<span data-ttu-id="fe419-153">下面的示例创建新的令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="fe419-153">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="fe419-154">请注意字符串定义参数具有转义双引号括起来。</span><span class="sxs-lookup"><span data-stu-id="fe419-154">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="fe419-155">请求</span><span class="sxs-lookup"><span data-stu-id="fe419-155">Request</span></span>
<span data-ttu-id="fe419-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe419-156">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="fe419-157">响应</span><span class="sxs-lookup"><span data-stu-id="fe419-157">Response</span></span>
<span data-ttu-id="fe419-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe419-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
