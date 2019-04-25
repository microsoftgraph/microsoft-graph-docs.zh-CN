---
title: 创建组设置
description: 根据 groupSettingTemplates 中可用的模板, 使用此 API 创建新的设置。 这些设置可以是租户级别, 也可以是组级别。 创建请求必须为模板中定义的所有设置提供 settingValues。 对于组特定的设置, 仅控制是否可以设置组成员是否可以邀请来宾用户的设置。 这样一来, 一旦能够将来宾用户添加到组中, 就可以控制此行为。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e87e34f5816818c25cef5768c08ab8f7c73a3a0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577796"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="4aa32-107">创建组设置</span><span class="sxs-lookup"><span data-stu-id="4aa32-107">Create a group setting</span></span>

<span data-ttu-id="4aa32-p102">根据 [groupSettingTemplates](../resources/groupsettingtemplate.md) 中提供的模板，使用此 API 创建新设置。这些设置可设置为租户级别或组级别。创建请求必须为模板中定义的所有设置提供 [settingValues](../resources/settingvalue.md)。对于组特定设置，仅可以设置管理组成员是否可以邀请来宾用户的设置。通常将来宾用户添加到群组的功能可用后，该操作将管理此行为。</span><span class="sxs-lookup"><span data-stu-id="4aa32-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="4aa32-113">若要获取其在 v1.0 中支持的模板及其属性的列表, 请使用[groupSettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)(对于 beta 终结点, 调用[directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。)</span><span class="sxs-lookup"><span data-stu-id="4aa32-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa32-114">权限</span><span class="sxs-lookup"><span data-stu-id="4aa32-114">Permissions</span></span>

<span data-ttu-id="4aa32-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aa32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4aa32-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aa32-117">Permission type</span></span>      | <span data-ttu-id="4aa32-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aa32-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aa32-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa32-119">Delegated (work or school account)</span></span> | <span data-ttu-id="4aa32-120">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4aa32-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4aa32-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aa32-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aa32-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aa32-122">Not supported.</span></span>    |
|<span data-ttu-id="4aa32-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aa32-123">Application</span></span> | <span data-ttu-id="4aa32-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aa32-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aa32-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aa32-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="4aa32-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aa32-126">Request headers</span></span>

| <span data-ttu-id="4aa32-127">名称</span><span class="sxs-lookup"><span data-stu-id="4aa32-127">Name</span></span> | <span data-ttu-id="4aa32-128">说明</span><span class="sxs-lookup"><span data-stu-id="4aa32-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4aa32-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aa32-129">Authorization</span></span> | <span data-ttu-id="4aa32-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aa32-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4aa32-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aa32-132">Content-Type</span></span> | <span data-ttu-id="4aa32-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4aa32-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aa32-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aa32-134">Request body</span></span>
<span data-ttu-id="4aa32-p105">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。但是，设置的显示名称将根据引用的设置模板名称进行设置。</span><span class="sxs-lookup"><span data-stu-id="4aa32-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="4aa32-137">响应</span><span class="sxs-lookup"><span data-stu-id="4aa32-137">Response</span></span>

<span data-ttu-id="4aa32-138">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4aa32-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aa32-139">示例</span><span class="sxs-lookup"><span data-stu-id="4aa32-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4aa32-140">请求</span><span class="sxs-lookup"><span data-stu-id="4aa32-140">Request</span></span>

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
<span data-ttu-id="4aa32-141">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aa32-141">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4aa32-142">响应</span><span class="sxs-lookup"><span data-stu-id="4aa32-142">Response</span></span>

<span data-ttu-id="4aa32-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4aa32-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
