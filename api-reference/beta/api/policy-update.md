---
title: 更新策略
description: 更新预先存在的策略中的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: 1194d746d0313da0835fc9939bc12671c372684d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408252"
---
# <a name="update-policy"></a><span data-ttu-id="3ee9c-103">更新策略</span><span class="sxs-lookup"><span data-stu-id="3ee9c-103">Update Policy</span></span>

<span data-ttu-id="3ee9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ee9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ee9c-105">更新预先存在的[策略](../resources/policy.md)中的属性。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-105">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ee9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ee9c-106">Permissions</span></span>
<span data-ttu-id="3ee9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ee9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ee9c-109">Permission type</span></span>      | <span data-ttu-id="3ee9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ee9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ee9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ee9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ee9c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ee9c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ee9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ee9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ee9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-114">Not supported.</span></span>    |
|<span data-ttu-id="3ee9c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ee9c-115">Application</span></span> | <span data-ttu-id="3ee9c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ee9c-117">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3ee9c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ee9c-118">Request headers</span></span>
| <span data-ttu-id="3ee9c-119">名称</span><span class="sxs-lookup"><span data-stu-id="3ee9c-119">Name</span></span>       | <span data-ttu-id="3ee9c-120">类型</span><span class="sxs-lookup"><span data-stu-id="3ee9c-120">Type</span></span> | <span data-ttu-id="3ee9c-121">说明</span><span class="sxs-lookup"><span data-stu-id="3ee9c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ee9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ee9c-122">Authorization</span></span>  | <span data-ttu-id="3ee9c-123">string</span><span class="sxs-lookup"><span data-stu-id="3ee9c-123">string</span></span>  | <span data-ttu-id="3ee9c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ee9c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ee9c-126">Content-Type</span></span> | <span data-ttu-id="3ee9c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3ee9c-127">application/json</span></span>  | <span data-ttu-id="3ee9c-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ee9c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ee9c-130">Request body</span></span>
<span data-ttu-id="3ee9c-131">在请求正文中，提供具有需要更新的参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-131">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="3ee9c-132">下表显示了可能的参数。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-132">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="3ee9c-133">参数</span><span class="sxs-lookup"><span data-stu-id="3ee9c-133">Parameter</span></span>    | <span data-ttu-id="3ee9c-134">类型</span><span class="sxs-lookup"><span data-stu-id="3ee9c-134">Type</span></span>   |<span data-ttu-id="3ee9c-135">说明</span><span class="sxs-lookup"><span data-stu-id="3ee9c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ee9c-136">定义</span><span class="sxs-lookup"><span data-stu-id="3ee9c-136">definition</span></span>|<span data-ttu-id="3ee9c-137">String</span><span class="sxs-lookup"><span data-stu-id="3ee9c-137">String</span></span>|<span data-ttu-id="3ee9c-138">[Policy](../resources/policy.md)对象的字符串化版本。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-138">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="3ee9c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3ee9c-139">displayName</span></span>|<span data-ttu-id="3ee9c-140">String</span><span class="sxs-lookup"><span data-stu-id="3ee9c-140">String</span></span>|<span data-ttu-id="3ee9c-141">策略的自定义名称。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-141">A custom name for the policy.</span></span>|
|<span data-ttu-id="3ee9c-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="3ee9c-142">isOrganizationDefault</span></span>|<span data-ttu-id="3ee9c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ee9c-143">Boolean</span></span>|<span data-ttu-id="3ee9c-144">指定默认情况下是否应用此策略。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-144">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="3ee9c-145">type</span><span class="sxs-lookup"><span data-stu-id="3ee9c-145">type</span></span>|<span data-ttu-id="3ee9c-146">String</span><span class="sxs-lookup"><span data-stu-id="3ee9c-146">String</span></span>|<span data-ttu-id="3ee9c-147">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-147">Specifies the type of policy.</span></span> <span data-ttu-id="3ee9c-148">当前必须是 "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="3ee9c-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="3ee9c-149">响应</span><span class="sxs-lookup"><span data-stu-id="3ee9c-149">Response</span></span>

<span data-ttu-id="3ee9c-150">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-150">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="3ee9c-151">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="3ee9c-152">示例</span><span class="sxs-lookup"><span data-stu-id="3ee9c-152">Example</span></span>
<span data-ttu-id="3ee9c-153">下面的示例更新令牌生存期策略的定义，并将其设置为组织的默认值。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-153">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="3ee9c-154">请求</span><span class="sxs-lookup"><span data-stu-id="3ee9c-154">Request</span></span>
<span data-ttu-id="3ee9c-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-155">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="3ee9c-156">响应</span><span class="sxs-lookup"><span data-stu-id="3ee9c-156">Response</span></span>
<span data-ttu-id="3ee9c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
