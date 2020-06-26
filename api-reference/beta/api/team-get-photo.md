---
title: 获取团队照片
description: 获取团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a02f0cd05c0f092fbafc584e9a74a578122f7c5
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896502"
---
# <a name="get-team-photo"></a><span data-ttu-id="6c6e4-103">获取团队照片</span><span class="sxs-lookup"><span data-stu-id="6c6e4-103">Get team photo</span></span>

<span data-ttu-id="6c6e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c6e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c6e4-105">获取团队的照片（图片），或者获取照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-105">Get the photo (picture) for a team, or metadata for the photo.</span></span> <span data-ttu-id="6c6e4-106">通常情况下，最佳做法是先尝试在元数据中检索想要获取的照片的尺寸，以确保该尺寸可用。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-106">In general, it is a best practice to first attempt to retrieve the metadata for the size of the photo you'd like to get to ensure that size is available.</span></span> <span data-ttu-id="6c6e4-107">检索到元数据后，使用 `/$value` 路径获取照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-107">Once you have retrieved the metadata, use the `/$value` path to get the binary data for the photo.</span></span>

<span data-ttu-id="6c6e4-108">此方法首先尝试从 Microsoft 365 检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-108">This method first attempts to retrieve the specified photo from Microsoft 365.</span></span> <span data-ttu-id="6c6e4-109">如果照片在 Microsoft 365 中不可用，则它会尝试改为从 Azure Active Directory 检索照片。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-109">If the photo is not available in Microsoft 365, it attempts to retrieve the photo from Azure Active Directory instead.</span></span>

<span data-ttu-id="6c6e4-110">以下是 Microsoft 365 中受支持的 HD 照片的大小：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-110">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="6c6e4-111">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-111">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="6c6e4-112">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-112">You can get the metadata of the largest available photo, or optionally specify a size to get the metadata for that photo size.</span></span> <span data-ttu-id="6c6e4-113">即使请求的尺寸不可用，也仍可获取更小的尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-113">If the size you request is not available, you can still get a smaller size.</span></span> <span data-ttu-id="6c6e4-114">例如，上传的照片最大为 504x504 像素，则除 648x648 尺寸以外的所有照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-114">For example, if the largest photo uploaded is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span> <span data-ttu-id="6c6e4-115">如果指定的大小在 Microsoft 365 或 Azure Active Directory 中不可用，则使用元数据的其余部分返回的大小为1x1。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-115">If the specified size is not available in the Microsoft 365 or in Azure Active Directory, the size 1x1 is returned with the rest of the metadata.</span></span>

> [!Note]
> <span data-ttu-id="6c6e4-116">REST 请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-116">There is a limit of 4 MB on the total size of the REST request.</span></span> <span data-ttu-id="6c6e4-117">这将照片尺寸限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-117">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c6e4-118">权限</span><span class="sxs-lookup"><span data-stu-id="6c6e4-118">Permissions</span></span>

