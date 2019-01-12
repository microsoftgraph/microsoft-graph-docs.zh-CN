---
title: 获取一个目录设置
description: 检索特定目录设置对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73953ccedeb7ecaeeba5cb68e6827956430ada82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950821"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="e46bc-103">获取一个目录设置</span><span class="sxs-lookup"><span data-stu-id="e46bc-103">Get a directory setting</span></span>

> <span data-ttu-id="e46bc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e46bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e46bc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e46bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e46bc-106">检索特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e46bc-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="e46bc-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="e46bc-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="e46bc-108">此 API 的 /v1.0 版本已被重命名为*Get groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="e46bc-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="e46bc-109">权限</span><span class="sxs-lookup"><span data-stu-id="e46bc-109">Permissions</span></span>
<span data-ttu-id="e46bc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e46bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e46bc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="e46bc-112">Permission type</span></span>      | <span data-ttu-id="e46bc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e46bc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e46bc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e46bc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e46bc-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e46bc-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e46bc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e46bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e46bc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e46bc-117">Not supported.</span></span>    |
|<span data-ttu-id="e46bc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e46bc-118">Application</span></span> | <span data-ttu-id="e46bc-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e46bc-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e46bc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e46bc-120">HTTP request</span></span>
<span data-ttu-id="e46bc-121"><!-- { "blockType": "ignored" } -->获取特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="e46bc-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e46bc-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e46bc-122">Optional query parameters</span></span>
<span data-ttu-id="e46bc-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e46bc-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e46bc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="e46bc-124">Request headers</span></span>
| <span data-ttu-id="e46bc-125">名称</span><span class="sxs-lookup"><span data-stu-id="e46bc-125">Name</span></span>      |<span data-ttu-id="e46bc-126">说明</span><span class="sxs-lookup"><span data-stu-id="e46bc-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e46bc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e46bc-127">Authorization</span></span>  | <span data-ttu-id="e46bc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e46bc-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e46bc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e46bc-130">Request body</span></span>
<span data-ttu-id="e46bc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e46bc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e46bc-132">响应</span><span class="sxs-lookup"><span data-stu-id="e46bc-132">Response</span></span>

<span data-ttu-id="e46bc-133">如果成功，此方法返回`200 OK`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e46bc-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e46bc-134">示例</span><span class="sxs-lookup"><span data-stu-id="e46bc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e46bc-135">请求</span><span class="sxs-lookup"><span data-stu-id="e46bc-135">Request</span></span>
<span data-ttu-id="e46bc-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e46bc-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="e46bc-137">响应</span><span class="sxs-lookup"><span data-stu-id="e46bc-137">Response</span></span>
<span data-ttu-id="e46bc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e46bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
