# <a name="create-a-group-setting"></a><span data-ttu-id="3a6a8-101">创建组设置</span><span class="sxs-lookup"><span data-stu-id="3a6a8-101">Create a group setting</span></span>

<span data-ttu-id="3a6a8-p101">根据 [groupSettingTemplates](../resources/groupsettingtemplate.md) 中提供的模板，使用此 API 创建新设置。这些设置可设置为租户级别或组级别。创建请求必须为模板中定义的所有设置提供 [settingValues](../resources/settingvalue.md)。对于组特定设置，仅可以设置管理组成员是否可以邀请来宾用户的设置。通常将来宾用户添加到群组的功能可用后，该操作将管理此行为。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="3a6a8-107">对于 v1.0 中支持的模板和属性列表，使用[groupSettingTemplate 查询](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)（对于 beta 终结点，调用[directorySettingTemplates](https://developer.microsoft.com/en-us/graph/graph-explorer?request=directorySettingTemplates&version=beta)。）</span><span class="sxs-lookup"><span data-stu-id="3a6a8-107">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/en-us/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="3a6a8-108">权限</span><span class="sxs-lookup"><span data-stu-id="3a6a8-108">Permissions</span></span>

<span data-ttu-id="3a6a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3a6a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a6a8-111">Permission type</span></span>      | <span data-ttu-id="3a6a8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a6a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a6a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a6a8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a6a8-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a6a8-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a6a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a6a8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a6a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-116">Not supported.</span></span>    |
|<span data-ttu-id="3a6a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a6a8-117">Application</span></span> | <span data-ttu-id="3a6a8-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a6a8-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a6a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a6a8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="3a6a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a6a8-120">Request headers</span></span>

| <span data-ttu-id="3a6a8-121">名称</span><span class="sxs-lookup"><span data-stu-id="3a6a8-121">Name</span></span> | <span data-ttu-id="3a6a8-122">说明</span><span class="sxs-lookup"><span data-stu-id="3a6a8-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3a6a8-123">授权</span><span class="sxs-lookup"><span data-stu-id="3a6a8-123">Authorization</span></span> | <span data-ttu-id="3a6a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a6a8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a6a8-126">Content-Type</span></span> | <span data-ttu-id="3a6a8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3a6a8-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a6a8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a6a8-128">Request body</span></span>
<span data-ttu-id="3a6a8-p104">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。但是，设置的显示名称将根据引用的设置模板名称进行设置。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="3a6a8-131">响应</span><span class="sxs-lookup"><span data-stu-id="3a6a8-131">Response</span></span>

<span data-ttu-id="3a6a8-132">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-132">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a6a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="3a6a8-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3a6a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="3a6a8-134">Request</span></span>

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
<span data-ttu-id="3a6a8-135">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-135">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3a6a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="3a6a8-136">Response</span></span>

<span data-ttu-id="3a6a8-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a6a8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
