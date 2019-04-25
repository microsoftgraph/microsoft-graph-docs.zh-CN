---
title: 创建策略
description: 通过指定显示名称、策略类型和策略说明来创建新的 policy 对象。
localization_priority: Normal
ms.openlocfilehash: 30a311b45f9705a07b62541a4f3a110daade09fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546841"
---
# <a name="create-policy"></a><span data-ttu-id="8c239-103">创建策略</span><span class="sxs-lookup"><span data-stu-id="8c239-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c239-104">通过指定显示名称、策略类型和策略说明来创建新的[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c239-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="8c239-105">注意: 将在存储策略详细信息之前对其进行验证。</span><span class="sxs-lookup"><span data-stu-id="8c239-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="8c239-106">如果它未通过验证, 将返回400个错误的请求。</span><span class="sxs-lookup"><span data-stu-id="8c239-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c239-107">权限</span><span class="sxs-lookup"><span data-stu-id="8c239-107">Permissions</span></span>
<span data-ttu-id="8c239-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c239-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c239-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c239-110">Permission type</span></span>      | <span data-ttu-id="8c239-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c239-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c239-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c239-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8c239-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c239-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c239-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c239-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c239-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c239-115">Not supported.</span></span>    |
|<span data-ttu-id="8c239-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c239-116">Application</span></span> | <span data-ttu-id="8c239-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c239-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c239-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c239-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="8c239-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c239-119">Request headers</span></span>
| <span data-ttu-id="8c239-120">名称</span><span class="sxs-lookup"><span data-stu-id="8c239-120">Name</span></span>       | <span data-ttu-id="8c239-121">类型</span><span class="sxs-lookup"><span data-stu-id="8c239-121">Type</span></span> | <span data-ttu-id="8c239-122">说明</span><span class="sxs-lookup"><span data-stu-id="8c239-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c239-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c239-123">Authorization</span></span>  | <span data-ttu-id="8c239-124">string</span><span class="sxs-lookup"><span data-stu-id="8c239-124">string</span></span>  | <span data-ttu-id="8c239-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c239-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c239-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c239-127">Content-Type</span></span> | <span data-ttu-id="8c239-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8c239-128">application/json</span></span>  | <span data-ttu-id="8c239-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="8c239-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c239-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c239-131">Request body</span></span>
<span data-ttu-id="8c239-132">在请求正文中, 提供[policy](../resources/policy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c239-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="8c239-133">下表显示创建策略时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c239-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="8c239-134">参数</span><span class="sxs-lookup"><span data-stu-id="8c239-134">Parameter</span></span>    | <span data-ttu-id="8c239-135">类型</span><span class="sxs-lookup"><span data-stu-id="8c239-135">Type</span></span>   |<span data-ttu-id="8c239-136">说明</span><span class="sxs-lookup"><span data-stu-id="8c239-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c239-137">定义</span><span class="sxs-lookup"><span data-stu-id="8c239-137">definition</span></span>|<span data-ttu-id="8c239-138">String</span><span class="sxs-lookup"><span data-stu-id="8c239-138">String</span></span>|<span data-ttu-id="8c239-139">[policy](../resources/policy.md)对象的字符串版本。</span><span class="sxs-lookup"><span data-stu-id="8c239-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="8c239-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8c239-140">displayName</span></span>|<span data-ttu-id="8c239-141">String</span><span class="sxs-lookup"><span data-stu-id="8c239-141">String</span></span>|<span data-ttu-id="8c239-142">策略的自定义名称。</span><span class="sxs-lookup"><span data-stu-id="8c239-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="8c239-143">类型</span><span class="sxs-lookup"><span data-stu-id="8c239-143">type</span></span>|<span data-ttu-id="8c239-144">String</span><span class="sxs-lookup"><span data-stu-id="8c239-144">String</span></span>|<span data-ttu-id="8c239-145">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="8c239-145">Specifies the type of policy.</span></span> <span data-ttu-id="8c239-146">当前必须是 "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="8c239-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="8c239-147">响应</span><span class="sxs-lookup"><span data-stu-id="8c239-147">Response</span></span>

<span data-ttu-id="8c239-148">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c239-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="8c239-149">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c239-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="8c239-150">示例</span><span class="sxs-lookup"><span data-stu-id="8c239-150">Example</span></span>
<span data-ttu-id="8c239-151">下面的示例创建一个新的令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="8c239-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="8c239-152">请注意, 字符串定义参数中包含转义双引号。</span><span class="sxs-lookup"><span data-stu-id="8c239-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="8c239-153">请求</span><span class="sxs-lookup"><span data-stu-id="8c239-153">Request</span></span>
<span data-ttu-id="8c239-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c239-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="8c239-155">响应</span><span class="sxs-lookup"><span data-stu-id="8c239-155">Response</span></span>
<span data-ttu-id="8c239-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c239-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/policy-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
