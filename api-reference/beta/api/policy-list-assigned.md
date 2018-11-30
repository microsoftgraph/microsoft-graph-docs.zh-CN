---
title: 分配给应用程序或服务主体的列表策略
description: 检索分配给应用程序或服务主体的策略对象。
ms.openlocfilehash: cfdcf3d8e6709080f4c8f7bfc3e2dbc256789f6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044011"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="beecc-103">分配给应用程序或服务主体的列表策略</span><span class="sxs-lookup"><span data-stu-id="beecc-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="beecc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="beecc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beecc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="beecc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="beecc-106">检索分配给应用程序或服务主体的[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="beecc-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="beecc-107">权限</span><span class="sxs-lookup"><span data-stu-id="beecc-107">Permissions</span></span>
<span data-ttu-id="beecc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="beecc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beecc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="beecc-110">Permission type</span></span>      | <span data-ttu-id="beecc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="beecc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beecc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="beecc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="beecc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="beecc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="beecc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="beecc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beecc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="beecc-115">Not supported.</span></span>    |
|<span data-ttu-id="beecc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="beecc-116">Application</span></span> | <span data-ttu-id="beecc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="beecc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="beecc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="beecc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="beecc-119">注意： 请求中的"id"为应用程序或服务主体，不是"appid"属性"id"属性。</span><span class="sxs-lookup"><span data-stu-id="beecc-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="beecc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="beecc-120">Request headers</span></span>
| <span data-ttu-id="beecc-121">名称</span><span class="sxs-lookup"><span data-stu-id="beecc-121">Name</span></span>       | <span data-ttu-id="beecc-122">类型</span><span class="sxs-lookup"><span data-stu-id="beecc-122">Type</span></span> | <span data-ttu-id="beecc-123">说明</span><span class="sxs-lookup"><span data-stu-id="beecc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="beecc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="beecc-124">Authorization</span></span>  | <span data-ttu-id="beecc-125">string</span><span class="sxs-lookup"><span data-stu-id="beecc-125">string</span></span>  | <span data-ttu-id="beecc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="beecc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beecc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="beecc-128">Request body</span></span>
<span data-ttu-id="beecc-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="beecc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beecc-130">响应</span><span class="sxs-lookup"><span data-stu-id="beecc-130">Response</span></span>

<span data-ttu-id="beecc-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="beecc-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="beecc-132">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="beecc-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="beecc-133">示例</span><span class="sxs-lookup"><span data-stu-id="beecc-133">Example</span></span>
<span data-ttu-id="beecc-134">以下示例检索分配给应用程序的策略。</span><span class="sxs-lookup"><span data-stu-id="beecc-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="beecc-135">请求</span><span class="sxs-lookup"><span data-stu-id="beecc-135">Request</span></span>
<span data-ttu-id="beecc-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="beecc-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="beecc-137">响应</span><span class="sxs-lookup"><span data-stu-id="beecc-137">Response</span></span>
<span data-ttu-id="beecc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="beecc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
