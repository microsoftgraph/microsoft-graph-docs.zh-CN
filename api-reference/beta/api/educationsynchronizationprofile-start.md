---
title: 将文件上传到 educationSynchronizationProfile 后开始同步
description: 验证是否已将文件上载到租户中的特定学校数据同步配置文件。 如果验证成功, 将在配置文件上启动同步。 否则, 响应中将包含错误和警告。 如果响应中包含错误, 同步将不会启动。 如果响应仅包含警告, 将启动同步。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2c571ca614c8bb97babe93537e99606ce8799b0f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441273"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="be919-107">将文件上传到 educationSynchronizationProfile 后开始同步</span><span class="sxs-lookup"><span data-stu-id="be919-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be919-108">验证是否已将文件上载到租户中的特定学校数据[同步配置文件](../resources/educationsynchronizationprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="be919-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="be919-109">如果验证成功, 将在配置文件上启动同步。</span><span class="sxs-lookup"><span data-stu-id="be919-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="be919-110">否则, 响应中将包含错误和警告。</span><span class="sxs-lookup"><span data-stu-id="be919-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="be919-111">如果响应中包含错误, 同步将不会启动。</span><span class="sxs-lookup"><span data-stu-id="be919-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="be919-112">如果响应仅包含警告, 将启动同步。</span><span class="sxs-lookup"><span data-stu-id="be919-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="be919-113">**注意:** 仅当数据提供程序的类型为[educationcsvdataprovider](../resources/educationcsvdataprovider.md)时, 才可使用此方法。</span><span class="sxs-lookup"><span data-stu-id="be919-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="be919-114">此外, 还需要先设置配置文件的 state 属性, 然后才能启动该属性。</span><span class="sxs-lookup"><span data-stu-id="be919-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="be919-115">轮询配置文件对象以检查其状态属性。</span><span class="sxs-lookup"><span data-stu-id="be919-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="be919-116">权限</span><span class="sxs-lookup"><span data-stu-id="be919-116">Permissions</span></span>
<span data-ttu-id="be919-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be919-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be919-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="be919-119">Permission type</span></span> | <span data-ttu-id="be919-120">权限</span><span class="sxs-lookup"><span data-stu-id="be919-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="be919-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be919-121">Delegated (work or school account)</span></span> | <span data-ttu-id="be919-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be919-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="be919-123">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="be919-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="be919-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="be919-124">Not supported.</span></span>|
|<span data-ttu-id="be919-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="be919-125">Application</span></span>|<span data-ttu-id="be919-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="be919-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be919-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be919-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="be919-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="be919-128">Request headers</span></span>
| <span data-ttu-id="be919-129">名称</span><span class="sxs-lookup"><span data-stu-id="be919-129">Name</span></span>       | <span data-ttu-id="be919-130">类型</span><span class="sxs-lookup"><span data-stu-id="be919-130">Type</span></span> | <span data-ttu-id="be919-131">说明</span><span class="sxs-lookup"><span data-stu-id="be919-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be919-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="be919-132">Authorization</span></span>  | <span data-ttu-id="be919-133">string</span><span class="sxs-lookup"><span data-stu-id="be919-133">string</span></span>  | <span data-ttu-id="be919-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be919-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be919-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="be919-136">Request body</span></span>
<span data-ttu-id="be919-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be919-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="be919-138">响应</span><span class="sxs-lookup"><span data-stu-id="be919-138">Response</span></span>
<span data-ttu-id="be919-139">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="be919-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="be919-140">如果不成功, 则返回`400 Bad Request`。</span><span class="sxs-lookup"><span data-stu-id="be919-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="be919-141">如果发现任何错误或警告, 响应将包含[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)对象的集合作为响应正文的一部分。</span><span class="sxs-lookup"><span data-stu-id="be919-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="be919-142">示例</span><span class="sxs-lookup"><span data-stu-id="be919-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be919-143">请求</span><span class="sxs-lookup"><span data-stu-id="be919-143">Request</span></span>
<span data-ttu-id="be919-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be919-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be919-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="be919-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="be919-146">C#</span><span class="sxs-lookup"><span data-stu-id="be919-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be919-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="be919-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be919-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="be919-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="be919-149">响应</span><span class="sxs-lookup"><span data-stu-id="be919-149">Response</span></span>
<span data-ttu-id="be919-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="be919-150">Here is an example of the response.</span></span> 

><span data-ttu-id="be919-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be919-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
