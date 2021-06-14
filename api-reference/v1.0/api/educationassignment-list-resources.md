---
title: 列出作业资源
description: 获取与此工作分配关联的所有资源。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6d9363bb6127bde54cd7e56eae382fae621185d7
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912291"
---
# <a name="list-assignment-resources"></a><span data-ttu-id="4891c-103">列出作业资源</span><span class="sxs-lookup"><span data-stu-id="4891c-103">List assignment resources</span></span>

<span data-ttu-id="4891c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4891c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4891c-105">获取与工作分配 关联的所有 [资源](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4891c-105">Get all the resources associated with an [assignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4891c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4891c-106">Permissions</span></span>
<span data-ttu-id="4891c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4891c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4891c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4891c-109">Permission type</span></span>      | <span data-ttu-id="4891c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4891c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4891c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4891c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4891c-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4891c-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4891c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4891c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4891c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4891c-114">Not supported.</span></span>  |
|<span data-ttu-id="4891c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4891c-115">Application</span></span> | <span data-ttu-id="4891c-116">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4891c-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4891c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4891c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4891c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4891c-118">Optional query parameters</span></span>
<span data-ttu-id="4891c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4891c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4891c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4891c-120">Request headers</span></span>
| <span data-ttu-id="4891c-121">标头</span><span class="sxs-lookup"><span data-stu-id="4891c-121">Header</span></span>       | <span data-ttu-id="4891c-122">值</span><span class="sxs-lookup"><span data-stu-id="4891c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4891c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4891c-123">Authorization</span></span>  | <span data-ttu-id="4891c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4891c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4891c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4891c-126">Request body</span></span>
<span data-ttu-id="4891c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4891c-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4891c-128">响应</span><span class="sxs-lookup"><span data-stu-id="4891c-128">Response</span></span>
<span data-ttu-id="4891c-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4891c-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4891c-130">示例</span><span class="sxs-lookup"><span data-stu-id="4891c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4891c-131">请求</span><span class="sxs-lookup"><span data-stu-id="4891c-131">Request</span></span>
<span data-ttu-id="4891c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4891c-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
```

### <a name="response"></a><span data-ttu-id="4891c-133">响应</span><span class="sxs-lookup"><span data-stu-id="4891c-133">Response</span></span>
<span data-ttu-id="4891c-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4891c-134">The following is an example of the response.</span></span> 

><span data-ttu-id="4891c-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4891c-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
      "resource": {
          "@odata.type": "#microsoft.graph.educationWordResource",
          "displayName": "Report.docx",
          "createdDateTime": "2017-10-21T07:52:53.9863696Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
