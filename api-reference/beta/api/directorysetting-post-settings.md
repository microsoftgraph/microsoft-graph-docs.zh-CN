---
title: 创建一个目录设置
description: 使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。 这些设置可以在租户级别或在对象级别 (当前只能针对组)。 创建请求必须提供 settingValues 模板中定义的所有设置。 对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。 能够向组添加来宾用户通常可用后，这将控制此行为。
ms.openlocfilehash: 40e90f66c43032deea8ee866b13508fd73c0f17f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043903"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="1ee18-107">创建一个目录设置</span><span class="sxs-lookup"><span data-stu-id="1ee18-107">Create a directory setting</span></span>

> <span data-ttu-id="1ee18-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1ee18-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ee18-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1ee18-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ee18-110">使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。</span><span class="sxs-lookup"><span data-stu-id="1ee18-110">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="1ee18-111">这些设置可以在租户级别或在对象级别 (当前只能针对组)。</span><span class="sxs-lookup"><span data-stu-id="1ee18-111">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="1ee18-112">创建请求必须提供 settingValues 模板中定义的所有设置。</span><span class="sxs-lookup"><span data-stu-id="1ee18-112">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="1ee18-113">对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。</span><span class="sxs-lookup"><span data-stu-id="1ee18-113">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="1ee18-114">能够向组添加来宾用户通常可用后，这将控制此行为。</span><span class="sxs-lookup"><span data-stu-id="1ee18-114">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="1ee18-115">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="1ee18-115">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="1ee18-116">此 API 的 /v1.0 版本已被重命名为*创建 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="1ee18-116">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="1ee18-117">有关模板和它们支持 beta 中的属性的列表，使用[directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。</span><span class="sxs-lookup"><span data-stu-id="1ee18-117">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="1ee18-118">（对于 v1.0 终结点，呼叫[groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)。）</span><span class="sxs-lookup"><span data-stu-id="1ee18-118">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="1ee18-119">权限</span><span class="sxs-lookup"><span data-stu-id="1ee18-119">Permissions</span></span>
<span data-ttu-id="1ee18-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ee18-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee18-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ee18-122">Permission type</span></span>      | <span data-ttu-id="1ee18-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ee18-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ee18-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee18-124">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee18-125">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ee18-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ee18-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee18-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee18-127">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee18-127">Not supported.</span></span>    |
|<span data-ttu-id="1ee18-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ee18-128">Application</span></span> | <span data-ttu-id="1ee18-129">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee18-129">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee18-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ee18-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="1ee18-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ee18-131">Request headers</span></span>
| <span data-ttu-id="1ee18-132">名称</span><span class="sxs-lookup"><span data-stu-id="1ee18-132">Name</span></span>       | <span data-ttu-id="1ee18-133">说明</span><span class="sxs-lookup"><span data-stu-id="1ee18-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ee18-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ee18-134">Authorization</span></span>  | <span data-ttu-id="1ee18-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ee18-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ee18-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ee18-137">Request body</span></span>
<span data-ttu-id="1ee18-138">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ee18-138">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="1ee18-139">但是，设置的显示名称将被设置基于在引用的设置模板名称。</span><span class="sxs-lookup"><span data-stu-id="1ee18-139">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="1ee18-140">响应</span><span class="sxs-lookup"><span data-stu-id="1ee18-140">Response</span></span>

<span data-ttu-id="1ee18-141">如果成功，此方法返回`201 Created`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1ee18-141">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee18-142">示例</span><span class="sxs-lookup"><span data-stu-id="1ee18-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ee18-143">请求</span><span class="sxs-lookup"><span data-stu-id="1ee18-143">Request</span></span>
<span data-ttu-id="1ee18-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ee18-144">Here is an example of the request.</span></span>
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
<span data-ttu-id="1ee18-145">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ee18-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ee18-146">响应</span><span class="sxs-lookup"><span data-stu-id="1ee18-146">Response</span></span>
<span data-ttu-id="1ee18-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ee18-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->