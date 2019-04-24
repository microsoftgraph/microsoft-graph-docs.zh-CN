---
title: 列出 groupLifecyclePolicy
description: 检索组所属的 groupLifecyclePolicy 对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 56ba6f47e1ccd0784f76204d0101171406263397
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502436"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="bae75-103">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bae75-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="bae75-104">检索组所属的 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bae75-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="bae75-105">权限</span><span class="sxs-lookup"><span data-stu-id="bae75-105">Permissions</span></span>

<span data-ttu-id="bae75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bae75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae75-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bae75-108">Permission type</span></span>      | <span data-ttu-id="bae75-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bae75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bae75-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bae75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bae75-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bae75-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="bae75-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bae75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae75-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bae75-113">Not supported.</span></span>    |
|<span data-ttu-id="bae75-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bae75-114">Application</span></span> | <span data-ttu-id="bae75-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bae75-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bae75-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bae75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bae75-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bae75-117">Optional query parameters</span></span>
<span data-ttu-id="bae75-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bae75-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bae75-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bae75-119">Request headers</span></span>
| <span data-ttu-id="bae75-120">名称</span><span class="sxs-lookup"><span data-stu-id="bae75-120">Name</span></span> | <span data-ttu-id="bae75-121">说明</span><span class="sxs-lookup"><span data-stu-id="bae75-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="bae75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae75-122">Authorization</span></span> | <span data-ttu-id="bae75-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bae75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bae75-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bae75-125">Request body</span></span>
<span data-ttu-id="bae75-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bae75-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bae75-127">响应</span><span class="sxs-lookup"><span data-stu-id="bae75-127">Response</span></span>
<span data-ttu-id="bae75-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bae75-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bae75-129">示例</span><span class="sxs-lookup"><span data-stu-id="bae75-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bae75-130">请求</span><span class="sxs-lookup"><span data-stu-id="bae75-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="bae75-131">响应</span><span class="sxs-lookup"><span data-stu-id="bae75-131">Response</span></span>

<span data-ttu-id="bae75-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bae75-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
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
