---
title: 创建目录设置
description: 根据 directorySettingTemplates 中可用的模板，使用此 API 创建新的设置。 这些设置可以是租户级别，也可以是对象级别（当前仅适用于组）。 创建请求必须为模板中定义的所有设置提供 settingValues。 对于组特定的设置，仅控制是否可以设置组成员是否可以邀请来宾用户的设置。 这样一来，一旦能够将来宾用户添加到组中，就可以控制此行为。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b88e405d8850eef49fd73fff792a94cf727863a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433970"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="dda3e-107">创建目录设置</span><span class="sxs-lookup"><span data-stu-id="dda3e-107">Create a directory setting</span></span>

<span data-ttu-id="dda3e-108">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dda3e-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dda3e-109">根据 directorySettingTemplates 中可用的模板，使用此 API 创建新的设置。</span><span class="sxs-lookup"><span data-stu-id="dda3e-109">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="dda3e-110">这些设置可以是租户级别，也可以是对象级别（当前仅适用于组）。</span><span class="sxs-lookup"><span data-stu-id="dda3e-110">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="dda3e-111">创建请求必须为模板中定义的所有设置提供 settingValues。</span><span class="sxs-lookup"><span data-stu-id="dda3e-111">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="dda3e-112">对于组特定的设置，仅控制是否可以设置组成员是否可以邀请来宾用户的设置。</span><span class="sxs-lookup"><span data-stu-id="dda3e-112">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="dda3e-113">这样一来，一旦能够将来宾用户添加到组中，就可以控制此行为。</span><span class="sxs-lookup"><span data-stu-id="dda3e-113">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="dda3e-114">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="dda3e-114">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="dda3e-115">此 API 的/v1.0 版本已重命名为*Create groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="dda3e-115">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="dda3e-116">若要获取在 beta 版中支持的模板及其属性的列表，请使用[directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。</span><span class="sxs-lookup"><span data-stu-id="dda3e-116">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="dda3e-117">（对于 v1.0 终结点，请调用[groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)。）</span><span class="sxs-lookup"><span data-stu-id="dda3e-117">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="dda3e-118">权限</span><span class="sxs-lookup"><span data-stu-id="dda3e-118">Permissions</span></span>
<span data-ttu-id="dda3e-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dda3e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dda3e-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="dda3e-121">Permission type</span></span>      | <span data-ttu-id="dda3e-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dda3e-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dda3e-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dda3e-123">Delegated (work or school account)</span></span> | <span data-ttu-id="dda3e-124">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dda3e-124">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dda3e-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dda3e-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dda3e-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="dda3e-126">Not supported.</span></span>    |
|<span data-ttu-id="dda3e-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="dda3e-127">Application</span></span> | <span data-ttu-id="dda3e-128">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda3e-128">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dda3e-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dda3e-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="dda3e-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="dda3e-130">Request headers</span></span>
| <span data-ttu-id="dda3e-131">名称</span><span class="sxs-lookup"><span data-stu-id="dda3e-131">Name</span></span>       | <span data-ttu-id="dda3e-132">说明</span><span class="sxs-lookup"><span data-stu-id="dda3e-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dda3e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="dda3e-133">Authorization</span></span>  | <span data-ttu-id="dda3e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dda3e-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dda3e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="dda3e-136">Request body</span></span>
<span data-ttu-id="dda3e-137">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dda3e-137">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="dda3e-138">但是，将根据引用的设置模板名称设置设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dda3e-138">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="dda3e-139">响应</span><span class="sxs-lookup"><span data-stu-id="dda3e-139">Response</span></span>

<span data-ttu-id="dda3e-140">如果成功，此方法在`201 Created`响应正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dda3e-140">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dda3e-141">示例</span><span class="sxs-lookup"><span data-stu-id="dda3e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dda3e-142">请求</span><span class="sxs-lookup"><span data-stu-id="dda3e-142">Request</span></span>
<span data-ttu-id="dda3e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dda3e-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dda3e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dda3e-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dda3e-145">C#</span><span class="sxs-lookup"><span data-stu-id="dda3e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dda3e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dda3e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dda3e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dda3e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dda3e-148">在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dda3e-148">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dda3e-149">响应</span><span class="sxs-lookup"><span data-stu-id="dda3e-149">Response</span></span>
<span data-ttu-id="dda3e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dda3e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
