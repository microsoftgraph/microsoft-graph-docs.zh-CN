---
title: 列表策略
description: 检索目录中的所有策略对象。
localization_priority: Normal
ms.openlocfilehash: ea97146b646068515ab6fdc7fab4b3cefb16031e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836054"
---
# <a name="list-policies"></a><span data-ttu-id="67129-103">列表策略</span><span class="sxs-lookup"><span data-stu-id="67129-103">List Policies</span></span>

> <span data-ttu-id="67129-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="67129-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67129-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67129-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67129-106">检索目录中的所有[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67129-106">Retrieve all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="67129-107">权限</span><span class="sxs-lookup"><span data-stu-id="67129-107">Permissions</span></span>
<span data-ttu-id="67129-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67129-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67129-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67129-110">Permission type</span></span>      | <span data-ttu-id="67129-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67129-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67129-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67129-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67129-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67129-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67129-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67129-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67129-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67129-115">Not supported.</span></span>    |
|<span data-ttu-id="67129-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67129-116">Application</span></span> | <span data-ttu-id="67129-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="67129-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67129-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67129-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="67129-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="67129-119">Request headers</span></span>
| <span data-ttu-id="67129-120">名称</span><span class="sxs-lookup"><span data-stu-id="67129-120">Name</span></span>       | <span data-ttu-id="67129-121">类型</span><span class="sxs-lookup"><span data-stu-id="67129-121">Type</span></span> | <span data-ttu-id="67129-122">说明</span><span class="sxs-lookup"><span data-stu-id="67129-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67129-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67129-123">Authorization</span></span>  | <span data-ttu-id="67129-124">string</span><span class="sxs-lookup"><span data-stu-id="67129-124">string</span></span>  | <span data-ttu-id="67129-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67129-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67129-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="67129-127">Request body</span></span>
<span data-ttu-id="67129-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67129-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67129-129">响应</span><span class="sxs-lookup"><span data-stu-id="67129-129">Response</span></span>

<span data-ttu-id="67129-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[策略](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67129-130">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="67129-131">如果不成功...</span><span class="sxs-lookup"><span data-stu-id="67129-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="67129-132">示例</span><span class="sxs-lookup"><span data-stu-id="67129-132">Example</span></span>
<span data-ttu-id="67129-133">以下示例检索所有策略。</span><span class="sxs-lookup"><span data-stu-id="67129-133">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="67129-134">请求</span><span class="sxs-lookup"><span data-stu-id="67129-134">Request</span></span>
<span data-ttu-id="67129-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67129-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="67129-136">响应</span><span class="sxs-lookup"><span data-stu-id="67129-136">Response</span></span>
<span data-ttu-id="67129-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67129-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "value":[
        {
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
