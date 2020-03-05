---
title: 分配策略
description: 将策略分配给应用程序或服务主体。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f005973677ca3e430706a7fced22e5fbf51bcd0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455532"
---
# <a name="assign-policy"></a><span data-ttu-id="6aa2b-103">分配策略</span><span class="sxs-lookup"><span data-stu-id="6aa2b-103">Assign Policy</span></span>

<span data-ttu-id="6aa2b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6aa2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aa2b-105">将[策略](../resources/policy.md)分配给应用程序或服务主体。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-105">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="6aa2b-106">注意：目前，策略分配仅适用于令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-106">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="6aa2b-107">[策略](../resources/policy.md)中介绍了这种类型的策略。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-107">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6aa2b-108">权限</span><span class="sxs-lookup"><span data-stu-id="6aa2b-108">Permissions</span></span>
<span data-ttu-id="6aa2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aa2b-111">Permission type</span></span>      | <span data-ttu-id="6aa2b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6aa2b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aa2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aa2b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6aa2b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6aa2b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6aa2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aa2b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-116">Not supported.</span></span>    |
|<span data-ttu-id="6aa2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aa2b-117">Application</span></span> | <span data-ttu-id="6aa2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aa2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aa2b-119">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="6aa2b-120">注意：请求中的 "id" 是应用程序或服务主体的 "id" 属性，而不是 "appid" 属性。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-120">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aa2b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aa2b-121">Request headers</span></span>
| <span data-ttu-id="6aa2b-122">名称</span><span class="sxs-lookup"><span data-stu-id="6aa2b-122">Name</span></span>       | <span data-ttu-id="6aa2b-123">类型</span><span class="sxs-lookup"><span data-stu-id="6aa2b-123">Type</span></span> | <span data-ttu-id="6aa2b-124">说明</span><span class="sxs-lookup"><span data-stu-id="6aa2b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6aa2b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aa2b-125">Authorization</span></span>  | <span data-ttu-id="6aa2b-126">string</span><span class="sxs-lookup"><span data-stu-id="6aa2b-126">string</span></span>  | <span data-ttu-id="6aa2b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6aa2b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6aa2b-129">Content-Type</span></span> | <span data-ttu-id="6aa2b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa2b-130">application/json</span></span>  | <span data-ttu-id="6aa2b-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aa2b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aa2b-133">Request body</span></span>
<span data-ttu-id="6aa2b-134">在请求正文中，提供要添加的策略对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-134">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6aa2b-135">响应</span><span class="sxs-lookup"><span data-stu-id="6aa2b-135">Response</span></span>

<span data-ttu-id="6aa2b-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-136">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="6aa2b-137">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6aa2b-138">示例</span><span class="sxs-lookup"><span data-stu-id="6aa2b-138">Example</span></span>
<span data-ttu-id="6aa2b-139">下面的示例将策略分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-139">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="6aa2b-140">请求</span><span class="sxs-lookup"><span data-stu-id="6aa2b-140">Request</span></span>
<span data-ttu-id="6aa2b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-141">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="6aa2b-142">响应</span><span class="sxs-lookup"><span data-stu-id="6aa2b-142">Response</span></span>
<span data-ttu-id="6aa2b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aa2b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
