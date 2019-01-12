---
title: 列出 educationClasses
description: 检索学校所拥有的课程列表。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 40b86e4f392179ffb0c98ec0284d4d7c017dd930
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990451"
---
# <a name="list-educationclasses"></a><span data-ttu-id="5c2e2-103">列出 educationClasses</span><span class="sxs-lookup"><span data-stu-id="5c2e2-103">List educationClasses</span></span>

> <span data-ttu-id="5c2e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c2e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c2e2-106">检索学校所拥有的课程列表。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-106">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c2e2-107">权限</span><span class="sxs-lookup"><span data-stu-id="5c2e2-107">Permissions</span></span>
<span data-ttu-id="5c2e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c2e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c2e2-110">Permission type</span></span>      | <span data-ttu-id="5c2e2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c2e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c2e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c2e2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5c2e2-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5c2e2-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="5c2e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c2e2-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5c2e2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-115">Not supported.</span></span>  |
|<span data-ttu-id="5c2e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c2e2-116">Application</span></span> | <span data-ttu-id="5c2e2-117">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c2e2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5c2e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c2e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c2e2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c2e2-119">Optional query parameters</span></span>
<span data-ttu-id="5c2e2-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c2e2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c2e2-121">Request headers</span></span>
| <span data-ttu-id="5c2e2-122">标头</span><span class="sxs-lookup"><span data-stu-id="5c2e2-122">Header</span></span>       | <span data-ttu-id="5c2e2-123">值</span><span class="sxs-lookup"><span data-stu-id="5c2e2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c2e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c2e2-124">Authorization</span></span>  | <span data-ttu-id="5c2e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c2e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c2e2-127">Request body</span></span>
<span data-ttu-id="5c2e2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5c2e2-129">响应</span><span class="sxs-lookup"><span data-stu-id="5c2e2-129">Response</span></span>
<span data-ttu-id="5c2e2-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c2e2-131">示例</span><span class="sxs-lookup"><span data-stu-id="5c2e2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c2e2-132">请求</span><span class="sxs-lookup"><span data-stu-id="5c2e2-132">Request</span></span>
<span data-ttu-id="5c2e2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/classes
```
##### <a name="response"></a><span data-ttu-id="5c2e2-134">响应</span><span class="sxs-lookup"><span data-stu-id="5c2e2-134">Response</span></span>
<span data-ttu-id="5c2e2-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5c2e2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5c2e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
