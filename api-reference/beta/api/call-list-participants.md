---
title: 参与者列表
description: 检索呼叫中的参与者对象的列表。
author: VinodRavichandran
ms.openlocfilehash: c22e276f7b7bb1ddd0a082bd54f0b5b8d93226c1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380441"
---
# <a name="list-participants"></a><span data-ttu-id="c5e27-103">参与者列表</span><span class="sxs-lookup"><span data-stu-id="c5e27-103">List participants</span></span>

> <span data-ttu-id="c5e27-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5e27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5e27-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5e27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5e27-106">检索呼叫中的参与者对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c5e27-106">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5e27-107">权限</span><span class="sxs-lookup"><span data-stu-id="c5e27-107">Permissions</span></span>
<span data-ttu-id="c5e27-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5e27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5e27-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5e27-110">Permission type</span></span> | <span data-ttu-id="c5e27-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5e27-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="c5e27-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5e27-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5e27-113">不支持</span><span class="sxs-lookup"><span data-stu-id="c5e27-113">Not Supported</span></span>        |
| <span data-ttu-id="c5e27-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5e27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5e27-115">不支持</span><span class="sxs-lookup"><span data-stu-id="c5e27-115">Not Supported</span></span>        |
| <span data-ttu-id="c5e27-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5e27-116">Application</span></span>     | <span data-ttu-id="c5e27-117">无</span><span class="sxs-lookup"><span data-stu-id="c5e27-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="c5e27-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5e27-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5e27-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5e27-119">Optional query parameters</span></span>
<span data-ttu-id="c5e27-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="c5e27-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5e27-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5e27-121">Request headers</span></span>
| <span data-ttu-id="c5e27-122">名称</span><span class="sxs-lookup"><span data-stu-id="c5e27-122">Name</span></span>          | <span data-ttu-id="c5e27-123">说明</span><span class="sxs-lookup"><span data-stu-id="c5e27-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c5e27-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5e27-124">Authorization</span></span> | <span data-ttu-id="c5e27-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5e27-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5e27-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5e27-127">Request body</span></span>
<span data-ttu-id="c5e27-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5e27-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5e27-129">响应</span><span class="sxs-lookup"><span data-stu-id="c5e27-129">Response</span></span>
<span data-ttu-id="c5e27-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[参与者](../resources/participant.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c5e27-130">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5e27-131">示例</span><span class="sxs-lookup"><span data-stu-id="c5e27-131">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="c5e27-132">示例 1</span><span class="sxs-lookup"><span data-stu-id="c5e27-132">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="c5e27-133">请求</span><span class="sxs-lookup"><span data-stu-id="c5e27-133">Request</span></span>
<span data-ttu-id="c5e27-134">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5e27-134">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="c5e27-135">响应</span><span class="sxs-lookup"><span data-stu-id="c5e27-135">Response</span></span>

> <span data-ttu-id="c5e27-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c5e27-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": [
    {
      "id": "id-value",
      "info": {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "languageId": "languageId-value",
        "region": "region-value"
      },
      "isInLobby": false,
      "isMuted": true,
      "mediaStreams": [
        {
          "sourceId": "1",
          "direction": "sendReceive",
          "label": "main-audio",
          "mediaType": "audio",
          "serverMuted": false
        }
      ],
      "metadata": "metadata-value"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="c5e27-138">示例 2</span><span class="sxs-lookup"><span data-stu-id="c5e27-138">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="c5e27-139">请求</span><span class="sxs-lookup"><span data-stu-id="c5e27-139">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="c5e27-140">响应</span><span class="sxs-lookup"><span data-stu-id="c5e27-140">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant",
  "isCollection": true,
  "truncated": true
}-->
```json
{
  "value": [
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "user" : {
            "displayName": "Test User",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "1",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ]
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "phone": {
            "displayName": "+12345678890",
            "id": "+12345678890"
          }
        }
      },
      "mediaStreams": [
        {
          "sourceId": "2",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    },
    {
      "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
      "info": {
        "identity" : {
          "application" : {
            "displayName": "Test BOT",
            "id": "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
          }
        },
        "region": "westus",
        "languageId": "en-US"
      },
      "mediaStreams": [
        {
          "sourceId": "3",
          "mediaType": "audio",
          "label": "main-audio",
          "direction": "sendReceive",
          "serverMuted": false
        }
      ],
      "isMuted": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
