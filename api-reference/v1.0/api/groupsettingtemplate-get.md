---
title: 获取组设置模板
description: 组设置模板代表可在租户中创建设置的设置模板。 此操作允许检索 groupSettingTemplate 对象的属性, 包括可用的设置及其默认值。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 642e896c61dee0d0ed3b49dee0124565bc1792c2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613018"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="b7205-104">获取组设置模板</span><span class="sxs-lookup"><span data-stu-id="b7205-104">Get a group setting template</span></span>

<span data-ttu-id="b7205-p102">组设置模板表示用于在租户内创建设置的设置模板。此操作允许检索 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象的属性，包括可用设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="b7205-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7205-107">权限</span><span class="sxs-lookup"><span data-stu-id="b7205-107">Permissions</span></span>

<span data-ttu-id="b7205-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7205-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7205-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7205-110">Permission type</span></span>      | <span data-ttu-id="b7205-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7205-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7205-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7205-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7205-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b7205-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b7205-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7205-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7205-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7205-115">Not supported.</span></span>    |
|<span data-ttu-id="b7205-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7205-116">Application</span></span> | <span data-ttu-id="b7205-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7205-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7205-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7205-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7205-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b7205-119">Optional query parameters</span></span>
<span data-ttu-id="b7205-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b7205-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7205-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7205-121">Request headers</span></span>
| <span data-ttu-id="b7205-122">名称</span><span class="sxs-lookup"><span data-stu-id="b7205-122">Name</span></span> | <span data-ttu-id="b7205-123">说明</span><span class="sxs-lookup"><span data-stu-id="b7205-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b7205-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7205-124">Authorization</span></span> | <span data-ttu-id="b7205-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7205-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7205-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7205-127">Request body</span></span>
<span data-ttu-id="b7205-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7205-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7205-129">响应</span><span class="sxs-lookup"><span data-stu-id="b7205-129">Response</span></span>

<span data-ttu-id="b7205-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7205-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7205-131">示例</span><span class="sxs-lookup"><span data-stu-id="b7205-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7205-132">请求</span><span class="sxs-lookup"><span data-stu-id="b7205-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="b7205-133">响应</span><span class="sxs-lookup"><span data-stu-id="b7205-133">Response</span></span>

<span data-ttu-id="b7205-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7205-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b7205-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="b7205-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b7205-137">语言</span><span class="sxs-lookup"><span data-stu-id="b7205-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7205-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b7205-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsettingtemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
