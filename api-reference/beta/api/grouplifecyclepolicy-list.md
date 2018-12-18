---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: dkershaw10
ms.openlocfilehash: e926d071121986e1aa06511ef8ec84e6b0cd55b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350328"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="1e7ef-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="1e7ef-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="1e7ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e7ef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e7ef-106">列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-106">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e7ef-107">权限</span><span class="sxs-lookup"><span data-stu-id="1e7ef-107">Permissions</span></span>

<span data-ttu-id="1e7ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e7ef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e7ef-110">Permission type</span></span>      | <span data-ttu-id="1e7ef-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e7ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e7ef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e7ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e7ef-113">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e7ef-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1e7ef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e7ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e7ef-115">不支持</span><span class="sxs-lookup"><span data-stu-id="1e7ef-115">Not supported</span></span> |
|<span data-ttu-id="1e7ef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e7ef-116">Application</span></span> | <span data-ttu-id="1e7ef-117">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e7ef-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e7ef-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e7ef-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e7ef-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e7ef-119">Optional query parameters</span></span>
<span data-ttu-id="1e7ef-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e7ef-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e7ef-121">Request headers</span></span>
| <span data-ttu-id="1e7ef-122">Name</span><span class="sxs-lookup"><span data-stu-id="1e7ef-122">Name</span></span> | <span data-ttu-id="1e7ef-123">说明</span><span class="sxs-lookup"><span data-stu-id="1e7ef-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="1e7ef-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e7ef-124">Authorization</span></span> | <span data-ttu-id="1e7ef-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e7ef-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e7ef-127">Request body</span></span>
<span data-ttu-id="1e7ef-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e7ef-129">响应</span><span class="sxs-lookup"><span data-stu-id="1e7ef-129">Response</span></span>

<span data-ttu-id="1e7ef-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-130">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e7ef-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e7ef-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1e7ef-132">请求</span><span class="sxs-lookup"><span data-stu-id="1e7ef-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="1e7ef-133">响应</span><span class="sxs-lookup"><span data-stu-id="1e7ef-133">Response</span></span>

<span data-ttu-id="1e7ef-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e7ef-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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