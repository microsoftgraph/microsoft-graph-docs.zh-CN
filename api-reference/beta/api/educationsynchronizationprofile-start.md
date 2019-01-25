---
title: 将文件上载到 educationSynchronizationProfile 后启动同步
description: 验证文件上载到租户中的特定学校数据同步配置文件。 如果验证操作成功，将配置文件上启动同步。 否则，响应将包含错误和警告。 如果响应中包含错误，将不会启动同步。 如果则响应中包含仅警告，将启动同步。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1447178e80d30058b415345aea83dce4390e6bcf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512351"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="f6a1a-107">将文件上载到 educationSynchronizationProfile 后启动同步</span><span class="sxs-lookup"><span data-stu-id="f6a1a-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a1a-108">验证文件上载到租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f6a1a-109">如果验证操作成功，将配置文件上启动同步。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="f6a1a-110">否则，响应将包含错误和警告。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="f6a1a-111">如果响应中包含错误，将不会启动同步。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="f6a1a-112">如果则响应中包含仅警告，将启动同步。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="f6a1a-113">**注意：** 仅当数据提供程序的类型[educationcsvdataprovider](../resources/educationcsvdataprovider.md)时，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="f6a1a-114">此外，需要设置之前可以启动配置文件的状态属性。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="f6a1a-115">轮询要检查其状态属性的配置文件对象。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6a1a-116">权限</span><span class="sxs-lookup"><span data-stu-id="f6a1a-116">Permissions</span></span>
<span data-ttu-id="f6a1a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6a1a-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6a1a-119">Permission type</span></span> | <span data-ttu-id="f6a1a-120">权限</span><span class="sxs-lookup"><span data-stu-id="f6a1a-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f6a1a-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a1a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="f6a1a-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6a1a-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f6a1a-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6a1a-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f6a1a-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-124">Not supported.</span></span>|
|<span data-ttu-id="f6a1a-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6a1a-125">Application</span></span>|<span data-ttu-id="f6a1a-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6a1a-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6a1a-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="f6a1a-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6a1a-128">Request headers</span></span>
| <span data-ttu-id="f6a1a-129">名称</span><span class="sxs-lookup"><span data-stu-id="f6a1a-129">Name</span></span>       | <span data-ttu-id="f6a1a-130">类型</span><span class="sxs-lookup"><span data-stu-id="f6a1a-130">Type</span></span> | <span data-ttu-id="f6a1a-131">说明</span><span class="sxs-lookup"><span data-stu-id="f6a1a-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6a1a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6a1a-132">Authorization</span></span>  | <span data-ttu-id="f6a1a-133">string</span><span class="sxs-lookup"><span data-stu-id="f6a1a-133">string</span></span>  | <span data-ttu-id="f6a1a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6a1a-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6a1a-136">Request body</span></span>
<span data-ttu-id="f6a1a-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f6a1a-138">响应</span><span class="sxs-lookup"><span data-stu-id="f6a1a-138">Response</span></span>
<span data-ttu-id="f6a1a-139">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="f6a1a-140">如果不成功，则返回`400 Bad Request`。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="f6a1a-141">如果找到任何错误或警告则响应中包含的响应正文一部分[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="f6a1a-142">示例</span><span class="sxs-lookup"><span data-stu-id="f6a1a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6a1a-143">请求</span><span class="sxs-lookup"><span data-stu-id="f6a1a-143">Request</span></span>
<span data-ttu-id="f6a1a-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="f6a1a-145">响应</span><span class="sxs-lookup"><span data-stu-id="f6a1a-145">Response</span></span>
<span data-ttu-id="f6a1a-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-146">Here is an example of the response.</span></span> 

><span data-ttu-id="f6a1a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6a1a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
