---
title: 列表应用程序和服务与特定的策略分配的安全主体
description: 检索与指定的策略分配的应用程序和服务主体对象。
localization_priority: Normal
ms.openlocfilehash: d7449428216a2e68d9ab8bb8399ca0e8dc4b72fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510475"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="9fb86-103">列表应用程序和服务与特定的策略分配的安全主体</span><span class="sxs-lookup"><span data-stu-id="9fb86-103">List Applications and Service Principals with specific Policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fb86-104">检索与指定的策略分配的[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fb86-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb86-105">权限</span><span class="sxs-lookup"><span data-stu-id="9fb86-105">Permissions</span></span>
<span data-ttu-id="9fb86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fb86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb86-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fb86-108">Permission type</span></span>      | <span data-ttu-id="9fb86-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fb86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb86-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fb86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9fb86-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9fb86-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9fb86-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fb86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb86-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fb86-113">Not supported.</span></span>    |
|<span data-ttu-id="9fb86-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fb86-114">Application</span></span> | <span data-ttu-id="9fb86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fb86-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb86-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fb86-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="9fb86-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fb86-117">Request headers</span></span>
| <span data-ttu-id="9fb86-118">名称</span><span class="sxs-lookup"><span data-stu-id="9fb86-118">Name</span></span>       | <span data-ttu-id="9fb86-119">类型</span><span class="sxs-lookup"><span data-stu-id="9fb86-119">Type</span></span> | <span data-ttu-id="9fb86-120">说明</span><span class="sxs-lookup"><span data-stu-id="9fb86-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9fb86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fb86-121">Authorization</span></span>  | <span data-ttu-id="9fb86-122">string</span><span class="sxs-lookup"><span data-stu-id="9fb86-122">string</span></span>  | <span data-ttu-id="9fb86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fb86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fb86-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fb86-125">Request body</span></span>
<span data-ttu-id="9fb86-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fb86-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb86-127">响应</span><span class="sxs-lookup"><span data-stu-id="9fb86-127">Response</span></span>

<span data-ttu-id="9fb86-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fb86-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="9fb86-129">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="9fb86-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="9fb86-130">示例</span><span class="sxs-lookup"><span data-stu-id="9fb86-130">Example</span></span>
<span data-ttu-id="9fb86-131">以下示例检索与特定的策略分配的应用程序和服务主体。</span><span class="sxs-lookup"><span data-stu-id="9fb86-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="9fb86-132">请求</span><span class="sxs-lookup"><span data-stu-id="9fb86-132">Request</span></span>
<span data-ttu-id="9fb86-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fb86-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="9fb86-134">响应</span><span class="sxs-lookup"><span data-stu-id="9fb86-134">Response</span></span>
<span data-ttu-id="9fb86-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fb86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-appliesto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
