---
title: 获取一个目录设置模板
description: 目录设置模板表示的设置可能会从其内租户中创建设置的模板。 此操作允许检索 directorySettingTemplate 对象，包括可用的设置和默认值的属性。
ms.openlocfilehash: 1928642883632a672ddaccb9181f6366ade5ce04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041982"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="7cbcb-104">获取一个目录设置模板</span><span class="sxs-lookup"><span data-stu-id="7cbcb-104">Get a directory setting template</span></span>

> <span data-ttu-id="7cbcb-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cbcb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cbcb-107">目录设置模板表示的设置可能会从其内租户中创建设置的模板。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-107">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="7cbcb-108">此操作允许检索 directorySettingTemplate 对象，包括可用的设置和默认值的属性。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-108">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="7cbcb-109">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7cbcb-110">此 API 的 /v1.0 版本已被重命名为*Get groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-110">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cbcb-111">权限</span><span class="sxs-lookup"><span data-stu-id="7cbcb-111">Permissions</span></span>
<span data-ttu-id="7cbcb-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cbcb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cbcb-114">Permission type</span></span>      | <span data-ttu-id="7cbcb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cbcb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cbcb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cbcb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7cbcb-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cbcb-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cbcb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cbcb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cbcb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-119">Not supported.</span></span>    |
|<span data-ttu-id="7cbcb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cbcb-120">Application</span></span> | <span data-ttu-id="7cbcb-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cbcb-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cbcb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cbcb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7cbcb-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7cbcb-123">Optional query parameters</span></span>
<span data-ttu-id="7cbcb-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cbcb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cbcb-125">Request headers</span></span>
| <span data-ttu-id="7cbcb-126">名称</span><span class="sxs-lookup"><span data-stu-id="7cbcb-126">Name</span></span>      |<span data-ttu-id="7cbcb-127">说明</span><span class="sxs-lookup"><span data-stu-id="7cbcb-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7cbcb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cbcb-128">Authorization</span></span>  | <span data-ttu-id="7cbcb-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cbcb-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cbcb-131">Request body</span></span>
<span data-ttu-id="7cbcb-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cbcb-133">响应</span><span class="sxs-lookup"><span data-stu-id="7cbcb-133">Response</span></span>

<span data-ttu-id="7cbcb-134">如果成功，此方法返回`200 OK`响应正文中的响应代码和[directorySettingTemplate](../resources/directorysettingtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-134">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7cbcb-135">示例</span><span class="sxs-lookup"><span data-stu-id="7cbcb-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cbcb-136">请求</span><span class="sxs-lookup"><span data-stu-id="7cbcb-136">Request</span></span>
<span data-ttu-id="7cbcb-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="7cbcb-138">响应</span><span class="sxs-lookup"><span data-stu-id="7cbcb-138">Response</span></span>
<span data-ttu-id="7cbcb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7cbcb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

{
  "id": "id-value",
  "displayName": "displayName-value",
  "description": "description-value",
  "values": [
    {
      "name": "name-value",
      "type": "type-value",
      "defaultValue": "defaultValue-value",
      "description": "description-value"
    }
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->