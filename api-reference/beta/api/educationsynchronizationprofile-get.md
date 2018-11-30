---
title: 获取 educationSynchronizationProfile
description: 检索学校数据同步配置文件中租户基于的标识符。
ms.openlocfilehash: a62b938f3177f06a02a8a5ad1190d72b3f27dfd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041346"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="5cd12-103">获取 educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="5cd12-103">Get an educationSynchronizationProfile</span></span>

> <span data-ttu-id="5cd12-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5cd12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cd12-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5cd12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cd12-106">检索基于标识符为租户中学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="5cd12-106">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="5cd12-107">权限</span><span class="sxs-lookup"><span data-stu-id="5cd12-107">Permissions</span></span>
<span data-ttu-id="5cd12-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cd12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cd12-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cd12-110">Permission type</span></span> | <span data-ttu-id="5cd12-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cd12-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5cd12-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cd12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5cd12-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cd12-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5cd12-114">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="5cd12-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5cd12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cd12-115">Not supported.</span></span>|
|<span data-ttu-id="5cd12-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cd12-116">Application</span></span>| <span data-ttu-id="5cd12-117">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd12-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cd12-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cd12-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5cd12-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cd12-119">Request headers</span></span>
| <span data-ttu-id="5cd12-120">名称</span><span class="sxs-lookup"><span data-stu-id="5cd12-120">Name</span></span>       | <span data-ttu-id="5cd12-121">类型</span><span class="sxs-lookup"><span data-stu-id="5cd12-121">Type</span></span> | <span data-ttu-id="5cd12-122">说明</span><span class="sxs-lookup"><span data-stu-id="5cd12-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5cd12-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cd12-123">Authorization</span></span>  | <span data-ttu-id="5cd12-124">string</span><span class="sxs-lookup"><span data-stu-id="5cd12-124">string</span></span>  | <span data-ttu-id="5cd12-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cd12-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5cd12-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cd12-127">Request body</span></span>
<span data-ttu-id="5cd12-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5cd12-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5cd12-129">响应</span><span class="sxs-lookup"><span data-stu-id="5cd12-129">Response</span></span>
<span data-ttu-id="5cd12-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5cd12-130">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd12-131">示例</span><span class="sxs-lookup"><span data-stu-id="5cd12-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cd12-132">请求</span><span class="sxs-lookup"><span data-stu-id="5cd12-132">Request</span></span>
<span data-ttu-id="5cd12-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5cd12-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="5cd12-134">响应</span><span class="sxs-lookup"><span data-stu-id="5cd12-134">Response</span></span>
<span data-ttu-id="5cd12-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5cd12-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5cd12-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5cd12-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
    "licensesToAssign": 
         [
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
```
