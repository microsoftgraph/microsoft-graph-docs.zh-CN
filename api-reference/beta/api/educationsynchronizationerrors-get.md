---
title: 获取 educationSynchronizationErrors
description: '获取验证期间和/或租户中的特定学校数据同步配置文件同步期间生成的错误。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6a15070b68e9cf249a6b6a7841ea24b0e265a24e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926139"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="50734-103">获取 educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="50734-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="50734-104">获取验证期间和/或租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)同步期间生成的错误。</span><span class="sxs-lookup"><span data-stu-id="50734-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="50734-105">权限</span><span class="sxs-lookup"><span data-stu-id="50734-105">Permissions</span></span>
<span data-ttu-id="50734-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50734-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="50734-108">Permission type</span></span> | <span data-ttu-id="50734-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50734-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="50734-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50734-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50734-111">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50734-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="50734-112">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="50734-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="50734-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="50734-113">Not supported.</span></span>|
|<span data-ttu-id="50734-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="50734-114">Application</span></span>| <span data-ttu-id="50734-115">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50734-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50734-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50734-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50734-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50734-117">Optional query parameters</span></span>
<span data-ttu-id="50734-118">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义响应： $filter、 $orderby、 $top、 $skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="50734-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50734-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50734-119">Request headers</span></span>
| <span data-ttu-id="50734-120">名称</span><span class="sxs-lookup"><span data-stu-id="50734-120">Name</span></span>       | <span data-ttu-id="50734-121">类型</span><span class="sxs-lookup"><span data-stu-id="50734-121">Type</span></span> | <span data-ttu-id="50734-122">说明</span><span class="sxs-lookup"><span data-stu-id="50734-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50734-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50734-123">Authorization</span></span>  | <span data-ttu-id="50734-124">string</span><span class="sxs-lookup"><span data-stu-id="50734-124">string</span></span>  | <span data-ttu-id="50734-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50734-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50734-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50734-127">Request body</span></span>
<span data-ttu-id="50734-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50734-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="50734-129">响应</span><span class="sxs-lookup"><span data-stu-id="50734-129">Response</span></span>
<span data-ttu-id="50734-130">如果成功，此方法返回`200 OK`响应代码和[同步错误](../resources/educationsynchronizationerror.md)响应正文中的对象的集合。</span><span class="sxs-lookup"><span data-stu-id="50734-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50734-131">示例</span><span class="sxs-lookup"><span data-stu-id="50734-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50734-132">请求</span><span class="sxs-lookup"><span data-stu-id="50734-132">Request</span></span>
<span data-ttu-id="50734-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="50734-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="50734-134">响应</span><span class="sxs-lookup"><span data-stu-id="50734-134">Response</span></span>
<span data-ttu-id="50734-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="50734-135">The following is an example of the response.</span></span> 

><span data-ttu-id="50734-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="50734-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
