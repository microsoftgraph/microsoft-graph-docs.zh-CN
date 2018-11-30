---
title: 获取策略
description: 检索策略的属性。
ms.openlocfilehash: a6827813193d134f54c3274e2b035e241bb99dc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042752"
---
# <a name="get-policy"></a><span data-ttu-id="68152-103">获取策略</span><span class="sxs-lookup"><span data-stu-id="68152-103">Get Policy</span></span>

> <span data-ttu-id="68152-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68152-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68152-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68152-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68152-106">检索[策略](../resources/policy.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="68152-106">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="68152-107">权限</span><span class="sxs-lookup"><span data-stu-id="68152-107">Permissions</span></span>
<span data-ttu-id="68152-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68152-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68152-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68152-110">Permission type</span></span>      | <span data-ttu-id="68152-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68152-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68152-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68152-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68152-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68152-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68152-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68152-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68152-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="68152-115">Not supported.</span></span>    |
|<span data-ttu-id="68152-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="68152-116">Application</span></span> | <span data-ttu-id="68152-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="68152-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68152-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68152-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="68152-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68152-119">Request headers</span></span>
| <span data-ttu-id="68152-120">名称</span><span class="sxs-lookup"><span data-stu-id="68152-120">Name</span></span>       | <span data-ttu-id="68152-121">类型</span><span class="sxs-lookup"><span data-stu-id="68152-121">Type</span></span> | <span data-ttu-id="68152-122">说明</span><span class="sxs-lookup"><span data-stu-id="68152-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68152-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68152-123">Authorization</span></span>  | <span data-ttu-id="68152-124">string</span><span class="sxs-lookup"><span data-stu-id="68152-124">string</span></span>  | <span data-ttu-id="68152-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68152-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68152-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="68152-127">Request body</span></span>
<span data-ttu-id="68152-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68152-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68152-129">响应</span><span class="sxs-lookup"><span data-stu-id="68152-129">Response</span></span>

<span data-ttu-id="68152-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="68152-130">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="68152-131">如果 unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="68152-131">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="68152-132">示例</span><span class="sxs-lookup"><span data-stu-id="68152-132">Example</span></span>
<span data-ttu-id="68152-133">以下示例检索特定的策略。</span><span class="sxs-lookup"><span data-stu-id="68152-133">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="68152-134">请求</span><span class="sxs-lookup"><span data-stu-id="68152-134">Request</span></span>
<span data-ttu-id="68152-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68152-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="68152-136">响应</span><span class="sxs-lookup"><span data-stu-id="68152-136">Response</span></span>
<span data-ttu-id="68152-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68152-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
