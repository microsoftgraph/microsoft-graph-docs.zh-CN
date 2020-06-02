---
title: 更新团队照片
description: 更新团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bb824a0bd6b79f4450f4a2d3658e0853376db594
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491887"
---
# <a name="update-team-photo"></a><span data-ttu-id="c15bd-103">更新团队照片</span><span class="sxs-lookup"><span data-stu-id="c15bd-103">Update team photo</span></span>

<span data-ttu-id="c15bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c15bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c15bd-105">更新团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="c15bd-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="c15bd-106">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="c15bd-106">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="c15bd-107">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="c15bd-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="c15bd-108">请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="c15bd-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="c15bd-109">这会将照片大小限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="c15bd-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="c15bd-110">权限</span><span class="sxs-lookup"><span data-stu-id="c15bd-110">Permissions</span></span>

<span data-ttu-id="c15bd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c15bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c15bd-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c15bd-113">Permission type</span></span>      | <span data-ttu-id="c15bd-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c15bd-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c15bd-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c15bd-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c15bd-116">TeamSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="c15bd-116">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c15bd-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c15bd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c15bd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c15bd-118">Not supported.</span></span>    |
|<span data-ttu-id="c15bd-119">Application</span><span class="sxs-lookup"><span data-stu-id="c15bd-119">Application</span></span> | <span data-ttu-id="c15bd-120">TeamSettings \*、TeamSettings、all、ReadWrite、all、all、All、All</span><span class="sxs-lookup"><span data-stu-id="c15bd-120">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="c15bd-121">**注意**：标记为 \* 的权限使用[特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="c15bd-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="c15bd-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="c15bd-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c15bd-123">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="c15bd-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c15bd-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c15bd-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="c15bd-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c15bd-125">Request headers</span></span>

| <span data-ttu-id="c15bd-126">标头</span><span class="sxs-lookup"><span data-stu-id="c15bd-126">Header</span></span>        | <span data-ttu-id="c15bd-127">值</span><span class="sxs-lookup"><span data-stu-id="c15bd-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c15bd-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c15bd-128">Authorization</span></span> | <span data-ttu-id="c15bd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c15bd-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c15bd-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="c15bd-131">Content-type</span></span> | <span data-ttu-id="c15bd-p106">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="c15bd-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c15bd-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c15bd-134">Request body</span></span>

<span data-ttu-id="c15bd-135">在请求正文中包括照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="c15bd-135">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="c15bd-136">响应</span><span class="sxs-lookup"><span data-stu-id="c15bd-136">Response</span></span>

<span data-ttu-id="c15bd-137">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c15bd-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c15bd-138">示例</span><span class="sxs-lookup"><span data-stu-id="c15bd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c15bd-139">请求</span><span class="sxs-lookup"><span data-stu-id="c15bd-139">Request</span></span>

<span data-ttu-id="c15bd-140">下面是更新团队照片的请求示例。</span><span class="sxs-lookup"><span data-stu-id="c15bd-140">Here is an example of the request to update a team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a><span data-ttu-id="c15bd-141">响应</span><span class="sxs-lookup"><span data-stu-id="c15bd-141">Response</span></span> 

<span data-ttu-id="c15bd-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c15bd-142">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
