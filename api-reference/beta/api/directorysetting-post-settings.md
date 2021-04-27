---
title: 创建目录设置
description: 使用此 API 基于 directorySettingTemplates 中可用的模板创建新设置。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ab5281a940dd1dace265d87954cc49893c4d97f5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046578"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="a3833-103">创建目录设置</span><span class="sxs-lookup"><span data-stu-id="a3833-103">Create a directory setting</span></span>

<span data-ttu-id="a3833-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3833-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3833-105">使用此 API 基于 directorySettingTemplates 中可用的模板创建新设置。</span><span class="sxs-lookup"><span data-stu-id="a3833-105">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="a3833-106">这些设置可以位于租户级别或对象级别， (仅适用于组) 。</span><span class="sxs-lookup"><span data-stu-id="a3833-106">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="a3833-107">创建请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="a3833-107">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="a3833-108">对于特定于组的设置，只能设置管理组的成员是否可以邀请来宾用户的设置。</span><span class="sxs-lookup"><span data-stu-id="a3833-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="a3833-109">一旦向组添加来宾用户这一功能已普遍可用，这将控制此行为。</span><span class="sxs-lookup"><span data-stu-id="a3833-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="a3833-110">**注意**：此 API 的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="a3833-110">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="a3833-111">此 API 的 /v1.0 版本已重命名为 *Create groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="a3833-111">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="a3833-112">有关模板列表及其在 beta 中支持的属性，请使用 [directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。</span><span class="sxs-lookup"><span data-stu-id="a3833-112">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="a3833-113"> (对于 v1.0 终结点，请调用 [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).) </span><span class="sxs-lookup"><span data-stu-id="a3833-113">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="a3833-114">权限</span><span class="sxs-lookup"><span data-stu-id="a3833-114">Permissions</span></span>
<span data-ttu-id="a3833-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3833-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3833-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3833-117">Permission type</span></span>      | <span data-ttu-id="a3833-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3833-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3833-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3833-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a3833-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3833-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3833-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3833-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3833-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3833-122">Not supported.</span></span>    |
|<span data-ttu-id="a3833-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3833-123">Application</span></span> | <span data-ttu-id="a3833-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3833-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3833-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3833-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="a3833-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3833-126">Request headers</span></span>
| <span data-ttu-id="a3833-127">名称</span><span class="sxs-lookup"><span data-stu-id="a3833-127">Name</span></span>       | <span data-ttu-id="a3833-128">说明</span><span class="sxs-lookup"><span data-stu-id="a3833-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a3833-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3833-129">Authorization</span></span>  | <span data-ttu-id="a3833-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3833-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3833-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3833-132">Request body</span></span>
<span data-ttu-id="a3833-133">在请求正文中，提供 [directorySetting](../resources/directorysetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3833-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="a3833-134">但是，显示名称设置的名称将基于引用的设置模板名称进行设置。</span><span class="sxs-lookup"><span data-stu-id="a3833-134">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="a3833-135">响应</span><span class="sxs-lookup"><span data-stu-id="a3833-135">Response</span></span>

<span data-ttu-id="a3833-136">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [directorySetting](../resources/directorysetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3833-136">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3833-137">示例</span><span class="sxs-lookup"><span data-stu-id="a3833-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3833-138">请求</span><span class="sxs-lookup"><span data-stu-id="a3833-138">Request</span></span>
<span data-ttu-id="a3833-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3833-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3833-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3833-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a3833-141">C#</span><span class="sxs-lookup"><span data-stu-id="a3833-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3833-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3833-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3833-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3833-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3833-144">Java</span><span class="sxs-lookup"><span data-stu-id="a3833-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3833-145">在请求正文中，提供 [directorySetting](../resources/directorysetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3833-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a3833-146">响应</span><span class="sxs-lookup"><span data-stu-id="a3833-146">Response</span></span>
<span data-ttu-id="a3833-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a3833-147">Here is an example of the response.</span></span> <span data-ttu-id="a3833-148">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3833-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


