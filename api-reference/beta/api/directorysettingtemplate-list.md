---
title: 列表 directorySettingTemplates
description: 目录设置模板代表一组目录设置，从目录设置可能会创建和租户中使用的模板。  此操作检索可用的 directorySettingTemplates 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 288a914da11c09cd39767a48d527510998c9be1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833325"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="8a0f3-104">列表 directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="8a0f3-104">List directorySettingTemplates</span></span>

> <span data-ttu-id="8a0f3-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a0f3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a0f3-107">目录设置模板代表一组目录设置，从目录设置可能会创建和租户中使用的模板。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-107">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="8a0f3-108">此操作检索可用的 directorySettingTemplates 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-108">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="8a0f3-109">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="8a0f3-110">此 API 的 /v1.0 版本已被重命名为*列表 groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-110">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a0f3-111">权限</span><span class="sxs-lookup"><span data-stu-id="8a0f3-111">Permissions</span></span>
<span data-ttu-id="8a0f3-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a0f3-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a0f3-114">Permission type</span></span>      | <span data-ttu-id="8a0f3-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a0f3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a0f3-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a0f3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8a0f3-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a0f3-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a0f3-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a0f3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a0f3-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-119">Not supported.</span></span>    |
|<span data-ttu-id="8a0f3-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a0f3-120">Application</span></span> | <span data-ttu-id="8a0f3-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a0f3-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a0f3-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a0f3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a0f3-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8a0f3-123">Optional query parameters</span></span>
<span data-ttu-id="8a0f3-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a0f3-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a0f3-125">Request headers</span></span>
| <span data-ttu-id="8a0f3-126">名称</span><span class="sxs-lookup"><span data-stu-id="8a0f3-126">Name</span></span>      |<span data-ttu-id="8a0f3-127">说明</span><span class="sxs-lookup"><span data-stu-id="8a0f3-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8a0f3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a0f3-128">Authorization</span></span>  | <span data-ttu-id="8a0f3-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a0f3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a0f3-131">Request body</span></span>
<span data-ttu-id="8a0f3-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a0f3-133">响应</span><span class="sxs-lookup"><span data-stu-id="8a0f3-133">Response</span></span>

<span data-ttu-id="8a0f3-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[directorySettingTemplate](../resources/directorysettingtemplate.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-134">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a0f3-135">示例</span><span class="sxs-lookup"><span data-stu-id="8a0f3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a0f3-136">请求</span><span class="sxs-lookup"><span data-stu-id="8a0f3-136">Request</span></span>
<span data-ttu-id="8a0f3-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="8a0f3-138">响应</span><span class="sxs-lookup"><span data-stu-id="8a0f3-138">Response</span></span>
<span data-ttu-id="8a0f3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a0f3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
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
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
