---
title: 更新策略
description: 更新预先存在的策略中的属性。
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538736"
---
# <a name="update-policy"></a><span data-ttu-id="b8b15-103">更新策略</span><span class="sxs-lookup"><span data-stu-id="b8b15-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8b15-104">更新预先存在的[策略](../resources/policy.md)中的属性。</span><span class="sxs-lookup"><span data-stu-id="b8b15-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8b15-105">权限</span><span class="sxs-lookup"><span data-stu-id="b8b15-105">Permissions</span></span>
<span data-ttu-id="b8b15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b15-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8b15-108">Permission type</span></span>      | <span data-ttu-id="b8b15-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8b15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8b15-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8b15-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8b15-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8b15-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8b15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8b15-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8b15-113">Not supported.</span></span>    |
|<span data-ttu-id="b8b15-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8b15-114">Application</span></span> | <span data-ttu-id="b8b15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8b15-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8b15-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8b15-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8b15-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8b15-117">Request headers</span></span>
| <span data-ttu-id="b8b15-118">名称</span><span class="sxs-lookup"><span data-stu-id="b8b15-118">Name</span></span>       | <span data-ttu-id="b8b15-119">类型</span><span class="sxs-lookup"><span data-stu-id="b8b15-119">Type</span></span> | <span data-ttu-id="b8b15-120">说明</span><span class="sxs-lookup"><span data-stu-id="b8b15-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8b15-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8b15-121">Authorization</span></span>  | <span data-ttu-id="b8b15-122">string</span><span class="sxs-lookup"><span data-stu-id="b8b15-122">string</span></span>  | <span data-ttu-id="b8b15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8b15-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8b15-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8b15-125">Content-Type</span></span> | <span data-ttu-id="b8b15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b15-126">application/json</span></span>  | <span data-ttu-id="b8b15-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="b8b15-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8b15-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8b15-129">Request body</span></span>
<span data-ttu-id="b8b15-130">在请求正文中, 提供具有需要更新的参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b8b15-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="b8b15-131">下表显示了可能的参数。</span><span class="sxs-lookup"><span data-stu-id="b8b15-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="b8b15-132">参数</span><span class="sxs-lookup"><span data-stu-id="b8b15-132">Parameter</span></span>    | <span data-ttu-id="b8b15-133">类型</span><span class="sxs-lookup"><span data-stu-id="b8b15-133">Type</span></span>   |<span data-ttu-id="b8b15-134">说明</span><span class="sxs-lookup"><span data-stu-id="b8b15-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8b15-135">定义</span><span class="sxs-lookup"><span data-stu-id="b8b15-135">definition</span></span>|<span data-ttu-id="b8b15-136">String</span><span class="sxs-lookup"><span data-stu-id="b8b15-136">String</span></span>|<span data-ttu-id="b8b15-137">[policy](../resources/policy.md)对象的字符串化版本。</span><span class="sxs-lookup"><span data-stu-id="b8b15-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="b8b15-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8b15-138">displayName</span></span>|<span data-ttu-id="b8b15-139">String</span><span class="sxs-lookup"><span data-stu-id="b8b15-139">String</span></span>|<span data-ttu-id="b8b15-140">策略的自定义名称。</span><span class="sxs-lookup"><span data-stu-id="b8b15-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="b8b15-141">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b8b15-141">isOrganizationDefault</span></span>|<span data-ttu-id="b8b15-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="b8b15-142">Boolean</span></span>|<span data-ttu-id="b8b15-143">指定默认情况下是否应用此策略。</span><span class="sxs-lookup"><span data-stu-id="b8b15-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="b8b15-144">类型</span><span class="sxs-lookup"><span data-stu-id="b8b15-144">type</span></span>|<span data-ttu-id="b8b15-145">String</span><span class="sxs-lookup"><span data-stu-id="b8b15-145">String</span></span>|<span data-ttu-id="b8b15-146">指定策略的类型。</span><span class="sxs-lookup"><span data-stu-id="b8b15-146">Specifies the type of policy.</span></span> <span data-ttu-id="b8b15-147">当前必须是 "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="b8b15-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="b8b15-148">响应</span><span class="sxs-lookup"><span data-stu-id="b8b15-148">Response</span></span>

<span data-ttu-id="b8b15-149">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b8b15-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="b8b15-150">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="b8b15-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="b8b15-151">示例</span><span class="sxs-lookup"><span data-stu-id="b8b15-151">Example</span></span>
<span data-ttu-id="b8b15-152">下面的示例更新令牌生存期策略的定义, 并将其设置为组织的默认值。</span><span class="sxs-lookup"><span data-stu-id="b8b15-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="b8b15-153">请求</span><span class="sxs-lookup"><span data-stu-id="b8b15-153">Request</span></span>
<span data-ttu-id="b8b15-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8b15-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="b8b15-155">响应</span><span class="sxs-lookup"><span data-stu-id="b8b15-155">Response</span></span>
<span data-ttu-id="b8b15-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8b15-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
