---
title: 在组中创建目录设置
description: 使用此 API 为组创建新的目录设置。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3ba33de148e34ce80c0a709a6a1b5faf99d5f32d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502079"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="e158d-103">在组中创建目录设置</span><span class="sxs-lookup"><span data-stu-id="e158d-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e158d-104">使用此 API 为组创建新的目录设置。</span><span class="sxs-lookup"><span data-stu-id="e158d-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e158d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e158d-105">Permissions</span></span>
<span data-ttu-id="e158d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e158d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e158d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e158d-108">Permission type</span></span>      | <span data-ttu-id="e158d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e158d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e158d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e158d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e158d-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e158d-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e158d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e158d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e158d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e158d-113">Not supported.</span></span>    |
|<span data-ttu-id="e158d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e158d-114">Application</span></span> | <span data-ttu-id="e158d-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e158d-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e158d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e158d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="e158d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e158d-117">Request headers</span></span>
| <span data-ttu-id="e158d-118">名称</span><span class="sxs-lookup"><span data-stu-id="e158d-118">Name</span></span>       | <span data-ttu-id="e158d-119">说明</span><span class="sxs-lookup"><span data-stu-id="e158d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e158d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e158d-120">Authorization</span></span>  | <span data-ttu-id="e158d-121">持有者 <token>。</span><span class="sxs-lookup"><span data-stu-id="e158d-121">Bearer <token>.</span></span> <span data-ttu-id="e158d-122">必需</span><span class="sxs-lookup"><span data-stu-id="e158d-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e158d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e158d-123">Request body</span></span>
<span data-ttu-id="e158d-124">在请求正文中, 提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e158d-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e158d-125">响应</span><span class="sxs-lookup"><span data-stu-id="e158d-125">Response</span></span>

<span data-ttu-id="e158d-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e158d-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e158d-127">示例</span><span class="sxs-lookup"><span data-stu-id="e158d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e158d-128">请求</span><span class="sxs-lookup"><span data-stu-id="e158d-128">Request</span></span>
<span data-ttu-id="e158d-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e158d-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="e158d-130">在请求正文中, 提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e158d-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e158d-131">响应</span><span class="sxs-lookup"><span data-stu-id="e158d-131">Response</span></span>
<span data-ttu-id="e158d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e158d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
