---
title: 分配策略
description: 将策略分配到应用程序或服务主体。
ms.openlocfilehash: 25dee4ac43716949125795114318d2571d5b8647
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047912"
---
# <a name="assign-policy"></a><span data-ttu-id="645fc-103">分配策略</span><span class="sxs-lookup"><span data-stu-id="645fc-103">Assign Policy</span></span>

> <span data-ttu-id="645fc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="645fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="645fc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="645fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="645fc-106">将[策略](../resources/policy.md)分配到应用程序或服务主体。</span><span class="sxs-lookup"><span data-stu-id="645fc-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="645fc-107">注意： 目前，策略分配仅适用于令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="645fc-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="645fc-108">在[策略](../resources/policy.md)中介绍了这种类型的策略。</span><span class="sxs-lookup"><span data-stu-id="645fc-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="645fc-109">权限</span><span class="sxs-lookup"><span data-stu-id="645fc-109">Permissions</span></span>
<span data-ttu-id="645fc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="645fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="645fc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="645fc-112">Permission type</span></span>      | <span data-ttu-id="645fc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="645fc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="645fc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="645fc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="645fc-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="645fc-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="645fc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="645fc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="645fc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="645fc-117">Not supported.</span></span>    |
|<span data-ttu-id="645fc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="645fc-118">Application</span></span> | <span data-ttu-id="645fc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="645fc-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="645fc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="645fc-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="645fc-121">注意： 请求中的"id"为应用程序或服务主体，不是"appid"属性"id"属性。</span><span class="sxs-lookup"><span data-stu-id="645fc-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="645fc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="645fc-122">Request headers</span></span>
| <span data-ttu-id="645fc-123">名称</span><span class="sxs-lookup"><span data-stu-id="645fc-123">Name</span></span>       | <span data-ttu-id="645fc-124">类型</span><span class="sxs-lookup"><span data-stu-id="645fc-124">Type</span></span> | <span data-ttu-id="645fc-125">说明</span><span class="sxs-lookup"><span data-stu-id="645fc-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="645fc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="645fc-126">Authorization</span></span>  | <span data-ttu-id="645fc-127">string</span><span class="sxs-lookup"><span data-stu-id="645fc-127">string</span></span>  | <span data-ttu-id="645fc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="645fc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="645fc-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="645fc-130">Content-Type</span></span> | <span data-ttu-id="645fc-131">application/json</span><span class="sxs-lookup"><span data-stu-id="645fc-131">application/json</span></span>  | <span data-ttu-id="645fc-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="645fc-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="645fc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="645fc-134">Request body</span></span>
<span data-ttu-id="645fc-135">在请求正文中，提供要添加的策略对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="645fc-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="645fc-136">响应</span><span class="sxs-lookup"><span data-stu-id="645fc-136">Response</span></span>

<span data-ttu-id="645fc-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="645fc-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="645fc-138">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="645fc-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="645fc-139">示例</span><span class="sxs-lookup"><span data-stu-id="645fc-139">Example</span></span>
<span data-ttu-id="645fc-140">下面的示例将策略分配到应用程序。</span><span class="sxs-lookup"><span data-stu-id="645fc-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="645fc-141">请求</span><span class="sxs-lookup"><span data-stu-id="645fc-141">Request</span></span>
<span data-ttu-id="645fc-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="645fc-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="645fc-143">响应</span><span class="sxs-lookup"><span data-stu-id="645fc-143">Response</span></span>
<span data-ttu-id="645fc-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="645fc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
