---
title: 获取组设置模板
description: 获取一个组设置模板，该模板代表可以在租户中创建设置的设置的模板。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c90fc6b3c30991583765d960173636580c7258e3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679748"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="8b9bb-103">获取组设置模板</span><span class="sxs-lookup"><span data-stu-id="8b9bb-103">Get a group setting template</span></span>

<span data-ttu-id="8b9bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b9bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b9bb-p101">组设置模板表示用于在租户内创建设置的设置模板。此操作允许检索 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象的属性，包括可用设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b9bb-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b9bb-107">Permissions</span></span>

<span data-ttu-id="8b9bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8b9bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b9bb-110">Permission type</span></span>      | <span data-ttu-id="8b9bb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b9bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b9bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b9bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b9bb-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b9bb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b9bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b9bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b9bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-115">Not supported.</span></span>    |
|<span data-ttu-id="8b9bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b9bb-116">Application</span></span> | <span data-ttu-id="8b9bb-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9bb-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b9bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b9bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b9bb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8b9bb-119">Optional query parameters</span></span>
<span data-ttu-id="8b9bb-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b9bb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b9bb-121">Request headers</span></span>
| <span data-ttu-id="8b9bb-122">名称</span><span class="sxs-lookup"><span data-stu-id="8b9bb-122">Name</span></span> | <span data-ttu-id="8b9bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="8b9bb-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8b9bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b9bb-124">Authorization</span></span> | <span data-ttu-id="8b9bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b9bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b9bb-127">Request body</span></span>
<span data-ttu-id="8b9bb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b9bb-129">响应</span><span class="sxs-lookup"><span data-stu-id="8b9bb-129">Response</span></span>

<span data-ttu-id="8b9bb-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b9bb-131">示例</span><span class="sxs-lookup"><span data-stu-id="8b9bb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b9bb-132">请求</span><span class="sxs-lookup"><span data-stu-id="8b9bb-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b9bb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9bb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="8b9bb-134">C#</span><span class="sxs-lookup"><span data-stu-id="8b9bb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b9bb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b9bb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b9bb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b9bb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b9bb-137">Java</span><span class="sxs-lookup"><span data-stu-id="8b9bb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b9bb-138">响应</span><span class="sxs-lookup"><span data-stu-id="8b9bb-138">Response</span></span>

<span data-ttu-id="8b9bb-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b9bb-139">Note: The response object shown here might be shortened for readability.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
