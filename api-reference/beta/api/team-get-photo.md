---
title: 获取团队照片
description: 获取团队的照片（图片）。
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7329a471abcc6d1777b5f067e892d3351e408ed5
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060311"
---
# <a name="get-team-photo"></a><span data-ttu-id="4e764-103">获取团队照片</span><span class="sxs-lookup"><span data-stu-id="4e764-103">Get team photo</span></span>

<span data-ttu-id="4e764-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e764-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e764-105">获取团队的照片（图片），或者获取照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-105">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="4e764-106">通常情况下，最佳做法是先尝试在元数据中检索想要获取的照片的尺寸，以确保该尺寸可用。</span><span class="sxs-lookup"><span data-stu-id="4e764-106">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="4e764-107">检索到元数据后，使用 `/$value` 路径获取照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-107">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="4e764-108">此方法会先尝试从 Microsoft 365 中检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="4e764-108">This method first attempts to retrieve the specified photo from Microsoft 365.</span></span> <span data-ttu-id="4e764-109">如果 Microsoft 365 中没有此照片，则它会改为尝试在 Active Directory 中检索照片。</span><span class="sxs-lookup"><span data-stu-id="4e764-109">If the photo is not available in Microsoft 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="4e764-110">Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="4e764-110">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="4e764-111">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-111">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="4e764-p104">可以获取最大可用照片的元数据，或者也可以指定一个大小来获取该照片大小的元数据。如果请求的大小不可用，仍可获取较小的大小。例如，如果上载的最大照片像素为 504x504 的照片，则除大小为 648x648 的照片之外的所有照片都可供下载。如果在 Microsoft 365 或 Azure Active Directory 中没有可用的指定大小，则会返回 1x1 的大小和剩余的元数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-p104">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size. If the size you request is not available, you can still get a smaller size. For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download. If the specified size is not available in the Microsoft 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="4e764-116">REST 请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="4e764-116">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="4e764-117">这将照片尺寸限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="4e764-117">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e764-118">权限</span><span class="sxs-lookup"><span data-stu-id="4e764-118">Permissions</span></span>

<span data-ttu-id="4e764-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e764-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e764-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e764-121">Permission type</span></span>      | <span data-ttu-id="4e764-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e764-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e764-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e764-123">Delegated (work or school account)</span></span> | <span data-ttu-id="4e764-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e764-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4e764-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e764-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e764-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e764-126">Not supported.</span></span>    |
|<span data-ttu-id="4e764-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e764-127">Application</span></span> | <span data-ttu-id="4e764-128">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e764-128">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>  |

> <span data-ttu-id="4e764-129">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="4e764-129">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4e764-p107">**注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="4e764-p107">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e764-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e764-132">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="4e764-133">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="4e764-133">Get the metadata of the photo</span></span>

<span data-ttu-id="4e764-134">此终结点将返回照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-134">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="4e764-135">如果未指定尺寸，则将返回可供使用的最大照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-135">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="4e764-136">获取照片</span><span class="sxs-lookup"><span data-stu-id="4e764-136">Get the photo</span></span>

<span data-ttu-id="4e764-137">此终结点将在二进制数据中检索照片。</span><span class="sxs-lookup"><span data-stu-id="4e764-137">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="4e764-138">如果未指定尺寸，则将返回可供使用的最大尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-138">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="4e764-139">路径参数</span><span class="sxs-lookup"><span data-stu-id="4e764-139">Path parameters</span></span>

<span data-ttu-id="4e764-140">此方法支持用可选路径参数来指定要检索的照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-140">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="4e764-141">指定的尺寸不得超过最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-141">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="4e764-142">获取照片元数据以确定最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-142">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="4e764-143">**参数**</span><span class="sxs-lookup"><span data-stu-id="4e764-143">**Parameter**</span></span>|<span data-ttu-id="4e764-144">**类型**</span><span class="sxs-lookup"><span data-stu-id="4e764-144">**Type**</span></span>|<span data-ttu-id="4e764-145">**说明**</span><span class="sxs-lookup"><span data-stu-id="4e764-145">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4e764-146">size</span><span class="sxs-lookup"><span data-stu-id="4e764-146">size</span></span>  |<span data-ttu-id="4e764-147">String</span><span class="sxs-lookup"><span data-stu-id="4e764-147">String</span></span>  | <span data-ttu-id="4e764-148">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-148">A photo size.</span></span> <span data-ttu-id="4e764-149">Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="4e764-149">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="4e764-150">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="4e764-150">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="4e764-151">可选。</span><span class="sxs-lookup"><span data-stu-id="4e764-151">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4e764-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e764-152">Request headers</span></span>

| <span data-ttu-id="4e764-153">标头</span><span class="sxs-lookup"><span data-stu-id="4e764-153">Header</span></span>        | <span data-ttu-id="4e764-154">值</span><span class="sxs-lookup"><span data-stu-id="4e764-154">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="4e764-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e764-155">Authorization</span></span> | <span data-ttu-id="4e764-p112">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e764-p112">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e764-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e764-158">Request body</span></span>

<span data-ttu-id="4e764-159">请勿提供此请求的正文。</span><span class="sxs-lookup"><span data-stu-id="4e764-159">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="4e764-160">响应</span><span class="sxs-lookup"><span data-stu-id="4e764-160">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="4e764-161">针对获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="4e764-161">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="4e764-162">如果成功，此方法会返回 `200 OK` 响应代码和照片元数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-162">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="4e764-163">针对获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="4e764-163">Response for getting the photo</span></span>

<span data-ttu-id="4e764-164">如果成功，此方法会返回 `200 OK` 响应代码和照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="4e764-164">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="4e764-165">示例</span><span class="sxs-lookup"><span data-stu-id="4e764-165">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="4e764-166">示例 1：获取照片元数据</span><span class="sxs-lookup"><span data-stu-id="4e764-166">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="4e764-167">请求</span><span class="sxs-lookup"><span data-stu-id="4e764-167">Request</span></span>

<span data-ttu-id="4e764-168">下述示例展示了要获取团队照片元数据的请求。</span><span class="sxs-lookup"><span data-stu-id="4e764-168">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="4e764-169">响应</span><span class="sxs-lookup"><span data-stu-id="4e764-169">Response</span></span>

<span data-ttu-id="4e764-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e764-170">Here is an example of the response.</span></span>

> <span data-ttu-id="4e764-171">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e764-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="4e764-172">示例 2：获取团队照片的特定尺寸</span><span class="sxs-lookup"><span data-stu-id="4e764-172">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="4e764-173">下述示例展示了要获取特定尺寸的团队照片的请求。</span><span class="sxs-lookup"><span data-stu-id="4e764-173">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="4e764-174">请求</span><span class="sxs-lookup"><span data-stu-id="4e764-174">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="4e764-175">响应</span><span class="sxs-lookup"><span data-stu-id="4e764-175">Response</span></span>

<span data-ttu-id="4e764-p113">包含所请求的 240x240 照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="4e764-p113">Contains the binary data of the requested 240x240 photo. The HTTP response code is 200.</span></span>

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


