---
title: 'cloudCommunications: getPresencesByUserId'
description: 获取多个用户的状态信息。
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 9480e85ad072d368b1afc768a859716865b78f75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982502"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="86d33-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="86d33-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="86d33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86d33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d33-105">获取多个用户的 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="86d33-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="86d33-106">权限</span><span class="sxs-lookup"><span data-stu-id="86d33-106">Permissions</span></span>
<span data-ttu-id="86d33-107">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="86d33-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="86d33-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86d33-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86d33-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86d33-109">Permission type</span></span> | <span data-ttu-id="86d33-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86d33-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="86d33-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86d33-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86d33-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="86d33-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="86d33-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86d33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86d33-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86d33-114">Not Supported.</span></span>                         |
| <span data-ttu-id="86d33-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86d33-115">Application</span></span>                            | <span data-ttu-id="86d33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86d33-116">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="86d33-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86d33-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="86d33-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="86d33-118">Request Headers</span></span>
| <span data-ttu-id="86d33-119">名称</span><span class="sxs-lookup"><span data-stu-id="86d33-119">Name</span></span>          | <span data-ttu-id="86d33-120">说明</span><span class="sxs-lookup"><span data-stu-id="86d33-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="86d33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d33-121">Authorization</span></span> | <span data-ttu-id="86d33-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86d33-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="86d33-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="86d33-124">Content-type</span></span> | <span data-ttu-id="86d33-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="86d33-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="86d33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86d33-127">Request body</span></span>

<span data-ttu-id="86d33-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="86d33-128">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="86d33-129">参数</span><span class="sxs-lookup"><span data-stu-id="86d33-129">Parameter</span></span>      | <span data-ttu-id="86d33-130">类型</span><span class="sxs-lookup"><span data-stu-id="86d33-130">Type</span></span>    |<span data-ttu-id="86d33-131">说明</span><span class="sxs-lookup"><span data-stu-id="86d33-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86d33-132">ids</span><span class="sxs-lookup"><span data-stu-id="86d33-132">ids</span></span>|<span data-ttu-id="86d33-133">String collection</span><span class="sxs-lookup"><span data-stu-id="86d33-133">String collection</span></span>|<span data-ttu-id="86d33-134">用户对象 Id。</span><span class="sxs-lookup"><span data-stu-id="86d33-134">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="86d33-135">响应</span><span class="sxs-lookup"><span data-stu-id="86d33-135">Response</span></span>

<span data-ttu-id="86d33-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="86d33-136">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="86d33-137">示例</span><span class="sxs-lookup"><span data-stu-id="86d33-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86d33-138">请求</span><span class="sxs-lookup"><span data-stu-id="86d33-138">Request</span></span>
<span data-ttu-id="86d33-139">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="86d33-139">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86d33-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="86d33-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
    "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[<span data-ttu-id="86d33-141">C#</span><span class="sxs-lookup"><span data-stu-id="86d33-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86d33-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86d33-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86d33-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86d33-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="86d33-144">响应</span><span class="sxs-lookup"><span data-stu-id="86d33-144">Response</span></span>
<span data-ttu-id="86d33-145">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="86d33-145">The following example shows the response.</span></span>

> <span data-ttu-id="86d33-146">**注意：** 为了提高可读性，响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="86d33-146">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="86d33-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86d33-147">All the properties will be returned from an actual call.</span></span>

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


