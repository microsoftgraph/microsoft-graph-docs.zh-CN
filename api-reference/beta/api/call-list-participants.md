---
title: 参与者列表
description: 检索呼叫中的参与者对象的列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4f4eb95e4aed03dfd9809f8afb0e3f3557717430
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507619"
---
# <a name="list-participants"></a><span data-ttu-id="8d6d3-103">参与者列表</span><span class="sxs-lookup"><span data-stu-id="8d6d3-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d6d3-104">检索呼叫中的参与者对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d6d3-105">权限</span><span class="sxs-lookup"><span data-stu-id="8d6d3-105">Permissions</span></span>
<span data-ttu-id="8d6d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d6d3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d6d3-108">Permission type</span></span> | <span data-ttu-id="8d6d3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d6d3-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8d6d3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6d3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d6d3-111">不支持</span><span class="sxs-lookup"><span data-stu-id="8d6d3-111">Not Supported</span></span>        |
| <span data-ttu-id="8d6d3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d6d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d6d3-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8d6d3-113">Not Supported</span></span>        |
| <span data-ttu-id="8d6d3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d6d3-114">Application</span></span>     | <span data-ttu-id="8d6d3-115">无</span><span class="sxs-lookup"><span data-stu-id="8d6d3-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8d6d3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d6d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d6d3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d6d3-117">Optional query parameters</span></span>
<span data-ttu-id="8d6d3-118">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d6d3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d6d3-119">Request headers</span></span>
| <span data-ttu-id="8d6d3-120">名称</span><span class="sxs-lookup"><span data-stu-id="8d6d3-120">Name</span></span>          | <span data-ttu-id="8d6d3-121">说明</span><span class="sxs-lookup"><span data-stu-id="8d6d3-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8d6d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d6d3-122">Authorization</span></span> | <span data-ttu-id="8d6d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d6d3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d6d3-125">Request body</span></span>
<span data-ttu-id="8d6d3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d6d3-127">响应</span><span class="sxs-lookup"><span data-stu-id="8d6d3-127">Response</span></span>
<span data-ttu-id="8d6d3-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[参与者](../resources/participant.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d6d3-129">示例</span><span class="sxs-lookup"><span data-stu-id="8d6d3-129">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="8d6d3-130">示例 1</span><span class="sxs-lookup"><span data-stu-id="8d6d3-130">Example 1</span></span>

##### <a name="request"></a><span data-ttu-id="8d6d3-131">请求</span><span class="sxs-lookup"><span data-stu-id="8d6d3-131">Request</span></span>
<span data-ttu-id="8d6d3-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants
```

##### <a name="response"></a><span data-ttu-id="8d6d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="8d6d3-133">Response</span></span>

> <span data-ttu-id="8d6d3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d6d3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2"></a><span data-ttu-id="8d6d3-136">示例 2</span><span class="sxs-lookup"><span data-stu-id="8d6d3-136">Example 2</span></span>

##### <a name="request"></a><span data-ttu-id="8d6d3-137">请求</span><span class="sxs-lookup"><span data-stu-id="8d6d3-137">Request</span></span>

```http
GET /app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

##### <a name="response"></a><span data-ttu-id="8d6d3-138">响应</span><span class="sxs-lookup"><span data-stu-id="8d6d3-138">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List participants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-list-participants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
