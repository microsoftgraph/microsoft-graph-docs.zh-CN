---
title: 列出分配了特定策略的应用程序和服务主体
description: 获取分配了指定策略的应用程序和服务主体对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7959f8b286f1068de454f6d0d36a182f190efafd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455520"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="ff97e-103">列出分配了特定策略的应用程序和服务主体</span><span class="sxs-lookup"><span data-stu-id="ff97e-103">List applications and service principals with specific policy assigned</span></span>

<span data-ttu-id="ff97e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff97e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff97e-105">获取分配了指定策略的[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff97e-105">Get the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff97e-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff97e-106">Permissions</span></span>
<span data-ttu-id="ff97e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff97e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff97e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff97e-109">Permission type</span></span>      | <span data-ttu-id="ff97e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff97e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff97e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff97e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff97e-112">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff97e-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff97e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff97e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff97e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff97e-114">Not supported.</span></span>    |
|<span data-ttu-id="ff97e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff97e-115">Application</span></span> | <span data-ttu-id="ff97e-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff97e-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff97e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff97e-117">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="ff97e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff97e-118">Request headers</span></span>
| <span data-ttu-id="ff97e-119">名称</span><span class="sxs-lookup"><span data-stu-id="ff97e-119">Name</span></span>       | <span data-ttu-id="ff97e-120">类型</span><span class="sxs-lookup"><span data-stu-id="ff97e-120">Type</span></span> | <span data-ttu-id="ff97e-121">说明</span><span class="sxs-lookup"><span data-stu-id="ff97e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff97e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff97e-122">Authorization</span></span>  | <span data-ttu-id="ff97e-123">string</span><span class="sxs-lookup"><span data-stu-id="ff97e-123">string</span></span>  | <span data-ttu-id="ff97e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff97e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff97e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff97e-126">Request body</span></span>
<span data-ttu-id="ff97e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff97e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff97e-128">响应</span><span class="sxs-lookup"><span data-stu-id="ff97e-128">Response</span></span>

<span data-ttu-id="ff97e-129">如果成功，此方法在`200 OK`响应正文中返回响应代码和[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ff97e-129">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="ff97e-130">如果失败，将返回 `4xx` 错误并显示具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="ff97e-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="ff97e-131">示例</span><span class="sxs-lookup"><span data-stu-id="ff97e-131">Example</span></span>
<span data-ttu-id="ff97e-132">下面的示例检索分配了特定策略的应用程序和服务主体。</span><span class="sxs-lookup"><span data-stu-id="ff97e-132">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="ff97e-133">请求</span><span class="sxs-lookup"><span data-stu-id="ff97e-133">Request</span></span>
<span data-ttu-id="ff97e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff97e-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="ff97e-135">响应</span><span class="sxs-lookup"><span data-stu-id="ff97e-135">Response</span></span>
<span data-ttu-id="ff97e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff97e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
