---
title: 获取团队照片
description: 获取团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 69bb246199ab38d3a17fc5ce30dce6f011f87b0a
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418340"
---
# <a name="get-team-photo"></a><span data-ttu-id="71fa8-103">获取团队照片</span><span class="sxs-lookup"><span data-stu-id="71fa8-103">Get team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71fa8-104">获取团队的照片（图片），或者获取照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-104">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="71fa8-105">通常情况下，最佳做法是先尝试在元数据中检索想要获取的照片的尺寸，以确保该尺寸可用。</span><span class="sxs-lookup"><span data-stu-id="71fa8-105">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="71fa8-106">检索到元数据后，使用 `/$value` 路径获取照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-106">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="71fa8-107">此方法会先尝试从 Office 365 中检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="71fa8-107">A GET photo method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="71fa8-108">如果 Office 365 中没有此照片，则它会改为尝试在 Active Directory 中检索照片。</span><span class="sxs-lookup"><span data-stu-id="71fa8-108">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="71fa8-109">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="71fa8-109">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="71fa8-110">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="71fa8-111">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-111">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="71fa8-112">即使请求的尺寸不可用，也仍可获取更小的尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-112">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span> <span data-ttu-id="71fa8-113">例如，上传的照片最大为 504x504 像素，则除 648x648 尺寸以外的所有照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="71fa8-113">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="71fa8-114">如果在 Office 365 或 Azure Active Directory 中找不到指定尺寸，则返回 1x1 的尺寸和剩余元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-114">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

> [!Note]
> <span data-ttu-id="71fa8-115">REST 请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="71fa8-115">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="71fa8-116">这将照片尺寸限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="71fa8-116">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="71fa8-117">权限</span><span class="sxs-lookup"><span data-stu-id="71fa8-117">Permissions</span></span>

<span data-ttu-id="71fa8-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71fa8-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fa8-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="71fa8-120">Permission type</span></span>      | <span data-ttu-id="71fa8-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71fa8-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71fa8-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71fa8-122">Delegated (work or school account)</span></span> | <span data-ttu-id="71fa8-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fa8-123">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="71fa8-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71fa8-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71fa8-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="71fa8-125">Not supported.</span></span>    |
|<span data-ttu-id="71fa8-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="71fa8-126">Application</span></span> | <span data-ttu-id="71fa8-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fa8-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71fa8-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71fa8-128">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="71fa8-129">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="71fa8-129">Get the metadata of the photo</span></span>

<span data-ttu-id="71fa8-130">此终结点将返回照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-130">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="71fa8-131">如果未指定尺寸，则将返回可供使用的最大照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-131">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo
GET /beta/teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="71fa8-132">获取照片</span><span class="sxs-lookup"><span data-stu-id="71fa8-132">Get the photo</span></span>

<span data-ttu-id="71fa8-133">此终结点将在二进制数据中检索照片。</span><span class="sxs-lookup"><span data-stu-id="71fa8-133">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="71fa8-134">如果未指定尺寸，则将返回可供使用的最大尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-134">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="71fa8-135">路径参数</span><span class="sxs-lookup"><span data-stu-id="71fa8-135">Path parameters</span></span>

<span data-ttu-id="71fa8-136">此方法支持用可选路径参数来指定要检索的照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-136">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="71fa8-137">指定的尺寸不得超过最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-137">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="71fa8-138">获取照片元数据以确定最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-138">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="71fa8-139">**参数**</span><span class="sxs-lookup"><span data-stu-id="71fa8-139">**Parameter**</span></span>|<span data-ttu-id="71fa8-140">**类型**</span><span class="sxs-lookup"><span data-stu-id="71fa8-140">**Type**</span></span>|<span data-ttu-id="71fa8-141">**说明**</span><span class="sxs-lookup"><span data-stu-id="71fa8-141">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="71fa8-142">size</span><span class="sxs-lookup"><span data-stu-id="71fa8-142">size</span></span>  |<span data-ttu-id="71fa8-143">String</span><span class="sxs-lookup"><span data-stu-id="71fa8-143">String</span></span>  | <span data-ttu-id="71fa8-144">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-144">A photo size.</span></span> <span data-ttu-id="71fa8-145">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="71fa8-145">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="71fa8-146">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="71fa8-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="71fa8-147">可选。</span><span class="sxs-lookup"><span data-stu-id="71fa8-147">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="71fa8-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="71fa8-148">Request headers</span></span>

| <span data-ttu-id="71fa8-149">标头</span><span class="sxs-lookup"><span data-stu-id="71fa8-149">Header</span></span>        | <span data-ttu-id="71fa8-150">值</span><span class="sxs-lookup"><span data-stu-id="71fa8-150">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="71fa8-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="71fa8-151">Authorization</span></span> | <span data-ttu-id="71fa8-p111">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71fa8-p111">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71fa8-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="71fa8-154">Request body</span></span>

<span data-ttu-id="71fa8-155">请勿提供此请求的正文。</span><span class="sxs-lookup"><span data-stu-id="71fa8-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71fa8-156">响应</span><span class="sxs-lookup"><span data-stu-id="71fa8-156">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="71fa8-157">针对获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="71fa8-157">Response for getting the metadata of the photo</span></span>

<span data-ttu-id="71fa8-158">如果成功，此方法会返回 `200 OK` 响应代码和照片元数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-158">If successful, this method returns a `200 OK` response code and binary data of the requested photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="71fa8-159">针对获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="71fa8-159">Response for getting the photo</span></span>

<span data-ttu-id="71fa8-160">如果成功，此方法会返回 `200 OK` 响应代码和照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-160">If successful, this method returns a `200 OK` response code and binary data of the requested photo.</span></span>

## <a name="examples"></a><span data-ttu-id="71fa8-161">示例</span><span class="sxs-lookup"><span data-stu-id="71fa8-161">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="71fa8-162">示例 1：获取照片元数据</span><span class="sxs-lookup"><span data-stu-id="71fa8-162">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="71fa8-163">请求</span><span class="sxs-lookup"><span data-stu-id="71fa8-163">Request</span></span>

<span data-ttu-id="71fa8-164">下述示例展示了要获取团队照片元数据的请求。</span><span class="sxs-lookup"><span data-stu-id="71fa8-164">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="71fa8-165">响应</span><span class="sxs-lookup"><span data-stu-id="71fa8-165">Response</span></span>

<span data-ttu-id="71fa8-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71fa8-166">Here is an example of the response.</span></span>

> <span data-ttu-id="71fa8-p112">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="71fa8-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="71fa8-169">示例 2：获取团队照片的特定尺寸</span><span class="sxs-lookup"><span data-stu-id="71fa8-169">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="71fa8-170">下述示例展示了要获取特定尺寸的团队照片的请求。</span><span class="sxs-lookup"><span data-stu-id="71fa8-170">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="71fa8-171">请求</span><span class="sxs-lookup"><span data-stu-id="71fa8-171">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="71fa8-172">响应</span><span class="sxs-lookup"><span data-stu-id="71fa8-172">Response</span></span>

<span data-ttu-id="71fa8-173">包含所请求的 240x240 尺寸照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="71fa8-173">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="71fa8-174">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="71fa8-174">The HTTP response code is 200.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
