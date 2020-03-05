---
title: 更新策略
description: 更新预先存在的策略中的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 81c9d429ba3a74d854a9d091f6e40af7993916f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455490"
---
# <a name="update-policy"></a><span data-ttu-id="7aeb4-103">更新策略</span><span class="sxs-lookup"><span data-stu-id="7aeb4-103">Update Policy</span></span>

<span data-ttu-id="7aeb4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7aeb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aeb4-105">更新预先存在的[策略](../resources/policy.md)中的属性。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-105">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7aeb4-106">权限</span><span class="sxs-lookup"><span data-stu-id="7aeb4-106">Permissions</span></span>
<span data-ttu-id="7aeb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aeb4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aeb4-109">Permission type</span></span>      | <span data-ttu-id="7aeb4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aeb4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aeb4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aeb4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7aeb4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7aeb4-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7aeb4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aeb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aeb4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-114">Not supported.</span></span>    |
|<span data-ttu-id="7aeb4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aeb4-115">Application</span></span> | <span data-ttu-id="7aeb4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aeb4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aeb4-117">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7aeb4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aeb4-118">Request headers</span></span>
| <span data-ttu-id="7aeb4-119">名称</span><span class="sxs-lookup"><span data-stu-id="7aeb4-119">Name</span></span>       | <span data-ttu-id="7aeb4-120">类型</span><span class="sxs-lookup"><span data-stu-id="7aeb4-120">Type</span></span> | <span data-ttu-id="7aeb4-121">说明</span><span class="sxs-lookup"><span data-stu-id="7aeb4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7aeb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aeb4-122">Authorization</span></span>  | <span data-ttu-id="7aeb4-123">string</span><span class="sxs-lookup"><span data-stu-id="7aeb4-123">string</span></span>  | <span data-ttu-id="7aeb4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7aeb4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aeb4-126">Content-Type</span></span> | <span data-ttu-id="7aeb4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7aeb4-127">application/json</span></span>  | <span data-ttu-id="7aeb4-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aeb4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aeb4-130">Request body</span></span>
<span data-ttu-id="7aeb4-131">在请求正文中，提供具有需要更新的参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-131">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="7aeb4-132">下表显示了可能的参数。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-132">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="7aeb4-133">参数</span><span class="sxs-lookup"><span data-stu-id="7aeb4-133">Parameter</span></span>    | <span data-ttu-id="7aeb4-134">类型</span><span class="sxs-lookup"><span data-stu-id="7aeb4-134">Type</span></span>   |<span data-ttu-id="7aeb4-135">说明</span><span class="sxs-lookup"><span data-stu-id="7aeb4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aeb4-136">定义</span><span class="sxs-lookup"><span data-stu-id="7aeb4-136">definition</span></span>|<span data-ttu-id="7aeb4-137">String</span><span class="sxs-lookup"><span data-stu-id="7aeb4-137">String</span></span>|<span data-ttu-id="7aeb4-138">[Policy](../resources/policy.md)对象的字符串化版本。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-138">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="7aeb4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7aeb4-139">displayName</span></span>|<span data-ttu-id="7aeb4-140">String</span><span class="sxs-lookup"><span data-stu-id="7aeb4-140">String</span></span>|<span data-ttu-id="7aeb4-141">策略的自定义名称。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-141">A custom name for the policy.</span></span>|
|<span data-ttu-id="7aeb4-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="7aeb4-142">isOrganizationDefault</span></span>|<span data-ttu-id="7aeb4-143">布尔</span><span class="sxs-lookup"><span data-stu-id="7aeb4-143">Boolean</span></span>|<span data-ttu-id="7aeb4-144">指定默认情况下是否应用此策略。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-144">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="7aeb4-145">type</span><span class="sxs-lookup"><span data-stu-id="7aeb4-145">type</span></span>|<span data-ttu-id="7aeb4-146">String</span><span class="sxs-lookup"><span data-stu-id="7aeb4-146">String</span></span>|<span data-ttu-id="7aeb4-147">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-147">Specifies the type of policy.</span></span> <span data-ttu-id="7aeb4-148">当前必须是 "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="7aeb4-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="7aeb4-149">响应</span><span class="sxs-lookup"><span data-stu-id="7aeb4-149">Response</span></span>

<span data-ttu-id="7aeb4-150">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-150">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7aeb4-151">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7aeb4-152">示例</span><span class="sxs-lookup"><span data-stu-id="7aeb4-152">Example</span></span>
<span data-ttu-id="7aeb4-153">下面的示例更新令牌生存期策略的定义，并将其设置为组织的默认值。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-153">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7aeb4-154">请求</span><span class="sxs-lookup"><span data-stu-id="7aeb4-154">Request</span></span>
<span data-ttu-id="7aeb4-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-155">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="7aeb4-156">响应</span><span class="sxs-lookup"><span data-stu-id="7aeb4-156">Response</span></span>
<span data-ttu-id="7aeb4-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7aeb4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
