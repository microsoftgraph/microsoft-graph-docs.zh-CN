---
title: 创建组设置
description: 基于 groupSettingTemplates 中可用的模板创建新设置。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b3d67940a8d4ba71b3377c867edf2a0a8f11c80
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679762"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="d59f8-103">创建组设置</span><span class="sxs-lookup"><span data-stu-id="d59f8-103">Create a group setting</span></span>

<span data-ttu-id="d59f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d59f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d59f8-105">使用此 API 基于 [groupSettingTemplates](../resources/groupsettingtemplate.md)中提供的模板创建新设置。</span><span class="sxs-lookup"><span data-stu-id="d59f8-105">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md).</span></span> <span data-ttu-id="d59f8-106">这些设置可以在租户级别或组级别。</span><span class="sxs-lookup"><span data-stu-id="d59f8-106">These settings can be at the tenant-level or at the group level.</span></span> <span data-ttu-id="d59f8-107">创建请求必须为模板中定义的所有设置提供[settingValues。](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d59f8-107">The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template.</span></span> <span data-ttu-id="d59f8-108">对于特定于组的设置，只能设置管理组的成员是否可以邀请来宾用户的设置。</span><span class="sxs-lookup"><span data-stu-id="d59f8-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="d59f8-109">一旦向组添加来宾用户这一功能已普遍可用，这将控制此行为。</span><span class="sxs-lookup"><span data-stu-id="d59f8-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span> <span data-ttu-id="d59f8-110">对于 beta 终结点，请使用 [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="d59f8-110">For beta endpoints, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="permissions"></a><span data-ttu-id="d59f8-111">权限</span><span class="sxs-lookup"><span data-stu-id="d59f8-111">Permissions</span></span>

<span data-ttu-id="d59f8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d59f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d59f8-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d59f8-114">Permission type</span></span>      | <span data-ttu-id="d59f8-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d59f8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d59f8-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d59f8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d59f8-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d59f8-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d59f8-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d59f8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d59f8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d59f8-119">Not supported.</span></span>    |
|<span data-ttu-id="d59f8-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d59f8-120">Application</span></span> | <span data-ttu-id="d59f8-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d59f8-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d59f8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d59f8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="d59f8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d59f8-123">Request headers</span></span>

| <span data-ttu-id="d59f8-124">名称</span><span class="sxs-lookup"><span data-stu-id="d59f8-124">Name</span></span> | <span data-ttu-id="d59f8-125">说明</span><span class="sxs-lookup"><span data-stu-id="d59f8-125">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d59f8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d59f8-126">Authorization</span></span> | <span data-ttu-id="d59f8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d59f8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d59f8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d59f8-129">Content-Type</span></span> | <span data-ttu-id="d59f8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d59f8-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d59f8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d59f8-131">Request body</span></span>
<span data-ttu-id="d59f8-p104">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。但是，设置的显示名称将根据引用的设置模板名称进行设置。</span><span class="sxs-lookup"><span data-stu-id="d59f8-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="d59f8-134">响应</span><span class="sxs-lookup"><span data-stu-id="d59f8-134">Response</span></span>

<span data-ttu-id="d59f8-135">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d59f8-135">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d59f8-136">示例</span><span class="sxs-lookup"><span data-stu-id="d59f8-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d59f8-137">请求</span><span class="sxs-lookup"><span data-stu-id="d59f8-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d59f8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d59f8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d59f8-139">C#</span><span class="sxs-lookup"><span data-stu-id="d59f8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d59f8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d59f8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d59f8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d59f8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d59f8-142">Java</span><span class="sxs-lookup"><span data-stu-id="d59f8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d59f8-143">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d59f8-143">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d59f8-144">响应</span><span class="sxs-lookup"><span data-stu-id="d59f8-144">Response</span></span>

<span data-ttu-id="d59f8-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d59f8-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

