---
title: 列表 directorySettingTemplates
description: 目录设置模板代表一组目录设置，从目录设置可能会创建和租户中使用的模板。  此操作检索可用的 directorySettingTemplates 对象的列表。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cd0112bd0d9f98f969832427d497d6e9ba2aa14
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530102"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="c61a8-104">列表 directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="c61a8-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61a8-105">目录设置模板代表一组目录设置，从目录设置可能会创建和租户中使用的模板。</span><span class="sxs-lookup"><span data-stu-id="c61a8-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="c61a8-106">此操作检索可用的 directorySettingTemplates 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c61a8-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="c61a8-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="c61a8-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="c61a8-108">此 API 的 /v1.0 版本已被重命名为*列表 groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="c61a8-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="c61a8-109">权限</span><span class="sxs-lookup"><span data-stu-id="c61a8-109">Permissions</span></span>
<span data-ttu-id="c61a8-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c61a8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61a8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c61a8-112">Permission type</span></span>      | <span data-ttu-id="c61a8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c61a8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61a8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c61a8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c61a8-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c61a8-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c61a8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c61a8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c61a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c61a8-117">Not supported.</span></span>    |
|<span data-ttu-id="c61a8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c61a8-118">Application</span></span> | <span data-ttu-id="c61a8-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61a8-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c61a8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c61a8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c61a8-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c61a8-121">Optional query parameters</span></span>
<span data-ttu-id="c61a8-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c61a8-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c61a8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c61a8-123">Request headers</span></span>
| <span data-ttu-id="c61a8-124">名称</span><span class="sxs-lookup"><span data-stu-id="c61a8-124">Name</span></span>      |<span data-ttu-id="c61a8-125">说明</span><span class="sxs-lookup"><span data-stu-id="c61a8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c61a8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61a8-126">Authorization</span></span>  | <span data-ttu-id="c61a8-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c61a8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c61a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c61a8-129">Request body</span></span>
<span data-ttu-id="c61a8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c61a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c61a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="c61a8-131">Response</span></span>

<span data-ttu-id="c61a8-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[directorySettingTemplate](../resources/directorysettingtemplate.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c61a8-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c61a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="c61a8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c61a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="c61a8-134">Request</span></span>
<span data-ttu-id="c61a8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c61a8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="c61a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="c61a8-136">Response</span></span>
<span data-ttu-id="c61a8-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c61a8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
