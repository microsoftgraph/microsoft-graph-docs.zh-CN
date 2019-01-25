---
title: 创建一个目录设置
description: 使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。 这些设置可以在租户级别或在对象级别 (当前只能针对组)。 创建请求必须提供 settingValues 模板中定义的所有设置。 对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。 能够向组添加来宾用户通常可用后，这将控制此行为。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f74c449f02726adc4ba0993f450a8a4351ec8f2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520751"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="0f1d9-107">创建一个目录设置</span><span class="sxs-lookup"><span data-stu-id="0f1d9-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f1d9-108">使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="0f1d9-109">这些设置可以在租户级别或在对象级别 (当前只能针对组)。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="0f1d9-110">创建请求必须提供 settingValues 模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="0f1d9-111">对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="0f1d9-112">能够向组添加来宾用户通常可用后，这将控制此行为。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="0f1d9-113">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0f1d9-114">此 API 的 /v1.0 版本已被重命名为*创建 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="0f1d9-115">有关模板和它们支持 beta 中的属性的列表，使用[directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="0f1d9-116">（对于 v1.0 终结点，呼叫[groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)。）</span><span class="sxs-lookup"><span data-stu-id="0f1d9-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="0f1d9-117">权限</span><span class="sxs-lookup"><span data-stu-id="0f1d9-117">Permissions</span></span>
<span data-ttu-id="0f1d9-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f1d9-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f1d9-120">Permission type</span></span>      | <span data-ttu-id="0f1d9-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f1d9-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f1d9-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f1d9-122">Delegated (work or school account)</span></span> | <span data-ttu-id="0f1d9-123">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0f1d9-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f1d9-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f1d9-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f1d9-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-125">Not supported.</span></span>    |
|<span data-ttu-id="0f1d9-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f1d9-126">Application</span></span> | <span data-ttu-id="0f1d9-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f1d9-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f1d9-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f1d9-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="0f1d9-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f1d9-129">Request headers</span></span>
| <span data-ttu-id="0f1d9-130">名称</span><span class="sxs-lookup"><span data-stu-id="0f1d9-130">Name</span></span>       | <span data-ttu-id="0f1d9-131">说明</span><span class="sxs-lookup"><span data-stu-id="0f1d9-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0f1d9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f1d9-132">Authorization</span></span>  | <span data-ttu-id="0f1d9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f1d9-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f1d9-135">Request body</span></span>
<span data-ttu-id="0f1d9-136">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="0f1d9-137">但是，设置的显示名称将被设置基于在引用的设置模板名称。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="0f1d9-138">响应</span><span class="sxs-lookup"><span data-stu-id="0f1d9-138">Response</span></span>

<span data-ttu-id="0f1d9-139">如果成功，此方法返回`201 Created`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f1d9-140">示例</span><span class="sxs-lookup"><span data-stu-id="0f1d9-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f1d9-141">请求</span><span class="sxs-lookup"><span data-stu-id="0f1d9-141">Request</span></span>
<span data-ttu-id="0f1d9-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-142">Here is an example of the request.</span></span>
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
<span data-ttu-id="0f1d9-143">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0f1d9-144">响应</span><span class="sxs-lookup"><span data-stu-id="0f1d9-144">Response</span></span>
<span data-ttu-id="0f1d9-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f1d9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
