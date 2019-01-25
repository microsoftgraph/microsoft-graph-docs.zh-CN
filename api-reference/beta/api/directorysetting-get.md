---
title: 获取一个目录设置
description: 检索特定目录设置对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad7b0137e741ff6c6766980f121838ae00d8200
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525288"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="d5fca-103">获取一个目录设置</span><span class="sxs-lookup"><span data-stu-id="d5fca-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5fca-104">检索特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d5fca-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="d5fca-105">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="d5fca-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d5fca-106">此 API 的 /v1.0 版本已被重命名为*Get groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="d5fca-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5fca-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5fca-107">Permissions</span></span>
<span data-ttu-id="d5fca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5fca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5fca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5fca-110">Permission type</span></span>      | <span data-ttu-id="d5fca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5fca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5fca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5fca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5fca-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5fca-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5fca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5fca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5fca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5fca-115">Not supported.</span></span>    |
|<span data-ttu-id="d5fca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5fca-116">Application</span></span> | <span data-ttu-id="d5fca-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5fca-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5fca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5fca-118">HTTP request</span></span>
<span data-ttu-id="d5fca-119"><!-- { "blockType": "ignored" } -->获取特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="d5fca-119"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5fca-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5fca-120">Optional query parameters</span></span>
<span data-ttu-id="d5fca-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5fca-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5fca-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5fca-122">Request headers</span></span>
| <span data-ttu-id="d5fca-123">名称</span><span class="sxs-lookup"><span data-stu-id="d5fca-123">Name</span></span>      |<span data-ttu-id="d5fca-124">说明</span><span class="sxs-lookup"><span data-stu-id="d5fca-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5fca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5fca-125">Authorization</span></span>  | <span data-ttu-id="d5fca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5fca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5fca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5fca-128">Request body</span></span>
<span data-ttu-id="d5fca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5fca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5fca-130">响应</span><span class="sxs-lookup"><span data-stu-id="d5fca-130">Response</span></span>

<span data-ttu-id="d5fca-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5fca-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5fca-132">示例</span><span class="sxs-lookup"><span data-stu-id="d5fca-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5fca-133">请求</span><span class="sxs-lookup"><span data-stu-id="d5fca-133">Request</span></span>
<span data-ttu-id="d5fca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5fca-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="d5fca-135">响应</span><span class="sxs-lookup"><span data-stu-id="d5fca-135">Response</span></span>
<span data-ttu-id="d5fca-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5fca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
