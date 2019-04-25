---
title: 分配策略
description: 将策略分配给应用程序或服务主体。
localization_priority: Normal
ms.openlocfilehash: 15ba6a42f5c5d39caf57b25ebafc5dd4bc7990fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546785"
---
# <a name="assign-policy"></a><span data-ttu-id="eb4a8-103">分配策略</span><span class="sxs-lookup"><span data-stu-id="eb4a8-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb4a8-104">将[策略](../resources/policy.md)分配给应用程序或服务主体。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="eb4a8-105">注意: 目前, 策略分配仅适用于令牌生存期策略。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="eb4a8-106">[策略](../resources/policy.md)中介绍了这种类型的策略。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb4a8-107">权限</span><span class="sxs-lookup"><span data-stu-id="eb4a8-107">Permissions</span></span>
<span data-ttu-id="eb4a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb4a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb4a8-110">Permission type</span></span>      | <span data-ttu-id="eb4a8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb4a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb4a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb4a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eb4a8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb4a8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb4a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb4a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb4a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-115">Not supported.</span></span>    |
|<span data-ttu-id="eb4a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb4a8-116">Application</span></span> | <span data-ttu-id="eb4a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb4a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb4a8-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="eb4a8-119">注意: 请求中的 "id" 是应用程序或服务主体的 "id" 属性, 而不是 "appid" 属性。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb4a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb4a8-120">Request headers</span></span>
| <span data-ttu-id="eb4a8-121">名称</span><span class="sxs-lookup"><span data-stu-id="eb4a8-121">Name</span></span>       | <span data-ttu-id="eb4a8-122">类型</span><span class="sxs-lookup"><span data-stu-id="eb4a8-122">Type</span></span> | <span data-ttu-id="eb4a8-123">说明</span><span class="sxs-lookup"><span data-stu-id="eb4a8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb4a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb4a8-124">Authorization</span></span>  | <span data-ttu-id="eb4a8-125">string</span><span class="sxs-lookup"><span data-stu-id="eb4a8-125">string</span></span>  | <span data-ttu-id="eb4a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb4a8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb4a8-128">Content-Type</span></span> | <span data-ttu-id="eb4a8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="eb4a8-129">application/json</span></span>  | <span data-ttu-id="eb4a8-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb4a8-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb4a8-132">Request body</span></span>
<span data-ttu-id="eb4a8-133">在请求正文中, 提供要添加的策略对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="eb4a8-134">响应</span><span class="sxs-lookup"><span data-stu-id="eb4a8-134">Response</span></span>

<span data-ttu-id="eb4a8-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="eb4a8-136">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="eb4a8-137">示例</span><span class="sxs-lookup"><span data-stu-id="eb4a8-137">Example</span></span>
<span data-ttu-id="eb4a8-138">下面的示例将策略分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="eb4a8-139">请求</span><span class="sxs-lookup"><span data-stu-id="eb4a8-139">Request</span></span>
<span data-ttu-id="eb4a8-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="eb4a8-141">响应</span><span class="sxs-lookup"><span data-stu-id="eb4a8-141">Response</span></span>
<span data-ttu-id="eb4a8-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb4a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-assign.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
