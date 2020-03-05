---
title: 获取策略
description: 检索策略的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: d9813151c2dde323ed685592ad6c00979d9c3f01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455538"
---
# <a name="get-policy"></a><span data-ttu-id="798d7-103">获取策略</span><span class="sxs-lookup"><span data-stu-id="798d7-103">Get Policy</span></span>

<span data-ttu-id="798d7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="798d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="798d7-105">检索[策略](../resources/policy.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="798d7-105">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="798d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="798d7-106">Permissions</span></span>
<span data-ttu-id="798d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="798d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="798d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="798d7-109">Permission type</span></span>      | <span data-ttu-id="798d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="798d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="798d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="798d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="798d7-112">Policy： All、Directory.accessasuser.all、All、All</span><span class="sxs-lookup"><span data-stu-id="798d7-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="798d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="798d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="798d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="798d7-114">Not supported.</span></span>    |
|<span data-ttu-id="798d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="798d7-115">Application</span></span> | <span data-ttu-id="798d7-116">Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="798d7-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="798d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="798d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="798d7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="798d7-118">Request headers</span></span>
| <span data-ttu-id="798d7-119">名称</span><span class="sxs-lookup"><span data-stu-id="798d7-119">Name</span></span>       | <span data-ttu-id="798d7-120">类型</span><span class="sxs-lookup"><span data-stu-id="798d7-120">Type</span></span> | <span data-ttu-id="798d7-121">说明</span><span class="sxs-lookup"><span data-stu-id="798d7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="798d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="798d7-122">Authorization</span></span>  | <span data-ttu-id="798d7-123">string</span><span class="sxs-lookup"><span data-stu-id="798d7-123">string</span></span>  | <span data-ttu-id="798d7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="798d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="798d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="798d7-126">Request body</span></span>
<span data-ttu-id="798d7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="798d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="798d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="798d7-128">Response</span></span>

<span data-ttu-id="798d7-129">如果成功，此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="798d7-129">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="798d7-130">如果 unsucccessful</span><span class="sxs-lookup"><span data-stu-id="798d7-130">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="798d7-131">示例</span><span class="sxs-lookup"><span data-stu-id="798d7-131">Example</span></span>
<span data-ttu-id="798d7-132">下面的示例检索特定策略。</span><span class="sxs-lookup"><span data-stu-id="798d7-132">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="798d7-133">请求</span><span class="sxs-lookup"><span data-stu-id="798d7-133">Request</span></span>
<span data-ttu-id="798d7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="798d7-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="798d7-135">响应</span><span class="sxs-lookup"><span data-stu-id="798d7-135">Response</span></span>
<span data-ttu-id="798d7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="798d7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
