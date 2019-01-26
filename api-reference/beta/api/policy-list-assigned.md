---
title: 分配给应用程序或服务主体的列表策略
description: 检索分配给应用程序或服务主体的策略对象。
localization_priority: Normal
ms.openlocfilehash: 417d59228aadd3c6a54c4634416fd577fce11f18
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575959"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="78f2a-103">分配给应用程序或服务主体的列表策略</span><span class="sxs-lookup"><span data-stu-id="78f2a-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f2a-104">检索分配给应用程序或服务主体的[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="78f2a-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="78f2a-105">权限</span><span class="sxs-lookup"><span data-stu-id="78f2a-105">Permissions</span></span>
<span data-ttu-id="78f2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78f2a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="78f2a-108">Permission type</span></span>      | <span data-ttu-id="78f2a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78f2a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78f2a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78f2a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78f2a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="78f2a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="78f2a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78f2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f2a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="78f2a-113">Not supported.</span></span>    |
|<span data-ttu-id="78f2a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="78f2a-114">Application</span></span> | <span data-ttu-id="78f2a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78f2a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78f2a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78f2a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="78f2a-117">注意： 请求中的"id"为应用程序或服务主体，不是"appid"属性"id"属性。</span><span class="sxs-lookup"><span data-stu-id="78f2a-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78f2a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="78f2a-118">Request headers</span></span>
| <span data-ttu-id="78f2a-119">名称</span><span class="sxs-lookup"><span data-stu-id="78f2a-119">Name</span></span>       | <span data-ttu-id="78f2a-120">类型</span><span class="sxs-lookup"><span data-stu-id="78f2a-120">Type</span></span> | <span data-ttu-id="78f2a-121">说明</span><span class="sxs-lookup"><span data-stu-id="78f2a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78f2a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f2a-122">Authorization</span></span>  | <span data-ttu-id="78f2a-123">string</span><span class="sxs-lookup"><span data-stu-id="78f2a-123">string</span></span>  | <span data-ttu-id="78f2a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78f2a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78f2a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="78f2a-126">Request body</span></span>
<span data-ttu-id="78f2a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78f2a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78f2a-128">响应</span><span class="sxs-lookup"><span data-stu-id="78f2a-128">Response</span></span>

<span data-ttu-id="78f2a-129">如果成功，此方法返回`200 OK`响应正文中的响应代码和[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="78f2a-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="78f2a-130">如果不成功，`4xx`与特定的详细信息，则返回错误。</span><span class="sxs-lookup"><span data-stu-id="78f2a-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="78f2a-131">示例</span><span class="sxs-lookup"><span data-stu-id="78f2a-131">Example</span></span>
<span data-ttu-id="78f2a-132">以下示例检索分配给应用程序的策略。</span><span class="sxs-lookup"><span data-stu-id="78f2a-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="78f2a-133">请求</span><span class="sxs-lookup"><span data-stu-id="78f2a-133">Request</span></span>
<span data-ttu-id="78f2a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78f2a-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="78f2a-135">响应</span><span class="sxs-lookup"><span data-stu-id="78f2a-135">Response</span></span>
<span data-ttu-id="78f2a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78f2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
            "isOrganizationDefault": true | false,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-assigned.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
