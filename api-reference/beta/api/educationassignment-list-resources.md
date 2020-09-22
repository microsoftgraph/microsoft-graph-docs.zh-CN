---
title: 列出 educationAssignmentResources
description: 获取与此工作分配相关联的所有资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5d4f54503d18b09691c877ab1a1bb7c5464e05fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007789"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="aa150-103">列出 educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="aa150-103">List educationAssignmentResources</span></span>

<span data-ttu-id="aa150-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa150-105">获取与此工作分配相关联的所有资源。</span><span class="sxs-lookup"><span data-stu-id="aa150-105">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa150-106">权限</span><span class="sxs-lookup"><span data-stu-id="aa150-106">Permissions</span></span>
<span data-ttu-id="aa150-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa150-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa150-109">Permission type</span></span>      | <span data-ttu-id="aa150-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa150-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa150-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa150-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa150-112">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="aa150-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="aa150-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa150-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aa150-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa150-114">Not supported.</span></span>  |
|<span data-ttu-id="aa150-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa150-115">Application</span></span> | <span data-ttu-id="aa150-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa150-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa150-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa150-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa150-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aa150-118">Optional query parameters</span></span>
<span data-ttu-id="aa150-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aa150-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa150-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa150-120">Request headers</span></span>
| <span data-ttu-id="aa150-121">标头</span><span class="sxs-lookup"><span data-stu-id="aa150-121">Header</span></span>       | <span data-ttu-id="aa150-122">值</span><span class="sxs-lookup"><span data-stu-id="aa150-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa150-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa150-123">Authorization</span></span>  | <span data-ttu-id="aa150-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa150-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa150-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa150-126">Request body</span></span>
<span data-ttu-id="aa150-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa150-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="aa150-128">响应</span><span class="sxs-lookup"><span data-stu-id="aa150-128">Response</span></span>
<span data-ttu-id="aa150-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationAssignmentResource](../resources/educationassignmentresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aa150-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa150-130">示例</span><span class="sxs-lookup"><span data-stu-id="aa150-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa150-131">请求</span><span class="sxs-lookup"><span data-stu-id="aa150-131">Request</span></span>
<span data-ttu-id="aa150-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aa150-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="aa150-133">响应</span><span class="sxs-lookup"><span data-stu-id="aa150-133">Response</span></span>
<span data-ttu-id="aa150-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aa150-134">The following is an example of the response.</span></span> 

><span data-ttu-id="aa150-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa150-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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


