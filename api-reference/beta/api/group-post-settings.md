---
title: 在组中创建一个目录设置
description: 使用此 API 创建新目录设置组。
author: dkershaw10
ms.openlocfilehash: 2e400babc809bdc8d9277cad1bd41b8b714e4e92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358994"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="fc02b-103">在组中创建一个目录设置</span><span class="sxs-lookup"><span data-stu-id="fc02b-103">Create a directory setting on groups</span></span>

> <span data-ttu-id="fc02b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fc02b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc02b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fc02b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc02b-106">使用此 API 创建新目录设置组。</span><span class="sxs-lookup"><span data-stu-id="fc02b-106">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc02b-107">权限</span><span class="sxs-lookup"><span data-stu-id="fc02b-107">Permissions</span></span>
<span data-ttu-id="fc02b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc02b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc02b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc02b-110">Permission type</span></span>      | <span data-ttu-id="fc02b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc02b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc02b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc02b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc02b-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc02b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc02b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc02b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc02b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc02b-115">Not supported.</span></span>    |
|<span data-ttu-id="fc02b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc02b-116">Application</span></span> | <span data-ttu-id="fc02b-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc02b-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc02b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc02b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="fc02b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc02b-119">Request headers</span></span>
| <span data-ttu-id="fc02b-120">Name</span><span class="sxs-lookup"><span data-stu-id="fc02b-120">Name</span></span>       | <span data-ttu-id="fc02b-121">说明</span><span class="sxs-lookup"><span data-stu-id="fc02b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc02b-122">授权</span><span class="sxs-lookup"><span data-stu-id="fc02b-122">Authorization</span></span>  | <span data-ttu-id="fc02b-123">持有者<token>。</span><span class="sxs-lookup"><span data-stu-id="fc02b-123">Bearer <token>.</span></span> <span data-ttu-id="fc02b-124">是否必需</span><span class="sxs-lookup"><span data-stu-id="fc02b-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc02b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc02b-125">Request body</span></span>
<span data-ttu-id="fc02b-126">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc02b-126">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc02b-127">响应</span><span class="sxs-lookup"><span data-stu-id="fc02b-127">Response</span></span>

<span data-ttu-id="fc02b-128">如果成功，此方法返回`201 Created`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc02b-128">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc02b-129">示例</span><span class="sxs-lookup"><span data-stu-id="fc02b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc02b-130">请求</span><span class="sxs-lookup"><span data-stu-id="fc02b-130">Request</span></span>
<span data-ttu-id="fc02b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc02b-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="fc02b-132">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc02b-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc02b-133">响应</span><span class="sxs-lookup"><span data-stu-id="fc02b-133">Response</span></span>
<span data-ttu-id="fc02b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc02b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->