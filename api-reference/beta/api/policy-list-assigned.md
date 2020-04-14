---
title: 为应用程序或服务主体分配的列表策略
description: 获取分配给应用程序或服务主体的策略对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: dkershaw10
ms.openlocfilehash: beb5afedd33d16fefaaeb83c46fddd45c9c9ad3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408369"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="fc905-103">为应用程序或服务主体分配的列表策略</span><span class="sxs-lookup"><span data-stu-id="fc905-103">List Policies assigned to Application or Service Principal</span></span>

<span data-ttu-id="fc905-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc905-105">获取分配给应用程序或服务主体的[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc905-105">Get the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc905-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc905-106">Permissions</span></span>
<span data-ttu-id="fc905-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc905-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc905-109">Permission type</span></span>      | <span data-ttu-id="fc905-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc905-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc905-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc905-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc905-112">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc905-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc905-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc905-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc905-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc905-114">Not supported.</span></span>    |
|<span data-ttu-id="fc905-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc905-115">Application</span></span> | <span data-ttu-id="fc905-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc905-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc905-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc905-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="fc905-118">注意：请求中的 "id" 是应用程序或服务主体的 "id" 属性，而不是 "appid" 属性。</span><span class="sxs-lookup"><span data-stu-id="fc905-118">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc905-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc905-119">Request headers</span></span>
| <span data-ttu-id="fc905-120">名称</span><span class="sxs-lookup"><span data-stu-id="fc905-120">Name</span></span>       | <span data-ttu-id="fc905-121">类型</span><span class="sxs-lookup"><span data-stu-id="fc905-121">Type</span></span> | <span data-ttu-id="fc905-122">说明</span><span class="sxs-lookup"><span data-stu-id="fc905-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc905-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc905-123">Authorization</span></span>  | <span data-ttu-id="fc905-124">string</span><span class="sxs-lookup"><span data-stu-id="fc905-124">string</span></span>  | <span data-ttu-id="fc905-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc905-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc905-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc905-127">Request body</span></span>
<span data-ttu-id="fc905-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc905-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc905-129">响应</span><span class="sxs-lookup"><span data-stu-id="fc905-129">Response</span></span>

<span data-ttu-id="fc905-130">如果成功，此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc905-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="fc905-131">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc905-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="fc905-132">示例</span><span class="sxs-lookup"><span data-stu-id="fc905-132">Example</span></span>
<span data-ttu-id="fc905-133">下面的示例检索分配给应用程序的策略。</span><span class="sxs-lookup"><span data-stu-id="fc905-133">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="fc905-134">请求</span><span class="sxs-lookup"><span data-stu-id="fc905-134">Request</span></span>
<span data-ttu-id="fc905-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc905-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="fc905-136">响应</span><span class="sxs-lookup"><span data-stu-id="fc905-136">Response</span></span>
<span data-ttu-id="fc905-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc905-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
