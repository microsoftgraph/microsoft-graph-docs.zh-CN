---
title: cloudCommunications：getPresencesByUserId
description: 获取多个用户状态信息。
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 78793623972e5887a1f74184789dbda87ee4dda4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964009"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="2ce09-103">cloudCommunications：getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="2ce09-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="2ce09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ce09-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ce09-105">获取 [多个](../resources/presence.md) 用户状态信息。</span><span class="sxs-lookup"><span data-stu-id="2ce09-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ce09-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ce09-106">Permissions</span></span>
<span data-ttu-id="2ce09-107">调用这些 API 需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="2ce09-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="2ce09-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ce09-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ce09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ce09-109">Permission type</span></span> | <span data-ttu-id="2ce09-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ce09-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="2ce09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ce09-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ce09-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="2ce09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ce09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce09-114">Not Supported.</span></span>                         |
| <span data-ttu-id="2ce09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ce09-115">Application</span></span>                            | <span data-ttu-id="2ce09-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce09-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="2ce09-117">**注意：**</span><span class="sxs-lookup"><span data-stu-id="2ce09-117">**Note:**</span></span>
> * <span data-ttu-id="2ce09-118">每个 API 请求最多支持 650 个用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2ce09-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="2ce09-119">此 API 的最大请求速率是 30 秒内每个租户每个应用程序 1500 个 API 请求。</span><span class="sxs-lookup"><span data-stu-id="2ce09-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="2ce09-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ce09-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="2ce09-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ce09-121">Request Headers</span></span>
| <span data-ttu-id="2ce09-122">名称</span><span class="sxs-lookup"><span data-stu-id="2ce09-122">Name</span></span>          | <span data-ttu-id="2ce09-123">说明</span><span class="sxs-lookup"><span data-stu-id="2ce09-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2ce09-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce09-124">Authorization</span></span> | <span data-ttu-id="2ce09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ce09-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="2ce09-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="2ce09-127">Content-type</span></span> | <span data-ttu-id="2ce09-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2ce09-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="2ce09-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ce09-130">Request body</span></span>

<span data-ttu-id="2ce09-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2ce09-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="2ce09-132">参数</span><span class="sxs-lookup"><span data-stu-id="2ce09-132">Parameter</span></span>      | <span data-ttu-id="2ce09-133">类型</span><span class="sxs-lookup"><span data-stu-id="2ce09-133">Type</span></span>    |<span data-ttu-id="2ce09-134">说明</span><span class="sxs-lookup"><span data-stu-id="2ce09-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce09-135">ids</span><span class="sxs-lookup"><span data-stu-id="2ce09-135">ids</span></span>|<span data-ttu-id="2ce09-136">String collection</span><span class="sxs-lookup"><span data-stu-id="2ce09-136">String collection</span></span>|<span data-ttu-id="2ce09-137">用户对象 ID。</span><span class="sxs-lookup"><span data-stu-id="2ce09-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="2ce09-138">响应</span><span class="sxs-lookup"><span data-stu-id="2ce09-138">Response</span></span>

<span data-ttu-id="2ce09-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [presence](../resources/presence.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ce09-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="2ce09-140">示例</span><span class="sxs-lookup"><span data-stu-id="2ce09-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ce09-141">请求</span><span class="sxs-lookup"><span data-stu-id="2ce09-141">Request</span></span>
<span data-ttu-id="2ce09-142">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="2ce09-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ce09-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ce09-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[<span data-ttu-id="2ce09-144">C#</span><span class="sxs-lookup"><span data-stu-id="2ce09-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ce09-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ce09-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ce09-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ce09-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ce09-147">Java</span><span class="sxs-lookup"><span data-stu-id="2ce09-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="2ce09-148">响应</span><span class="sxs-lookup"><span data-stu-id="2ce09-148">Response</span></span>
<span data-ttu-id="2ce09-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2ce09-149">The following example shows the response.</span></span>

> <span data-ttu-id="2ce09-150">**注意：** 为了可读性，可能会缩短响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ce09-150">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="2ce09-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ce09-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574
```
```json
{
    "value": [{
            "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
            "availability": "Busy",
            "activity": "InAMeeting"
        },
        {
            "id": "66825e03-7ef5-42da-9069-724602c31f6b",
            "availability": "Away",
            "activity": "Away"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


