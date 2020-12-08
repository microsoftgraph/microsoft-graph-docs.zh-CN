---
title: 获取状态
description: 获取用户的状态信息。
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: a82c03e9b63d83f8aab8b3556e75b17d926ff3e6
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581197"
---
# <a name="get-presence"></a><span data-ttu-id="bbc29-103">获取状态</span><span class="sxs-lookup"><span data-stu-id="bbc29-103">Get presence</span></span>

<span data-ttu-id="bbc29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbc29-105">获取用户的 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="bbc29-105">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc29-106">权限</span><span class="sxs-lookup"><span data-stu-id="bbc29-106">Permissions</span></span>
<span data-ttu-id="bbc29-107">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="bbc29-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="bbc29-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbc29-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbc29-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbc29-109">Permission type</span></span> | <span data-ttu-id="bbc29-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbc29-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="bbc29-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc29-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbc29-112">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="bbc29-112">Presence.Read, Presence.Read.All</span></span>      |
| <span data-ttu-id="bbc29-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc29-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbc29-114">Not Supported.</span></span>                        |
| <span data-ttu-id="bbc29-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbc29-115">Application</span></span>                            | <span data-ttu-id="bbc29-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbc29-116">Not Supported.</span></span>                        |

> <span data-ttu-id="bbc29-117">**注意：** 此 API 的最大请求速率为每个租户在30秒内的每个应用程序的 1500 API 请求数。</span><span class="sxs-lookup"><span data-stu-id="bbc29-117">**Note:** The maximum request rate for this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-requests"></a><span data-ttu-id="bbc29-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbc29-118">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
GET /communications/presences
```

## <a name="request-headers"></a><span data-ttu-id="bbc29-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbc29-119">Request Headers</span></span>
| <span data-ttu-id="bbc29-120">名称</span><span class="sxs-lookup"><span data-stu-id="bbc29-120">Name</span></span>          | <span data-ttu-id="bbc29-121">说明</span><span class="sxs-lookup"><span data-stu-id="bbc29-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bbc29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbc29-122">Authorization</span></span> | <span data-ttu-id="bbc29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbc29-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bbc29-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbc29-125">Request body</span></span>

<span data-ttu-id="bbc29-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbc29-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbc29-127">响应</span><span class="sxs-lookup"><span data-stu-id="bbc29-127">Response</span></span>
<span data-ttu-id="bbc29-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbc29-128">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbc29-129">示例</span><span class="sxs-lookup"><span data-stu-id="bbc29-129">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="bbc29-130">示例1：获取自己的状态信息</span><span class="sxs-lookup"><span data-stu-id="bbc29-130">Example 1: Get your own presence information</span></span>

<span data-ttu-id="bbc29-131">下面的示例展示了如何获取自己的状态信息。</span><span class="sxs-lookup"><span data-stu-id="bbc29-131">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="bbc29-132">此操作需要状态为 "读取" 权限。</span><span class="sxs-lookup"><span data-stu-id="bbc29-132">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc29-133">请求</span><span class="sxs-lookup"><span data-stu-id="bbc29-133">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/presence
```

---


#### <a name="response"></a><span data-ttu-id="bbc29-134">响应</span><span class="sxs-lookup"><span data-stu-id="bbc29-134">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="bbc29-135">示例2：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="bbc29-135">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="bbc29-136">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="bbc29-136">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="bbc29-137">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="bbc29-137">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc29-138">请求</span><span class="sxs-lookup"><span data-stu-id="bbc29-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

---


#### <a name="response"></a><span data-ttu-id="bbc29-139">响应</span><span class="sxs-lookup"><span data-stu-id="bbc29-139">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

### <a name="example-3-get-the-presence-information-of-another-user"></a><span data-ttu-id="bbc29-140">示例3：获取其他用户的状态信息</span><span class="sxs-lookup"><span data-stu-id="bbc29-140">Example 3: Get the presence information of another user</span></span>

<span data-ttu-id="bbc29-141">下面的示例展示了如何获取其他用户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="bbc29-141">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="bbc29-142">此操作需要已读。 All 权限。</span><span class="sxs-lookup"><span data-stu-id="bbc29-142">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="bbc29-143">请求</span><span class="sxs-lookup"><span data-stu-id="bbc29-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-user-presences"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647
```

---


#### <a name="response"></a><span data-ttu-id="bbc29-144">响应</span><span class="sxs-lookup"><span data-stu-id="bbc29-144">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presences",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK

{
    "value": [
        {
            "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
            "availability": "Away",
            "activity": "BeRightBack"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


