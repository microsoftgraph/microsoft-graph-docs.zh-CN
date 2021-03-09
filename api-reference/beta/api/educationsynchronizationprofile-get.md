---
title: 获取 educationSynchronizationProfile
description: 根据标识符检索租户中的学校数据同步配置文件。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f6a8dd354a93ec2a99c739585c4562e17552bb47
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574242"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="808fb-103">获取 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="808fb-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="808fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="808fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="808fb-105">根据 [标识符检索租户](../resources/educationsynchronizationprofile.md) 中的学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="808fb-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="808fb-106">权限</span><span class="sxs-lookup"><span data-stu-id="808fb-106">Permissions</span></span>
<span data-ttu-id="808fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="808fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="808fb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="808fb-109">Permission type</span></span> | <span data-ttu-id="808fb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="808fb-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="808fb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="808fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="808fb-112">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="808fb-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="808fb-113">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="808fb-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="808fb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="808fb-114">Not supported.</span></span>|
|<span data-ttu-id="808fb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="808fb-115">Application</span></span>| <span data-ttu-id="808fb-116">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="808fb-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="808fb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="808fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="808fb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="808fb-118">Request headers</span></span>
| <span data-ttu-id="808fb-119">名称</span><span class="sxs-lookup"><span data-stu-id="808fb-119">Name</span></span>       | <span data-ttu-id="808fb-120">类型</span><span class="sxs-lookup"><span data-stu-id="808fb-120">Type</span></span> | <span data-ttu-id="808fb-121">说明</span><span class="sxs-lookup"><span data-stu-id="808fb-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="808fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="808fb-122">Authorization</span></span>  | <span data-ttu-id="808fb-123">string</span><span class="sxs-lookup"><span data-stu-id="808fb-123">string</span></span>  | <span data-ttu-id="808fb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="808fb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="808fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="808fb-126">Request body</span></span>
<span data-ttu-id="808fb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="808fb-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="808fb-128">响应</span><span class="sxs-lookup"><span data-stu-id="808fb-128">Response</span></span>
<span data-ttu-id="808fb-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="808fb-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="808fb-130">示例</span><span class="sxs-lookup"><span data-stu-id="808fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="808fb-131">请求</span><span class="sxs-lookup"><span data-stu-id="808fb-131">Request</span></span>
<span data-ttu-id="808fb-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="808fb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="808fb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="808fb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="808fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="808fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="808fb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="808fb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="808fb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="808fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="808fb-137">Java</span><span class="sxs-lookup"><span data-stu-id="808fb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="808fb-138">响应</span><span class="sxs-lookup"><span data-stu-id="808fb-138">Response</span></span>
<span data-ttu-id="808fb-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="808fb-139">The following is an example of the response.</span></span> 

><span data-ttu-id="808fb-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="808fb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
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
        "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
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
    "licensesToAssign": 
         [
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
}
```


