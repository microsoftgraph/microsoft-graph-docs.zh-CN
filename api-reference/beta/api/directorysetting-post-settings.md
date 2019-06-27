---
title: 创建目录设置
description: 根据 directorySettingTemplates 中可用的模板, 使用此 API 创建新的设置。 这些设置可以是租户级别, 也可以是对象级别 (当前仅适用于组)。 创建请求必须为模板中定义的所有设置提供 settingValues。 对于组特定的设置, 仅控制是否可以设置组成员是否可以邀请来宾用户的设置。 这样一来, 一旦能够将来宾用户添加到组中, 就可以控制此行为。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d3d0d9d9875c7dab66b7f9220cdf306164658ff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260548"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="a8cac-107">创建目录设置</span><span class="sxs-lookup"><span data-stu-id="a8cac-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8cac-108">根据 directorySettingTemplates 中可用的模板, 使用此 API 创建新的设置。</span><span class="sxs-lookup"><span data-stu-id="a8cac-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="a8cac-109">这些设置可以是租户级别, 也可以是对象级别 (当前仅适用于组)。</span><span class="sxs-lookup"><span data-stu-id="a8cac-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="a8cac-110">创建请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="a8cac-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="a8cac-111">对于组特定的设置, 仅控制是否可以设置组成员是否可以邀请来宾用户的设置。</span><span class="sxs-lookup"><span data-stu-id="a8cac-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="a8cac-112">这样一来, 一旦能够将来宾用户添加到组中, 就可以控制此行为。</span><span class="sxs-lookup"><span data-stu-id="a8cac-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="a8cac-113">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="a8cac-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="a8cac-114">此 API 的/v1.0 版本已重命名为*Create groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="a8cac-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="a8cac-115">若要获取在 beta 版中支持的模板及其属性的列表, 请使用[directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。</span><span class="sxs-lookup"><span data-stu-id="a8cac-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="a8cac-116">(对于 v1.0 终结点, 请调用[groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)。)</span><span class="sxs-lookup"><span data-stu-id="a8cac-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="a8cac-117">权限</span><span class="sxs-lookup"><span data-stu-id="a8cac-117">Permissions</span></span>
<span data-ttu-id="a8cac-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8cac-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8cac-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8cac-120">Permission type</span></span>      | <span data-ttu-id="a8cac-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8cac-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8cac-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8cac-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a8cac-123">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8cac-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8cac-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8cac-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8cac-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8cac-125">Not supported.</span></span>    |
|<span data-ttu-id="a8cac-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8cac-126">Application</span></span> | <span data-ttu-id="a8cac-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8cac-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8cac-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8cac-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="a8cac-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8cac-129">Request headers</span></span>
| <span data-ttu-id="a8cac-130">名称</span><span class="sxs-lookup"><span data-stu-id="a8cac-130">Name</span></span>       | <span data-ttu-id="a8cac-131">说明</span><span class="sxs-lookup"><span data-stu-id="a8cac-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8cac-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8cac-132">Authorization</span></span>  | <span data-ttu-id="a8cac-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8cac-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8cac-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8cac-135">Request body</span></span>
<span data-ttu-id="a8cac-136">在请求正文中, 提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8cac-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="a8cac-137">但是, 将根据引用的设置模板名称设置设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a8cac-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="a8cac-138">响应</span><span class="sxs-lookup"><span data-stu-id="a8cac-138">Response</span></span>

<span data-ttu-id="a8cac-139">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8cac-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8cac-140">示例</span><span class="sxs-lookup"><span data-stu-id="a8cac-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8cac-141">请求</span><span class="sxs-lookup"><span data-stu-id="a8cac-141">Request</span></span>
<span data-ttu-id="a8cac-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8cac-142">Here is an example of the request.</span></span>
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
<span data-ttu-id="a8cac-143">在请求正文中, 提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8cac-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a8cac-144">响应</span><span class="sxs-lookup"><span data-stu-id="a8cac-144">Response</span></span>
<span data-ttu-id="a8cac-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8cac-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a8cac-148">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a8cac-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a8cac-149">C#</span><span class="sxs-lookup"><span data-stu-id="a8cac-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directorysetting_from_settings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8cac-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8cac-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directorysetting_from_settings-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a8cac-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="a8cac-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directorysetting_from_settings-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
