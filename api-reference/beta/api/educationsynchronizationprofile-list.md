---
title: 列表 educationSynchronizationProfiles
description: 检索为租户中的学校数据同步配置文件的集合。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9b234ac8a6a99f5cc32a3f4416975ea77f4c66ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853667"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="56c9d-103">列表 educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="56c9d-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="56c9d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="56c9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56c9d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56c9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56c9d-106">检索为租户中的学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="56c9d-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="56c9d-107">权限</span><span class="sxs-lookup"><span data-stu-id="56c9d-107">Permissions</span></span>
<span data-ttu-id="56c9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56c9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56c9d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="56c9d-110">Permission type</span></span> | <span data-ttu-id="56c9d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56c9d-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="56c9d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56c9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56c9d-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56c9d-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="56c9d-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="56c9d-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="56c9d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56c9d-115">Not supported.</span></span>|
|<span data-ttu-id="56c9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="56c9d-116">Application</span></span>|<span data-ttu-id="56c9d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="56c9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56c9d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56c9d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56c9d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56c9d-119">Optional query parameters</span></span>
<span data-ttu-id="56c9d-120">此方法支持以下[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义响应： $filter、 $orderby、 $top、 $skip 和 $count。</span><span class="sxs-lookup"><span data-stu-id="56c9d-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56c9d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="56c9d-121">Request headers</span></span>
| <span data-ttu-id="56c9d-122">名称</span><span class="sxs-lookup"><span data-stu-id="56c9d-122">Name</span></span>       | <span data-ttu-id="56c9d-123">类型</span><span class="sxs-lookup"><span data-stu-id="56c9d-123">Type</span></span> | <span data-ttu-id="56c9d-124">说明</span><span class="sxs-lookup"><span data-stu-id="56c9d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56c9d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56c9d-125">Authorization</span></span>  | <span data-ttu-id="56c9d-126">string</span><span class="sxs-lookup"><span data-stu-id="56c9d-126">string</span></span>  | <span data-ttu-id="56c9d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56c9d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56c9d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="56c9d-129">Request body</span></span>
<span data-ttu-id="56c9d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56c9d-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56c9d-131">响应</span><span class="sxs-lookup"><span data-stu-id="56c9d-131">Response</span></span>
<span data-ttu-id="56c9d-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="56c9d-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56c9d-133">示例</span><span class="sxs-lookup"><span data-stu-id="56c9d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56c9d-134">请求</span><span class="sxs-lookup"><span data-stu-id="56c9d-134">Request</span></span>
<span data-ttu-id="56c9d-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56c9d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="56c9d-136">响应</span><span class="sxs-lookup"><span data-stu-id="56c9d-136">Response</span></span>
<span data-ttu-id="56c9d-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56c9d-137">The following is an example of the response.</span></span> 

><span data-ttu-id="56c9d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="56c9d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "#microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "studentEnrollment": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacherRoster": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                }
            }
        },
        "identitySynchronizationConfiguration": {
            "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
            "userDomains": [
                {
                    "appliesTo": "student",
                    "name": "testschool.edu"
                },
                {
                    "appliesTo": "teacher",
                    "name": "testschool.edu"
                }
            ]
        },
        "licensesToAssign": [
            {
                "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
    }
  ]
}
```
