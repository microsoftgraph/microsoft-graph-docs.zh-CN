---
title: 列出课程
description: '检索所有 class 对象的列表。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1d494dd272ef42d7a5d0ade50aec9379c053e79f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324569"
---
# <a name="list-classes"></a><span data-ttu-id="92e57-103">列出课程</span><span class="sxs-lookup"><span data-stu-id="92e57-103">List classes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92e57-104">检索所有 class 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="92e57-104">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="92e57-105">权限</span><span class="sxs-lookup"><span data-stu-id="92e57-105">Permissions</span></span>
<span data-ttu-id="92e57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e57-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92e57-108">Permission type</span></span>      | <span data-ttu-id="92e57-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92e57-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92e57-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92e57-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92e57-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="92e57-111">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="92e57-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92e57-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92e57-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e57-113">Not supported.</span></span>  |
|<span data-ttu-id="92e57-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92e57-114">Application</span></span> | <span data-ttu-id="92e57-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e57-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92e57-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92e57-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92e57-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92e57-117">Optional query parameters</span></span>
<span data-ttu-id="92e57-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92e57-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92e57-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="92e57-119">Request headers</span></span>
| <span data-ttu-id="92e57-120">标头</span><span class="sxs-lookup"><span data-stu-id="92e57-120">Header</span></span>       | <span data-ttu-id="92e57-121">值</span><span class="sxs-lookup"><span data-stu-id="92e57-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92e57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e57-122">Authorization</span></span>  | <span data-ttu-id="92e57-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92e57-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="92e57-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92e57-125">Request body</span></span>
<span data-ttu-id="92e57-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92e57-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="92e57-127">响应</span><span class="sxs-lookup"><span data-stu-id="92e57-127">Response</span></span>
<span data-ttu-id="92e57-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="92e57-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92e57-129">示例</span><span class="sxs-lookup"><span data-stu-id="92e57-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92e57-130">请求</span><span class="sxs-lookup"><span data-stu-id="92e57-130">Request</span></span>
<span data-ttu-id="92e57-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92e57-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes
```
##### <a name="response"></a><span data-ttu-id="92e57-132">响应</span><span class="sxs-lookup"><span data-stu-id="92e57-132">Response</span></span>
<span data-ttu-id="92e57-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92e57-133">The following is an example of the response.</span></span> 

><span data-ttu-id="92e57-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="92e57-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
