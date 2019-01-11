---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: da0251e044912c4ee5b107f7ec0c7e052ddb0046
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864440"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="5559f-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="5559f-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="5559f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5559f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5559f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5559f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5559f-106">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="5559f-106">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5559f-107">权限</span><span class="sxs-lookup"><span data-stu-id="5559f-107">Permissions</span></span>

<span data-ttu-id="5559f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5559f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5559f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5559f-110">Permission type</span></span>      | <span data-ttu-id="5559f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5559f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5559f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5559f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5559f-113">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5559f-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="5559f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5559f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5559f-115">不支持</span><span class="sxs-lookup"><span data-stu-id="5559f-115">Not supported</span></span> |
|<span data-ttu-id="5559f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5559f-116">Application</span></span> | <span data-ttu-id="5559f-117">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5559f-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5559f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5559f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5559f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5559f-119">Optional query parameters</span></span>
<span data-ttu-id="5559f-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5559f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5559f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5559f-121">Request headers</span></span>
| <span data-ttu-id="5559f-122">名称</span><span class="sxs-lookup"><span data-stu-id="5559f-122">Name</span></span> | <span data-ttu-id="5559f-123">说明</span><span class="sxs-lookup"><span data-stu-id="5559f-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="5559f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5559f-124">Authorization</span></span> | <span data-ttu-id="5559f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5559f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5559f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5559f-127">Request body</span></span>
<span data-ttu-id="5559f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5559f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5559f-129">响应</span><span class="sxs-lookup"><span data-stu-id="5559f-129">Response</span></span>

<span data-ttu-id="5559f-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5559f-130">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5559f-131">示例</span><span class="sxs-lookup"><span data-stu-id="5559f-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5559f-132">请求</span><span class="sxs-lookup"><span data-stu-id="5559f-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="5559f-133">响应</span><span class="sxs-lookup"><span data-stu-id="5559f-133">Response</span></span>

<span data-ttu-id="5559f-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5559f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
