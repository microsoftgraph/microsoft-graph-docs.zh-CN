---
title: 更新团队照片
description: 更新团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a33220682e2df2fb084944cfb8474c592e7649d7
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290088"
---
# <a name="update-team-photo"></a><span data-ttu-id="73113-103">更新团队照片</span><span class="sxs-lookup"><span data-stu-id="73113-103">Update team photo</span></span>

<span data-ttu-id="73113-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73113-105">更新团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="73113-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="73113-106">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="73113-106">The following are the supported sizes of HD photos in Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="73113-107">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="73113-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="73113-108">请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="73113-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="73113-109">这会将照片大小限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="73113-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="73113-110">权限</span><span class="sxs-lookup"><span data-stu-id="73113-110">Permissions</span></span>

<span data-ttu-id="73113-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73113-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73113-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="73113-113">Permission type</span></span>      | <span data-ttu-id="73113-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73113-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73113-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73113-115">Delegated (work or school account)</span></span> | <span data-ttu-id="73113-116">TeamSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="73113-116">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="73113-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73113-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73113-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="73113-118">Not supported.</span></span>    |
|<span data-ttu-id="73113-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="73113-119">Application</span></span> | <span data-ttu-id="73113-120">TeamSettings （[RSC](https://aka.ms/teams-rsc)）、TeamSettings、All、group、All、All 和 All。 all</span><span class="sxs-lookup"><span data-stu-id="73113-120">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73113-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73113-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="73113-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="73113-122">Request headers</span></span>

| <span data-ttu-id="73113-123">标头</span><span class="sxs-lookup"><span data-stu-id="73113-123">Header</span></span>        | <span data-ttu-id="73113-124">值</span><span class="sxs-lookup"><span data-stu-id="73113-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="73113-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73113-125">Authorization</span></span> | <span data-ttu-id="73113-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73113-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73113-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="73113-128">Content-type</span></span> | <span data-ttu-id="73113-p105">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="73113-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73113-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="73113-131">Request body</span></span>

<span data-ttu-id="73113-132">在请求正文中包括照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="73113-132">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="73113-133">响应</span><span class="sxs-lookup"><span data-stu-id="73113-133">Response</span></span>

<span data-ttu-id="73113-134">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="73113-134">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73113-135">示例</span><span class="sxs-lookup"><span data-stu-id="73113-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="73113-136">请求</span><span class="sxs-lookup"><span data-stu-id="73113-136">Request</span></span>

<span data-ttu-id="73113-137">下面是更新团队照片的请求示例。</span><span class="sxs-lookup"><span data-stu-id="73113-137">Here is an example of the request to update a team photo.</span></span>

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

### <a name="response"></a><span data-ttu-id="73113-138">响应</span><span class="sxs-lookup"><span data-stu-id="73113-138">Response</span></span> 

<span data-ttu-id="73113-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73113-139">Here is an example of the response.</span></span>

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
