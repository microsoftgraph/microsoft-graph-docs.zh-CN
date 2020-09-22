---
title: 参与者： muteAll
description: 将呼叫中的所有参与者设为静音。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0842ebbf4710c964a1ee35e3d63b0f8a0311cb90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040339"
---
# <a name="participant-muteall"></a><span data-ttu-id="f6846-103">参与者： muteAll</span><span class="sxs-lookup"><span data-stu-id="f6846-103">participant: muteAll</span></span>

<span data-ttu-id="f6846-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6846-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6846-105">将呼叫中的所有参与者设为静音。</span><span class="sxs-lookup"><span data-stu-id="f6846-105">Mute all participants in the call.</span></span>

> <span data-ttu-id="f6846-106">**注意：** 此 API 已弃用，将在2020年3月15日之前删除。</span><span class="sxs-lookup"><span data-stu-id="f6846-106">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="f6846-107">若要使单个参与者静音，请参阅 [参与者：静音](participant-mute.md)。</span><span class="sxs-lookup"><span data-stu-id="f6846-107">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f6846-108">权限</span><span class="sxs-lookup"><span data-stu-id="f6846-108">Permissions</span></span>
<span data-ttu-id="f6846-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6846-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6846-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6846-111">Permission type</span></span>                        | <span data-ttu-id="f6846-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6846-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f6846-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6846-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6846-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f6846-114">Not Supported</span></span>                               |
| <span data-ttu-id="f6846-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6846-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6846-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f6846-116">Not Supported</span></span>                               |
| <span data-ttu-id="f6846-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6846-117">Application</span></span>                            | <span data-ttu-id="f6846-118">无</span><span class="sxs-lookup"><span data-stu-id="f6846-118">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f6846-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6846-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="f6846-120">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="f6846-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f6846-121">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="f6846-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6846-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6846-122">Request headers</span></span>
| <span data-ttu-id="f6846-123">名称</span><span class="sxs-lookup"><span data-stu-id="f6846-123">Name</span></span>          | <span data-ttu-id="f6846-124">说明</span><span class="sxs-lookup"><span data-stu-id="f6846-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f6846-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6846-125">Authorization</span></span> | <span data-ttu-id="f6846-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6846-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6846-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="f6846-128">Content-type</span></span> | <span data-ttu-id="f6846-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f6846-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6846-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6846-131">Request body</span></span>
<span data-ttu-id="f6846-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f6846-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6846-133">参数</span><span class="sxs-lookup"><span data-stu-id="f6846-133">Parameter</span></span>      | <span data-ttu-id="f6846-134">类型</span><span class="sxs-lookup"><span data-stu-id="f6846-134">Type</span></span>    |<span data-ttu-id="f6846-135">说明</span><span class="sxs-lookup"><span data-stu-id="f6846-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6846-136">participants</span><span class="sxs-lookup"><span data-stu-id="f6846-136">participants</span></span>|<span data-ttu-id="f6846-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="f6846-137">String collection</span></span>|<span data-ttu-id="f6846-138">要静音的参与者。</span><span class="sxs-lookup"><span data-stu-id="f6846-138">The participants to be muted.</span></span>|
|<span data-ttu-id="f6846-139">适用</span><span class="sxs-lookup"><span data-stu-id="f6846-139">clientContext</span></span>|<span data-ttu-id="f6846-140">String</span><span class="sxs-lookup"><span data-stu-id="f6846-140">String</span></span>|<span data-ttu-id="f6846-141">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="f6846-141">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f6846-142">响应</span><span class="sxs-lookup"><span data-stu-id="f6846-142">Response</span></span>
<span data-ttu-id="f6846-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [commsOperation](../resources/commsoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6846-143">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6846-144">示例</span><span class="sxs-lookup"><span data-stu-id="f6846-144">Example</span></span>
<span data-ttu-id="f6846-145">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f6846-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f6846-146">请求</span><span class="sxs-lookup"><span data-stu-id="f6846-146">Request</span></span>
<span data-ttu-id="f6846-147">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6846-147">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6846-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6846-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="f6846-149">C#</span><span class="sxs-lookup"><span data-stu-id="f6846-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6846-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6846-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6846-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6846-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6846-152">响应</span><span class="sxs-lookup"><span data-stu-id="f6846-152">Response</span></span>

> <span data-ttu-id="f6846-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6846-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-muteAll",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


