---
title: 列表 educationAssignmentResources
description: 获取与此工作分配关联的所有资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0fa0a5b46d7f40b1d1e8b6d265b12f84384e2c50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936198"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="9b4a9-103">列表 educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="9b4a9-103">List educationAssignmentResources</span></span>

> <span data-ttu-id="9b4a9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4a9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b4a9-106">获取与此工作分配关联的所有资源。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-106">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b4a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="9b4a9-107">Permissions</span></span>
<span data-ttu-id="9b4a9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b4a9-110">Permission type</span></span>      | <span data-ttu-id="9b4a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b4a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b4a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b4a9-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9b4a9-113">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b4a9-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9b4a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b4a9-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9b4a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-115">Not supported.</span></span>  |
|<span data-ttu-id="9b4a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b4a9-116">Application</span></span> | <span data-ttu-id="9b4a9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9b4a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b4a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b4a9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b4a9-119">Optional query parameters</span></span>
<span data-ttu-id="9b4a9-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b4a9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b4a9-121">Request headers</span></span>
| <span data-ttu-id="9b4a9-122">标头</span><span class="sxs-lookup"><span data-stu-id="9b4a9-122">Header</span></span>       | <span data-ttu-id="9b4a9-123">值</span><span class="sxs-lookup"><span data-stu-id="9b4a9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b4a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b4a9-124">Authorization</span></span>  | <span data-ttu-id="9b4a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b4a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b4a9-127">Request body</span></span>
<span data-ttu-id="9b4a9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9b4a9-129">响应</span><span class="sxs-lookup"><span data-stu-id="9b4a9-129">Response</span></span>
<span data-ttu-id="9b4a9-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationAssignmentResource](../resources/educationassignmentresource.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b4a9-131">示例</span><span class="sxs-lookup"><span data-stu-id="9b4a9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b4a9-132">请求</span><span class="sxs-lookup"><span data-stu-id="9b4a9-132">Request</span></span>
<span data-ttu-id="9b4a9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="9b4a9-134">响应</span><span class="sxs-lookup"><span data-stu-id="9b4a9-134">Response</span></span>
<span data-ttu-id="9b4a9-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9b4a9-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b4a9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