<span data-ttu-id="6c6e4-119">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6c6e4-119">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6c6e4-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6e4-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6e4-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c6e4-121">Permission type</span></span>      | <span data-ttu-id="6c6e4-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c6e4-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c6e4-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6e4-123">Delegated (work or school account)</span></span> | <span data-ttu-id="6c6e4-124">User.readbasic.all、TeamSettings、TeamSettings、Group、group、group。 all、、、all、all、all、all 和 all。 all</span><span class="sxs-lookup"><span data-stu-id="6c6e4-124">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="6c6e4-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c6e4-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c6e4-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-126">Not supported.</span></span>    |
|<span data-ttu-id="6c6e4-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c6e4-127">Application</span></span> | <span data-ttu-id="6c6e4-128">TeamSettings、*TeamSettings*、User.readbasic.all、TeamSettings、、group、group、group、group。 all、、、、all、all、all、all、All 和 all 的所有</span><span class="sxs-lookup"><span data-stu-id="6c6e4-128">TeamSettings.Read.Group *, TeamSettings.Edit.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="6c6e4-129">**注意**：标记为 \* 的权限使用[特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-129">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="6c6e4-130">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-130">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6c6e4-131">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-131">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c6e4-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c6e4-132">HTTP request</span></span>

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="6c6e4-133">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="6c6e4-133">Get the metadata of the photo</span></span>

<span data-ttu-id="6c6e4-134">此终结点将返回照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-134">This endpoint will return the metadata of the photo.</span></span> <span data-ttu-id="6c6e4-135">如果未指定尺寸，则将返回可供使用的最大照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-135">If no size is specified, the metadata for the largest photo size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
GET /teams/{id}/photo/{size}
```

### <a name="get-the-photo"></a><span data-ttu-id="6c6e4-136">获取照片</span><span class="sxs-lookup"><span data-stu-id="6c6e4-136">Get the photo</span></span>

<span data-ttu-id="6c6e4-137">此终结点将在二进制数据中检索照片。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-137">This endpoint will retrieve the binary data for the photo.</span></span> <span data-ttu-id="6c6e4-138">如果未指定尺寸，则将返回可供使用的最大尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-138">If no size is specified, the largest size available will be returned.</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
GET /beta/teams/{id}/photo/$value
GET /beta/teams/{id}/photo/{size}/$value
```

## <a name="path-parameters"></a><span data-ttu-id="6c6e4-139">路径参数</span><span class="sxs-lookup"><span data-stu-id="6c6e4-139">Path parameters</span></span>

<span data-ttu-id="6c6e4-140">此方法支持用可选路径参数来指定要检索的照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-140">This method supports an optional path parameter to specify the size of the photo to be retrieved.</span></span> <span data-ttu-id="6c6e4-141">指定的尺寸不得超过最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-141">You can specify any size up to the largest available size.</span></span> <span data-ttu-id="6c6e4-142">获取照片元数据以确定最大可用尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-142">Get the photo metadata to determine the largest size available.</span></span>

|<span data-ttu-id="6c6e4-143">**参数**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-143">**Parameter**</span></span>|<span data-ttu-id="6c6e4-144">**类型**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-144">**Type**</span></span>|<span data-ttu-id="6c6e4-145">**说明**</span><span class="sxs-lookup"><span data-stu-id="6c6e4-145">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6c6e4-146">size</span><span class="sxs-lookup"><span data-stu-id="6c6e4-146">size</span></span>  |<span data-ttu-id="6c6e4-147">String</span><span class="sxs-lookup"><span data-stu-id="6c6e4-147">String</span></span>  | <span data-ttu-id="6c6e4-148">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-148">A photo size.</span></span> <span data-ttu-id="6c6e4-149">Microsoft 365 上支持的 HD 照片的大小如下所示：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和648x648。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-149">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="6c6e4-150">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-150">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> <span data-ttu-id="6c6e4-151">可选。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-151">Optional.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6c6e4-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c6e4-152">Request headers</span></span>

| <span data-ttu-id="6c6e4-153">标头</span><span class="sxs-lookup"><span data-stu-id="6c6e4-153">Header</span></span>        | <span data-ttu-id="6c6e4-154">值</span><span class="sxs-lookup"><span data-stu-id="6c6e4-154">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6c6e4-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6e4-155">Authorization</span></span> | <span data-ttu-id="6c6e4-156">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6c6e4-156">Bearer {token}.</span></span> <span data-ttu-id="6c6e4-157">Required.</span><span class="sxs-lookup"><span data-stu-id="6c6e4-157">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c6e4-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c6e4-158">Request body</span></span>

<span data-ttu-id="6c6e4-159">请勿提供此请求的正文。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-159">Do not supply a body for this request.</span></span>

## <a name="response"></a><span data-ttu-id="6c6e4-160">响应</span><span class="sxs-lookup"><span data-stu-id="6c6e4-160">Response</span></span>

### <a name="response-for-getting-the-metadata-of-a-photo"></a><span data-ttu-id="6c6e4-161">针对获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="6c6e4-161">Response for getting the metadata of a photo</span></span>

<span data-ttu-id="6c6e4-162">如果成功，此方法会返回 `200 OK` 响应代码和照片元数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-162">If successful, this method returns a `200 OK` response code, and metadata about the photo.</span></span>

### <a name="response-for-getting-the-photo"></a><span data-ttu-id="6c6e4-163">针对获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="6c6e4-163">Response for getting the photo</span></span>

<span data-ttu-id="6c6e4-164">如果成功，此方法会返回 `200 OK` 响应代码和照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-164">If successful, this method returns a `200 OK` response code, and the binary data for the photo.</span></span>

## <a name="examples"></a><span data-ttu-id="6c6e4-165">示例</span><span class="sxs-lookup"><span data-stu-id="6c6e4-165">Examples</span></span>

### <a name="example-1-get-the-photo-metadata"></a><span data-ttu-id="6c6e4-166">示例 1：获取照片元数据</span><span class="sxs-lookup"><span data-stu-id="6c6e4-166">Example 1: Get the photo metadata</span></span>

#### <a name="request"></a><span data-ttu-id="6c6e4-167">请求</span><span class="sxs-lookup"><span data-stu-id="6c6e4-167">Request</span></span>

<span data-ttu-id="6c6e4-168">下述示例展示了要获取团队照片元数据的请求。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-168">Here is an example of the request to get the metadata of the team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a><span data-ttu-id="6c6e4-169">响应</span><span class="sxs-lookup"><span data-stu-id="6c6e4-169">Response</span></span>

<span data-ttu-id="6c6e4-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-170">Here is an example of the response.</span></span>

> <span data-ttu-id="6c6e4-171">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="6c6e4-171">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6c6e4-172">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6c6e4-172">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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

### <a name="example-2-get-a-specific-size-of-the-team-photo"></a><span data-ttu-id="6c6e4-173">示例 2：获取团队照片的特定尺寸</span><span class="sxs-lookup"><span data-stu-id="6c6e4-173">Example 2: Get a specific size of the team photo</span></span>

<span data-ttu-id="6c6e4-174">下述示例展示了要获取特定尺寸的团队照片的请求。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-174">Here is an example of the request to get the team photo in a specific size.</span></span>

#### <a name="request"></a><span data-ttu-id="6c6e4-175">请求</span><span class="sxs-lookup"><span data-stu-id="6c6e4-175">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/240x240/$value
```

#### <a name="response"></a><span data-ttu-id="6c6e4-176">响应</span><span class="sxs-lookup"><span data-stu-id="6c6e4-176">Response</span></span>

<span data-ttu-id="6c6e4-177">包含所请求的 240x240 尺寸照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-177">Contains the binary data of the requested 240x240 photo.</span></span> <span data-ttu-id="6c6e4-178">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="6c6e4-178">The HTTP response code is 200.</span></span>

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
