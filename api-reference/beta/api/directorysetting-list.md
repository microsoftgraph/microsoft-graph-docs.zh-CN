---
title: 列表目录设置
description: 检索目录设置对象的列表。
author: lleonard-msft
ms.openlocfilehash: 2d3c7d24009fb0068376629aa50197678774f683
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319038"
---
# <a name="list-directory-settings"></a><span data-ttu-id="b676d-103">列表目录设置</span><span class="sxs-lookup"><span data-stu-id="b676d-103">List directory settings</span></span>

> <span data-ttu-id="b676d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b676d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b676d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b676d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b676d-106">检索目录设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b676d-106">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="b676d-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="b676d-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b676d-108">此 API 的 /v1.0 版本已被重命名为*列表 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="b676d-108">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b676d-109">权限</span><span class="sxs-lookup"><span data-stu-id="b676d-109">Permissions</span></span>
<span data-ttu-id="b676d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b676d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b676d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b676d-112">Permission type</span></span>      | <span data-ttu-id="b676d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b676d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b676d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b676d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b676d-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b676d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b676d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b676d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b676d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b676d-117">Not supported.</span></span>    |
|<span data-ttu-id="b676d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b676d-118">Application</span></span> | <span data-ttu-id="b676d-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b676d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b676d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b676d-120">HTTP request</span></span>
<span data-ttu-id="b676d-121"><!-- { "blockType": "ignored" } -->列出租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="b676d-121"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b676d-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b676d-122">Optional query parameters</span></span>
<span data-ttu-id="b676d-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b676d-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b676d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b676d-124">Request headers</span></span>
| <span data-ttu-id="b676d-125">Name</span><span class="sxs-lookup"><span data-stu-id="b676d-125">Name</span></span>      |<span data-ttu-id="b676d-126">说明</span><span class="sxs-lookup"><span data-stu-id="b676d-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b676d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b676d-127">Authorization</span></span>  | <span data-ttu-id="b676d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b676d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b676d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b676d-130">Request body</span></span>
<span data-ttu-id="b676d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b676d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b676d-132">响应</span><span class="sxs-lookup"><span data-stu-id="b676d-132">Response</span></span>

<span data-ttu-id="b676d-133">如果成功，此方法返回`200 OK`响应代码和响应正文中的[directorySetting](../resources/directorysetting.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b676d-133">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b676d-134">示例</span><span class="sxs-lookup"><span data-stu-id="b676d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b676d-135">请求</span><span class="sxs-lookup"><span data-stu-id="b676d-135">Request</span></span>
<span data-ttu-id="b676d-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b676d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="b676d-137">响应</span><span class="sxs-lookup"><span data-stu-id="b676d-137">Response</span></span>
<span data-ttu-id="b676d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b676d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
