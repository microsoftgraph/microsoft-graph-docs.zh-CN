---
title: 列出分配了特定策略的应用程序和服务主体
description: 使用分配的指定策略检索应用程序和服务主体对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a3a24b3f54fa6d53b3936664be97cc3da0979a01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992085"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="2c0f9-103">列出分配了特定策略的应用程序和服务主体</span><span class="sxs-lookup"><span data-stu-id="2c0f9-103">List applications and service principals with specific policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c0f9-104">使用分配的指定策略检索[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c0f9-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c0f9-105">Permissions</span></span>
<span data-ttu-id="2c0f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c0f9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c0f9-108">Permission type</span></span>      | <span data-ttu-id="2c0f9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c0f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c0f9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c0f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c0f9-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c0f9-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c0f9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c0f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c0f9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-113">Not supported.</span></span>    |
|<span data-ttu-id="2c0f9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c0f9-114">Application</span></span> | <span data-ttu-id="2c0f9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c0f9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c0f9-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="2c0f9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c0f9-117">Request headers</span></span>
| <span data-ttu-id="2c0f9-118">名称</span><span class="sxs-lookup"><span data-stu-id="2c0f9-118">Name</span></span>       | <span data-ttu-id="2c0f9-119">类型</span><span class="sxs-lookup"><span data-stu-id="2c0f9-119">Type</span></span> | <span data-ttu-id="2c0f9-120">说明</span><span class="sxs-lookup"><span data-stu-id="2c0f9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c0f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c0f9-121">Authorization</span></span>  | <span data-ttu-id="2c0f9-122">string</span><span class="sxs-lookup"><span data-stu-id="2c0f9-122">string</span></span>  | <span data-ttu-id="2c0f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c0f9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c0f9-125">Request body</span></span>
<span data-ttu-id="2c0f9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c0f9-127">响应</span><span class="sxs-lookup"><span data-stu-id="2c0f9-127">Response</span></span>

<span data-ttu-id="2c0f9-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="2c0f9-129">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="2c0f9-130">示例</span><span class="sxs-lookup"><span data-stu-id="2c0f9-130">Example</span></span>
<span data-ttu-id="2c0f9-131">下面的示例检索分配了特定策略的应用程序和服务主体。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="2c0f9-132">请求</span><span class="sxs-lookup"><span data-stu-id="2c0f9-132">Request</span></span>
<span data-ttu-id="2c0f9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="2c0f9-134">响应</span><span class="sxs-lookup"><span data-stu-id="2c0f9-134">Response</span></span>
<span data-ttu-id="2c0f9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c0f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
