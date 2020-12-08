---
title: 'cloudCommunications: getPresencesByUserId'
description: 获取多个用户的状态信息。
author: elvinyang-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: e06c1403b1d96a42a670f4c6d53c3bf5251d3b8a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581190"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a><span data-ttu-id="f5fc8-103">cloudCommunications: getPresencesByUserId</span><span class="sxs-lookup"><span data-stu-id="f5fc8-103">cloudCommunications: getPresencesByUserId</span></span>

<span data-ttu-id="f5fc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5fc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5fc8-105">获取多个用户的 [状态](../resources/presence.md) 信息。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-105">Get the [presence](../resources/presence.md) information for multiple users.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5fc8-106">权限</span><span class="sxs-lookup"><span data-stu-id="f5fc8-106">Permissions</span></span>
<span data-ttu-id="f5fc8-107">若要调用这些 Api，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-107">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="f5fc8-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5fc8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5fc8-109">Permission type</span></span> | <span data-ttu-id="f5fc8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5fc8-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f5fc8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5fc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5fc8-112">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5fc8-112">Presence.Read.All</span></span>                         |
| <span data-ttu-id="f5fc8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5fc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5fc8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-114">Not Supported.</span></span>                         |
| <span data-ttu-id="f5fc8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5fc8-115">Application</span></span>                            | <span data-ttu-id="f5fc8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-116">Not Supported.</span></span>                                  |

> <span data-ttu-id="f5fc8-117">**注意：**</span><span class="sxs-lookup"><span data-stu-id="f5fc8-117">**Note:**</span></span>
> * <span data-ttu-id="f5fc8-118">每个 API 请求最多支持650个用户 Id。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-118">Maximum of 650 user IDs are supported per API request.</span></span>
> * <span data-ttu-id="f5fc8-119">此 API 的最大请求速率为每个租户在30秒内的每个应用程序的 1500 API 请求数。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-119">The maximum request rate of this API is 1500 API requests in a 30 second period, per application per tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f5fc8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5fc8-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a><span data-ttu-id="f5fc8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5fc8-121">Request Headers</span></span>
| <span data-ttu-id="f5fc8-122">名称</span><span class="sxs-lookup"><span data-stu-id="f5fc8-122">Name</span></span>          | <span data-ttu-id="f5fc8-123">说明</span><span class="sxs-lookup"><span data-stu-id="f5fc8-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f5fc8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5fc8-124">Authorization</span></span> | <span data-ttu-id="f5fc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f5fc8-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="f5fc8-127">Content-type</span></span> | <span data-ttu-id="f5fc8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f5fc8-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f5fc8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5fc8-130">Request body</span></span>

<span data-ttu-id="f5fc8-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-131">In the request body, provide a JSON object with the following parameter.</span></span>

| <span data-ttu-id="f5fc8-132">参数</span><span class="sxs-lookup"><span data-stu-id="f5fc8-132">Parameter</span></span>      | <span data-ttu-id="f5fc8-133">类型</span><span class="sxs-lookup"><span data-stu-id="f5fc8-133">Type</span></span>    |<span data-ttu-id="f5fc8-134">说明</span><span class="sxs-lookup"><span data-stu-id="f5fc8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5fc8-135">ids</span><span class="sxs-lookup"><span data-stu-id="f5fc8-135">ids</span></span>|<span data-ttu-id="f5fc8-136">String collection</span><span class="sxs-lookup"><span data-stu-id="f5fc8-136">String collection</span></span>|<span data-ttu-id="f5fc8-137">用户对象 Id。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-137">The user object IDs.</span></span>|

## <a name="response"></a><span data-ttu-id="f5fc8-138">响应</span><span class="sxs-lookup"><span data-stu-id="f5fc8-138">Response</span></span>

<span data-ttu-id="f5fc8-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [状态](../resources/presence.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-139">If successful, this method returns a `200 OK` response code and a collection of [presence](../resources/presence.md) objects in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="f5fc8-140">示例</span><span class="sxs-lookup"><span data-stu-id="f5fc8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5fc8-141">请求</span><span class="sxs-lookup"><span data-stu-id="f5fc8-141">Request</span></span>
<span data-ttu-id="f5fc8-142">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-142">The following example shows a request.</span></span>

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

---

### <a name="response"></a><span data-ttu-id="f5fc8-143">响应</span><span class="sxs-lookup"><span data-stu-id="f5fc8-143">Response</span></span>
<span data-ttu-id="f5fc8-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-144">The following example shows the response.</span></span>

> <span data-ttu-id="f5fc8-145">**注意：** 为了提高可读性，响应对象可能会缩短。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-145">**Note:** The response objects might be shortened for readability.</span></span> <span data-ttu-id="f5fc8-146">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f5fc8-146">All the properties will be returned from an actual call.</span></span>

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


