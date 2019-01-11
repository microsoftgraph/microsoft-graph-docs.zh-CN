---
title: 更新策略
description: 更新以前存在策略中的属性。
localization_priority: Normal
ms.openlocfilehash: 2992f2f76c0e8b213ad8aabca1bfd0fe59883989
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857153"
---
# <a name="update-policy"></a><span data-ttu-id="98a80-103">更新策略</span><span class="sxs-lookup"><span data-stu-id="98a80-103">Update Policy</span></span>

> <span data-ttu-id="98a80-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="98a80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98a80-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="98a80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98a80-106">更新以前存在[策略](../resources/policy.md)中的属性。</span><span class="sxs-lookup"><span data-stu-id="98a80-106">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98a80-107">权限</span><span class="sxs-lookup"><span data-stu-id="98a80-107">Permissions</span></span>
<span data-ttu-id="98a80-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98a80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98a80-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98a80-110">Permission type</span></span>      | <span data-ttu-id="98a80-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98a80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98a80-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98a80-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98a80-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="98a80-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98a80-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98a80-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98a80-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98a80-115">Not supported.</span></span>    |
|<span data-ttu-id="98a80-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98a80-116">Application</span></span> | <span data-ttu-id="98a80-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="98a80-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98a80-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98a80-118">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="98a80-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98a80-119">Request headers</span></span>
| <span data-ttu-id="98a80-120">名称</span><span class="sxs-lookup"><span data-stu-id="98a80-120">Name</span></span>       | <span data-ttu-id="98a80-121">类型</span><span class="sxs-lookup"><span data-stu-id="98a80-121">Type</span></span> | <span data-ttu-id="98a80-122">说明</span><span class="sxs-lookup"><span data-stu-id="98a80-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98a80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98a80-123">Authorization</span></span>  | <span data-ttu-id="98a80-124">string</span><span class="sxs-lookup"><span data-stu-id="98a80-124">string</span></span>  | <span data-ttu-id="98a80-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98a80-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98a80-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98a80-127">Content-Type</span></span> | <span data-ttu-id="98a80-128">application/json</span><span class="sxs-lookup"><span data-stu-id="98a80-128">application/json</span></span>  | <span data-ttu-id="98a80-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="98a80-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98a80-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="98a80-131">Request body</span></span>
<span data-ttu-id="98a80-132">在请求正文中，将一个 JSON 对象，提供需要更新的参数。</span><span class="sxs-lookup"><span data-stu-id="98a80-132">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="98a80-133">下表显示可能的参数。</span><span class="sxs-lookup"><span data-stu-id="98a80-133">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="98a80-134">参数</span><span class="sxs-lookup"><span data-stu-id="98a80-134">Parameter</span></span>    | <span data-ttu-id="98a80-135">类型</span><span class="sxs-lookup"><span data-stu-id="98a80-135">Type</span></span>   |<span data-ttu-id="98a80-136">Description</span><span class="sxs-lookup"><span data-stu-id="98a80-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98a80-137">definition</span><span class="sxs-lookup"><span data-stu-id="98a80-137">definition</span></span>|<span data-ttu-id="98a80-138">字符串</span><span class="sxs-lookup"><span data-stu-id="98a80-138">String</span></span>|<span data-ttu-id="98a80-139">Stringified 的[策略](../resources/policy.md)对象的版本。</span><span class="sxs-lookup"><span data-stu-id="98a80-139">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="98a80-140">displayName</span><span class="sxs-lookup"><span data-stu-id="98a80-140">displayName</span></span>|<span data-ttu-id="98a80-141">字符串</span><span class="sxs-lookup"><span data-stu-id="98a80-141">String</span></span>|<span data-ttu-id="98a80-142">自定义策略名称。</span><span class="sxs-lookup"><span data-stu-id="98a80-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="98a80-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="98a80-143">isOrganizationDefault</span></span>|<span data-ttu-id="98a80-144">布尔</span><span class="sxs-lookup"><span data-stu-id="98a80-144">Boolean</span></span>|<span data-ttu-id="98a80-145">指定默认情况下是否应用此策略。</span><span class="sxs-lookup"><span data-stu-id="98a80-145">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="98a80-146">type</span><span class="sxs-lookup"><span data-stu-id="98a80-146">type</span></span>|<span data-ttu-id="98a80-147">字符串</span><span class="sxs-lookup"><span data-stu-id="98a80-147">String</span></span>|<span data-ttu-id="98a80-148">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="98a80-148">Specifies the type of policy.</span></span> <span data-ttu-id="98a80-149">当前值必须为"TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="98a80-149">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="98a80-150">响应</span><span class="sxs-lookup"><span data-stu-id="98a80-150">Response</span></span>

<span data-ttu-id="98a80-151">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="98a80-151">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="98a80-152">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="98a80-152">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="98a80-153">示例</span><span class="sxs-lookup"><span data-stu-id="98a80-153">Example</span></span>
<span data-ttu-id="98a80-154">以下示例更新的令牌生存期策略定义，并将其设置为默认组织。</span><span class="sxs-lookup"><span data-stu-id="98a80-154">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="98a80-155">请求</span><span class="sxs-lookup"><span data-stu-id="98a80-155">Request</span></span>
<span data-ttu-id="98a80-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98a80-156">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="98a80-157">响应</span><span class="sxs-lookup"><span data-stu-id="98a80-157">Response</span></span>
<span data-ttu-id="98a80-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98a80-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
