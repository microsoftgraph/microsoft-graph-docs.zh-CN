---
title: 列表应用程序和服务与特定的策略分配的安全主体
description: 检索与指定的策略分配的应用程序和服务主体对象。
ms.openlocfilehash: 3f281d7c60a506676a78637ad71f1ce26de35e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047911"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="40ccb-103">列表应用程序和服务与特定的策略分配的安全主体</span><span class="sxs-lookup"><span data-stu-id="40ccb-103">List Applications and Service Principals with specific Policy assigned</span></span>

> <span data-ttu-id="40ccb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="40ccb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40ccb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40ccb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40ccb-106">检索与指定的策略分配的[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40ccb-106">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="40ccb-107">权限</span><span class="sxs-lookup"><span data-stu-id="40ccb-107">Permissions</span></span>
<span data-ttu-id="40ccb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40ccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ccb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="40ccb-110">Permission type</span></span>      | <span data-ttu-id="40ccb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40ccb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ccb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40ccb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="40ccb-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40ccb-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40ccb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40ccb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ccb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ccb-115">Not supported.</span></span>    |
|<span data-ttu-id="40ccb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="40ccb-116">Application</span></span> | <span data-ttu-id="40ccb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ccb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40ccb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40ccb-118">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="40ccb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="40ccb-119">Request headers</span></span>
| <span data-ttu-id="40ccb-120">名称</span><span class="sxs-lookup"><span data-stu-id="40ccb-120">Name</span></span>       | <span data-ttu-id="40ccb-121">类型</span><span class="sxs-lookup"><span data-stu-id="40ccb-121">Type</span></span> | <span data-ttu-id="40ccb-122">说明</span><span class="sxs-lookup"><span data-stu-id="40ccb-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="40ccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ccb-123">Authorization</span></span>  | <span data-ttu-id="40ccb-124">string</span><span class="sxs-lookup"><span data-stu-id="40ccb-124">string</span></span>  | <span data-ttu-id="40ccb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40ccb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40ccb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40ccb-127">Request body</span></span>
<span data-ttu-id="40ccb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40ccb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ccb-129">响应</span><span class="sxs-lookup"><span data-stu-id="40ccb-129">Response</span></span>

<span data-ttu-id="40ccb-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40ccb-130">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="40ccb-131">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="40ccb-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="40ccb-132">示例</span><span class="sxs-lookup"><span data-stu-id="40ccb-132">Example</span></span>
<span data-ttu-id="40ccb-133">以下示例检索与特定的策略分配的应用程序和服务主体。</span><span class="sxs-lookup"><span data-stu-id="40ccb-133">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="40ccb-134">请求</span><span class="sxs-lookup"><span data-stu-id="40ccb-134">Request</span></span>
<span data-ttu-id="40ccb-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40ccb-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="40ccb-136">响应</span><span class="sxs-lookup"><span data-stu-id="40ccb-136">Response</span></span>
<span data-ttu-id="40ccb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40ccb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
