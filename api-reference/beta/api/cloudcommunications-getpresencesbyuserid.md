---
title: 'cloudCommunications: getPresencesByUserId'
description: 获取多个用户的状态信息。
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 93a782a0d46125a1f4a4a751c45d254e293c05cb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868096"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="b1e20-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="b1e20-103">cloudCommunications: getPresencesByUserId</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e20-104">获取多个用户的[状态](../resources/presence.md)信息。</span><span class="sxs-lookup"><span data-stu-id="b1e20-104">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e20-105">权限</span><span class="sxs-lookup"><span data-stu-id="b1e20-105">Permissions</span></span>
<span data-ttu-id="b1e20-106">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="b1e20-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="b1e20-107">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1e20-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1e20-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1e20-108">Permission type</span></span> | <span data-ttu-id="b1e20-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1e20-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b1e20-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1e20-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1e20-111">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1e20-111">Presence.Read.All</span></span>                         |
| <span data-ttu-id="b1e20-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1e20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1e20-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1e20-113">Not Supported.</span></span>                         |
| <span data-ttu-id="b1e20-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1e20-114">Application</span></span>                            | <span data-ttu-id="b1e20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1e20-115">Not Supported.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="b1e20-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1e20-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="b1e20-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1e20-117">Request Headers</span></span>
| <span data-ttu-id="b1e20-118">名称</span><span class="sxs-lookup"><span data-stu-id="b1e20-118">Name</span></span>          | <span data-ttu-id="b1e20-119">说明</span><span class="sxs-lookup"><span data-stu-id="b1e20-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b1e20-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1e20-120">Authorization</span></span> | <span data-ttu-id="b1e20-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1e20-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b1e20-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="b1e20-123">Content-type</span></span> | <span data-ttu-id="b1e20-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b1e20-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b1e20-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1e20-126">Request body</span></span>

<span data-ttu-id="b1e20-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b1e20-127">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="b1e20-128">参数</span><span class="sxs-lookup"><span data-stu-id="b1e20-128">Parameter</span></span>      | <span data-ttu-id="b1e20-129">类型</span><span class="sxs-lookup"><span data-stu-id="b1e20-129">Type</span></span>    |<span data-ttu-id="b1e20-130">说明</span><span class="sxs-lookup"><span data-stu-id="b1e20-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1e20-131">ids</span><span class="sxs-lookup"><span data-stu-id="b1e20-131">ids</span></span>|<span data-ttu-id="b1e20-132">String collection</span><span class="sxs-lookup"><span data-stu-id="b1e20-132">String collection</span></span>|<span data-ttu-id="b1e20-133">用户对象 Id。</span><span class="sxs-lookup"><span data-stu-id="b1e20-133">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="b1e20-134">响应</span><span class="sxs-lookup"><span data-stu-id="b1e20-134">Response</span></span>

<span data-ttu-id="b1e20-135">如果成功，此方法在响应`200 OK`正文中返回响应代码和[状态](../resources/presence.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b1e20-135">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="b1e20-136">示例</span><span class="sxs-lookup"><span data-stu-id="b1e20-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1e20-137">请求</span><span class="sxs-lookup"><span data-stu-id="b1e20-137">Request</span></span>
<span data-ttu-id="b1e20-138">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="b1e20-138">The following example shows a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1e20-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e20-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1e20-140">C#</span><span class="sxs-lookup"><span data-stu-id="b1e20-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1e20-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1e20-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1e20-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1e20-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b1e20-143">响应</span><span class="sxs-lookup"><span data-stu-id="b1e20-143">Response</span></span>
<span data-ttu-id="b1e20-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="b1e20-144">The following example shows the response.</span></span>

> <span data-ttu-id="b1e20-145">**注意：** 为了提高可读性，响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="b1e20-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="b1e20-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b1e20-146">All the properties will be returned from an actual call.</span></span>

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
