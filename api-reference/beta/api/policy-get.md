---
title: 获取策略
description: 检索策略的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 435e711c711675b94b089d818b7451b551f8b5ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978873"
---
# <a name="get-policy"></a><span data-ttu-id="2393f-103">获取策略</span><span class="sxs-lookup"><span data-stu-id="2393f-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2393f-104">检索[策略](../resources/policy.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="2393f-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2393f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2393f-105">Permissions</span></span>
<span data-ttu-id="2393f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2393f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2393f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2393f-108">Permission type</span></span>      | <span data-ttu-id="2393f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2393f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2393f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2393f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2393f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2393f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2393f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2393f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2393f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2393f-113">Not supported.</span></span>    |
|<span data-ttu-id="2393f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2393f-114">Application</span></span> | <span data-ttu-id="2393f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2393f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2393f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2393f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2393f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2393f-117">Request headers</span></span>
| <span data-ttu-id="2393f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2393f-118">Name</span></span>       | <span data-ttu-id="2393f-119">类型</span><span class="sxs-lookup"><span data-stu-id="2393f-119">Type</span></span> | <span data-ttu-id="2393f-120">说明</span><span class="sxs-lookup"><span data-stu-id="2393f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2393f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2393f-121">Authorization</span></span>  | <span data-ttu-id="2393f-122">string</span><span class="sxs-lookup"><span data-stu-id="2393f-122">string</span></span>  | <span data-ttu-id="2393f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2393f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2393f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2393f-125">Request body</span></span>
<span data-ttu-id="2393f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2393f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2393f-127">响应</span><span class="sxs-lookup"><span data-stu-id="2393f-127">Response</span></span>

<span data-ttu-id="2393f-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2393f-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="2393f-129">如果 unsucccessful</span><span class="sxs-lookup"><span data-stu-id="2393f-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="2393f-130">示例</span><span class="sxs-lookup"><span data-stu-id="2393f-130">Example</span></span>
<span data-ttu-id="2393f-131">下面的示例检索特定策略。</span><span class="sxs-lookup"><span data-stu-id="2393f-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="2393f-132">请求</span><span class="sxs-lookup"><span data-stu-id="2393f-132">Request</span></span>
<span data-ttu-id="2393f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2393f-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="2393f-134">响应</span><span class="sxs-lookup"><span data-stu-id="2393f-134">Response</span></span>
<span data-ttu-id="2393f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2393f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
