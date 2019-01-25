---
title: 创建所有者
description: 使用此 API 创建一个新的所有者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 81008665fadab5b81907a334329169870cd5fab6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528583"
---
# <a name="create-owner"></a><span data-ttu-id="a0caf-103">创建所有者</span><span class="sxs-lookup"><span data-stu-id="a0caf-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0caf-104">使用此 API 创建一个新的所有者。</span><span class="sxs-lookup"><span data-stu-id="a0caf-104">Use this API to create a new owner.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0caf-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0caf-105">Permissions</span></span>
<span data-ttu-id="a0caf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0caf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0caf-108">Permission type</span></span>      | <span data-ttu-id="a0caf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0caf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0caf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0caf-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0caf-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0caf-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0caf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0caf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0caf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0caf-113">Not supported.</span></span>    |
|<span data-ttu-id="a0caf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0caf-114">Application</span></span> | <span data-ttu-id="a0caf-115">Application.ReadWrite.OwnedBy Directory.Read.All、 Application.ReadWrite.All 和 Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0caf-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0caf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0caf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners

```
## <a name="request-headers"></a><span data-ttu-id="a0caf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0caf-117">Request headers</span></span>
| <span data-ttu-id="a0caf-118">名称</span><span class="sxs-lookup"><span data-stu-id="a0caf-118">Name</span></span>       | <span data-ttu-id="a0caf-119">类型</span><span class="sxs-lookup"><span data-stu-id="a0caf-119">Type</span></span> | <span data-ttu-id="a0caf-120">说明</span><span class="sxs-lookup"><span data-stu-id="a0caf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0caf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0caf-121">Authorization</span></span>  | <span data-ttu-id="a0caf-122">string</span><span class="sxs-lookup"><span data-stu-id="a0caf-122">string</span></span>  | <span data-ttu-id="a0caf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0caf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0caf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0caf-125">Request body</span></span>
<span data-ttu-id="a0caf-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0caf-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0caf-127">响应</span><span class="sxs-lookup"><span data-stu-id="a0caf-127">Response</span></span>

<span data-ttu-id="a0caf-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0caf-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0caf-129">示例</span><span class="sxs-lookup"><span data-stu-id="a0caf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0caf-130">请求</span><span class="sxs-lookup"><span data-stu-id="a0caf-130">Request</span></span>
<span data-ttu-id="a0caf-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0caf-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="a0caf-132">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0caf-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0caf-133">响应</span><span class="sxs-lookup"><span data-stu-id="a0caf-133">Response</span></span>
<span data-ttu-id="a0caf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0caf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
