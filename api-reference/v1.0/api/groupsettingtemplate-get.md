---
title: 获取组设置模板
description: 获取一个组设置模板，该模板代表可在租户中创建设置的设置的模板。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7af640dcf585499297a4df59ebc7f48b84749728
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402133"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="b68e5-103">获取组设置模板</span><span class="sxs-lookup"><span data-stu-id="b68e5-103">Get a group setting template</span></span>

<span data-ttu-id="b68e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b68e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b68e5-p101">组设置模板表示用于在租户内创建设置的设置模板。此操作允许检索 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象的属性，包括可用设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="b68e5-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="b68e5-107">权限</span><span class="sxs-lookup"><span data-stu-id="b68e5-107">Permissions</span></span>

<span data-ttu-id="b68e5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b68e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b68e5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b68e5-110">Permission type</span></span>      | <span data-ttu-id="b68e5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b68e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b68e5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b68e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b68e5-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b68e5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b68e5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b68e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b68e5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b68e5-115">Not supported.</span></span>    |
|<span data-ttu-id="b68e5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b68e5-116">Application</span></span> | <span data-ttu-id="b68e5-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b68e5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b68e5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b68e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b68e5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b68e5-119">Optional query parameters</span></span>
<span data-ttu-id="b68e5-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b68e5-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b68e5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b68e5-121">Request headers</span></span>
| <span data-ttu-id="b68e5-122">名称</span><span class="sxs-lookup"><span data-stu-id="b68e5-122">Name</span></span> | <span data-ttu-id="b68e5-123">说明</span><span class="sxs-lookup"><span data-stu-id="b68e5-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b68e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b68e5-124">Authorization</span></span> | <span data-ttu-id="b68e5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b68e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b68e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b68e5-127">Request body</span></span>
<span data-ttu-id="b68e5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b68e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b68e5-129">响应</span><span class="sxs-lookup"><span data-stu-id="b68e5-129">Response</span></span>

<span data-ttu-id="b68e5-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b68e5-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b68e5-131">示例</span><span class="sxs-lookup"><span data-stu-id="b68e5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b68e5-132">请求</span><span class="sxs-lookup"><span data-stu-id="b68e5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b68e5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b68e5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="b68e5-134">C#</span><span class="sxs-lookup"><span data-stu-id="b68e5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b68e5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b68e5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b68e5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b68e5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b68e5-137">Java</span><span class="sxs-lookup"><span data-stu-id="b68e5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b68e5-138">响应</span><span class="sxs-lookup"><span data-stu-id="b68e5-138">Response</span></span>

<span data-ttu-id="b68e5-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b68e5-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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