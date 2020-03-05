---
title: 列表策略
description: 获取目录中的所有 policy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 0f3119d79ed7c9dfa37453aa90bf0b95eecb901b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455506"
---
# <a name="list-policies"></a><span data-ttu-id="5b4da-103">列表策略</span><span class="sxs-lookup"><span data-stu-id="5b4da-103">List Policies</span></span>

<span data-ttu-id="5b4da-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5b4da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b4da-105">获取目录中的所有[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b4da-105">Get all [policy](../resources/policy.md) objects in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4da-106">权限</span><span class="sxs-lookup"><span data-stu-id="5b4da-106">Permissions</span></span>
<span data-ttu-id="5b4da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b4da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b4da-109">Permission type</span></span>      | <span data-ttu-id="5b4da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b4da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b4da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b4da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5b4da-112">Policy： All、Directory.accessasuser.all、All、All</span><span class="sxs-lookup"><span data-stu-id="5b4da-112">Policy.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b4da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b4da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b4da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b4da-114">Not supported.</span></span>    |
|<span data-ttu-id="5b4da-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b4da-115">Application</span></span> | <span data-ttu-id="5b4da-116">Read. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="5b4da-116">Policy.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b4da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b4da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies
```
## <a name="request-headers"></a><span data-ttu-id="5b4da-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b4da-118">Request headers</span></span>
| <span data-ttu-id="5b4da-119">名称</span><span class="sxs-lookup"><span data-stu-id="5b4da-119">Name</span></span>       | <span data-ttu-id="5b4da-120">类型</span><span class="sxs-lookup"><span data-stu-id="5b4da-120">Type</span></span> | <span data-ttu-id="5b4da-121">说明</span><span class="sxs-lookup"><span data-stu-id="5b4da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b4da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b4da-122">Authorization</span></span>  | <span data-ttu-id="5b4da-123">string</span><span class="sxs-lookup"><span data-stu-id="5b4da-123">string</span></span>  | <span data-ttu-id="5b4da-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b4da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b4da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b4da-126">Request body</span></span>
<span data-ttu-id="5b4da-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b4da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4da-128">响应</span><span class="sxs-lookup"><span data-stu-id="5b4da-128">Response</span></span>

<span data-ttu-id="5b4da-129">如果成功，此方法在`200 OK`响应正文中返回响应代码和[policy](../resources/policy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b4da-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="5b4da-130">如果不成功 .。。</span><span class="sxs-lookup"><span data-stu-id="5b4da-130">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="5b4da-131">示例</span><span class="sxs-lookup"><span data-stu-id="5b4da-131">Example</span></span>
<span data-ttu-id="5b4da-132">下面的示例检索所有策略。</span><span class="sxs-lookup"><span data-stu-id="5b4da-132">The following example retrieves all policies.</span></span>

##### <a name="request"></a><span data-ttu-id="5b4da-133">请求</span><span class="sxs-lookup"><span data-stu-id="5b4da-133">Request</span></span>
<span data-ttu-id="5b4da-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b4da-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies
```

##### <a name="response"></a><span data-ttu-id="5b4da-135">响应</span><span class="sxs-lookup"><span data-stu-id="5b4da-135">Response</span></span>
<span data-ttu-id="5b4da-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b4da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
