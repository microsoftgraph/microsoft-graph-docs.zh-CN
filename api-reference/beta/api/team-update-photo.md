---
title: 更新团队照片
description: 更新团队的照片（图片）。
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c19e09713d16f8c2739b1a8398509953a19ddd0
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418333"
---
# <a name="update-team-photo"></a><span data-ttu-id="02a32-103">更新团队照片</span><span class="sxs-lookup"><span data-stu-id="02a32-103">Update team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a32-104">更新团队的照片（图片）。</span><span class="sxs-lookup"><span data-stu-id="02a32-104">Update the photo (picture) for a team.</span></span> <span data-ttu-id="02a32-105">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648 像素。</span><span class="sxs-lookup"><span data-stu-id="02a32-105">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="02a32-106">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="02a32-106">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="02a32-107">请求的总大小不得超过 4 MB。</span><span class="sxs-lookup"><span data-stu-id="02a32-107">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="02a32-108">这会将照片大小限制为小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="02a32-108">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a32-109">权限</span><span class="sxs-lookup"><span data-stu-id="02a32-109">Permissions</span></span>

<span data-ttu-id="02a32-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02a32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a32-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="02a32-112">Permission type</span></span>      | <span data-ttu-id="02a32-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02a32-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a32-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02a32-114">Delegated (work or school account)</span></span> | <span data-ttu-id="02a32-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a32-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02a32-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02a32-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a32-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="02a32-117">Not supported.</span></span>    |
|<span data-ttu-id="02a32-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="02a32-118">Application</span></span> | <span data-ttu-id="02a32-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a32-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a32-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02a32-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="02a32-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="02a32-121">Request headers</span></span>

| <span data-ttu-id="02a32-122">标头</span><span class="sxs-lookup"><span data-stu-id="02a32-122">Header</span></span>        | <span data-ttu-id="02a32-123">值</span><span class="sxs-lookup"><span data-stu-id="02a32-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="02a32-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a32-124">Authorization</span></span> | <span data-ttu-id="02a32-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02a32-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="02a32-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="02a32-127">Content-type</span></span> | <span data-ttu-id="02a32-p105">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="02a32-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02a32-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="02a32-130">Request body</span></span>

<span data-ttu-id="02a32-131">在请求正文中包括照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="02a32-131">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="02a32-132">响应</span><span class="sxs-lookup"><span data-stu-id="02a32-132">Response</span></span>

<span data-ttu-id="02a32-133">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="02a32-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02a32-134">示例</span><span class="sxs-lookup"><span data-stu-id="02a32-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a32-135">请求</span><span class="sxs-lookup"><span data-stu-id="02a32-135">Request</span></span>

<span data-ttu-id="02a32-136">下面是更新团队照片的请求示例。</span><span class="sxs-lookup"><span data-stu-id="02a32-136">Here is an example of the request to update a team photo.</span></span>

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

### <a name="response"></a><span data-ttu-id="02a32-137">响应</span><span class="sxs-lookup"><span data-stu-id="02a32-137">Response</span></span> 

<span data-ttu-id="02a32-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="02a32-138">Here is an example of the response.</span></span>

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
