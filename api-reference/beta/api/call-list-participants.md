---
title: 列出参与者
description: 检索呼叫中的参与者对象的列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc38af4a6bee4a380a001310303d67efb2705dcf
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967345"
---
# <a name="list-participants"></a><span data-ttu-id="d5ffa-103">列出参与者</span><span class="sxs-lookup"><span data-stu-id="d5ffa-103">List participants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5ffa-104">检索呼叫中的参与者对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-104">Retrieve a list of participant objects in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5ffa-105">权限</span><span class="sxs-lookup"><span data-stu-id="d5ffa-105">Permissions</span></span>

<span data-ttu-id="d5ffa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5ffa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5ffa-108">Permission type</span></span> | <span data-ttu-id="d5ffa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5ffa-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d5ffa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5ffa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5ffa-111">不支持</span><span class="sxs-lookup"><span data-stu-id="d5ffa-111">Not Supported</span></span>        |
| <span data-ttu-id="d5ffa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5ffa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5ffa-113">不支持</span><span class="sxs-lookup"><span data-stu-id="d5ffa-113">Not Supported</span></span>        |
| <span data-ttu-id="d5ffa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5ffa-114">Application</span></span>     | <span data-ttu-id="d5ffa-115">None</span><span class="sxs-lookup"><span data-stu-id="d5ffa-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="d5ffa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5ffa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /app/calls/{id}/participants
GET /applications/{id}/calls/{id}/participants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5ffa-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="d5ffa-117">Optional query parameters</span></span>

<span data-ttu-id="d5ffa-118">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5ffa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5ffa-119">Request headers</span></span>

| <span data-ttu-id="d5ffa-120">Name</span><span class="sxs-lookup"><span data-stu-id="d5ffa-120">Name</span></span>          | <span data-ttu-id="d5ffa-121">说明</span><span class="sxs-lookup"><span data-stu-id="d5ffa-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d5ffa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5ffa-122">Authorization</span></span> | <span data-ttu-id="d5ffa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5ffa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5ffa-125">Request body</span></span>

<span data-ttu-id="d5ffa-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5ffa-127">响应</span><span class="sxs-lookup"><span data-stu-id="d5ffa-127">Response</span></span>

<span data-ttu-id="d5ffa-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[参与者](../resources/participant.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-128">If successful, this method returns a `200 OK` response code and collection of [participant](../resources/participant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5ffa-129">示例</span><span class="sxs-lookup"><span data-stu-id="d5ffa-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5ffa-130">请求</span><span class="sxs-lookup"><span data-stu-id="d5ffa-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-participants"
}-->

```http
GET https://graph.microsoft.com/beta/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants
Authorization: Bearer <TOKEN>
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="d5ffa-131">响应</span><span class="sxs-lookup"><span data-stu-id="d5ffa-131">Response</span></span>

> <span data-ttu-id="d5ffa-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5ffa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
