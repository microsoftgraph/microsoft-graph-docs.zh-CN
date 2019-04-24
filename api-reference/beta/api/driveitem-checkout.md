---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 签出文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bd69a02a3c243a86d7f9d05b54eb3fac00eeee88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454727"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="cf673-102">签出 DriveItem 资源</span><span class="sxs-lookup"><span data-stu-id="cf673-102">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf673-103">签出 driveItem 资源以防止在[签入](driveitem-checkin.md)文档前其他人编辑文档和看到所做的更改。</span><span class="sxs-lookup"><span data-stu-id="cf673-103">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf673-104">权限</span><span class="sxs-lookup"><span data-stu-id="cf673-104">Permissions</span></span>

<span data-ttu-id="cf673-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf673-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf673-107">Permission type</span></span>      | <span data-ttu-id="cf673-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf673-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf673-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf673-109">Delegated (work or school account)</span></span> | <span data-ttu-id="cf673-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf673-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf673-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf673-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf673-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf673-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf673-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf673-113">Application</span></span> | <span data-ttu-id="cf673-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf673-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf673-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf673-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="cf673-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf673-116">Request body</span></span>

<span data-ttu-id="cf673-117">无需请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf673-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="cf673-118">示例</span><span class="sxs-lookup"><span data-stu-id="cf673-118">Example</span></span>

<span data-ttu-id="cf673-119">本示例签出由 `{item-id}` 标识的文件。</span><span class="sxs-lookup"><span data-stu-id="cf673-119">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="cf673-120">响应</span><span class="sxs-lookup"><span data-stu-id="cf673-120">Response</span></span>

<span data-ttu-id="cf673-121">如果成功，该 API 调用会返回 `204 No content`。</span><span class="sxs-lookup"><span data-stu-id="cf673-121">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="cf673-122">注解</span><span class="sxs-lookup"><span data-stu-id="cf673-122">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-checkout.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
