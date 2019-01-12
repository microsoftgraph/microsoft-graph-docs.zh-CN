---
title: 将文件上载到 educationSynchronizationProfile 后启动同步
description: 验证文件上载到租户中的特定学校数据同步配置文件。 如果验证操作成功，将配置文件上启动同步。 否则，响应将包含错误和警告。 如果响应中包含错误，将不会启动同步。 如果则响应中包含仅警告，将启动同步。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: efdc0863a1de58f7ebf46492b662e632972275c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915247"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="3193d-107">将文件上载到 educationSynchronizationProfile 后启动同步</span><span class="sxs-lookup"><span data-stu-id="3193d-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

> <span data-ttu-id="3193d-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3193d-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3193d-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3193d-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3193d-110">验证文件上载到租户中特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="3193d-110">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="3193d-111">如果验证操作成功，将配置文件上启动同步。</span><span class="sxs-lookup"><span data-stu-id="3193d-111">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="3193d-112">否则，响应将包含错误和警告。</span><span class="sxs-lookup"><span data-stu-id="3193d-112">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="3193d-113">如果响应中包含错误，将不会启动同步。</span><span class="sxs-lookup"><span data-stu-id="3193d-113">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="3193d-114">如果则响应中包含仅警告，将启动同步。</span><span class="sxs-lookup"><span data-stu-id="3193d-114">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="3193d-115">**注意：** 仅当数据提供程序的类型[educationcsvdataprovider](../resources/educationcsvdataprovider.md)时，请使用此方法。</span><span class="sxs-lookup"><span data-stu-id="3193d-115">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="3193d-116">此外，需要设置之前可以启动配置文件的状态属性。</span><span class="sxs-lookup"><span data-stu-id="3193d-116">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="3193d-117">轮询要检查其状态属性的配置文件对象。</span><span class="sxs-lookup"><span data-stu-id="3193d-117">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3193d-118">权限</span><span class="sxs-lookup"><span data-stu-id="3193d-118">Permissions</span></span>
<span data-ttu-id="3193d-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3193d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3193d-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="3193d-121">Permission type</span></span> | <span data-ttu-id="3193d-122">Permissions</span><span class="sxs-lookup"><span data-stu-id="3193d-122">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3193d-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3193d-123">Delegated (work or school account)</span></span> | <span data-ttu-id="3193d-124">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3193d-124">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3193d-125">委派 （个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="3193d-125">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3193d-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="3193d-126">Not supported.</span></span>|
|<span data-ttu-id="3193d-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="3193d-127">Application</span></span>|<span data-ttu-id="3193d-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="3193d-128">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3193d-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3193d-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="3193d-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="3193d-130">Request headers</span></span>
| <span data-ttu-id="3193d-131">名称</span><span class="sxs-lookup"><span data-stu-id="3193d-131">Name</span></span>       | <span data-ttu-id="3193d-132">类型</span><span class="sxs-lookup"><span data-stu-id="3193d-132">Type</span></span> | <span data-ttu-id="3193d-133">说明</span><span class="sxs-lookup"><span data-stu-id="3193d-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3193d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3193d-134">Authorization</span></span>  | <span data-ttu-id="3193d-135">string</span><span class="sxs-lookup"><span data-stu-id="3193d-135">string</span></span>  | <span data-ttu-id="3193d-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3193d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3193d-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="3193d-138">Request body</span></span>
<span data-ttu-id="3193d-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3193d-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3193d-140">响应</span><span class="sxs-lookup"><span data-stu-id="3193d-140">Response</span></span>
<span data-ttu-id="3193d-141">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3193d-141">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="3193d-142">如果不成功，则返回`400 Bad Request`。</span><span class="sxs-lookup"><span data-stu-id="3193d-142">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="3193d-143">如果找到任何错误或警告则响应中包含的响应正文一部分[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3193d-143">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="3193d-144">示例</span><span class="sxs-lookup"><span data-stu-id="3193d-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3193d-145">请求</span><span class="sxs-lookup"><span data-stu-id="3193d-145">Request</span></span>
<span data-ttu-id="3193d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3193d-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="3193d-147">响应</span><span class="sxs-lookup"><span data-stu-id="3193d-147">Response</span></span>
<span data-ttu-id="3193d-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3193d-148">Here is an example of the response.</span></span> 

><span data-ttu-id="3193d-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3193d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
