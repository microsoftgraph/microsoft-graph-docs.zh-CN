# <a name="create-a-group-setting"></a><span data-ttu-id="00187-101">创建组设置</span><span class="sxs-lookup"><span data-stu-id="00187-101">Create a group setting</span></span>

<span data-ttu-id="00187-p101">根据 [groupSettingTemplates](../resources/groupsettingtemplate.md) 中提供的模板，使用此 API 创建新设置。这些设置可设置为租户级别或组级别。创建请求必须为模板中定义的所有设置提供 [settingValues](../resources/settingvalue.md)。对于组特定设置，仅可以设置管理组成员是否可以邀请来宾用户的设置。通常将来宾用户添加到群组的功能可用后，该操作将管理此行为。</span><span class="sxs-lookup"><span data-stu-id="00187-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

## <a name="permissions"></a><span data-ttu-id="00187-107">权限</span><span class="sxs-lookup"><span data-stu-id="00187-107">Permissions</span></span>

<span data-ttu-id="00187-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="00187-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="00187-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00187-110">Permission type</span></span>      | <span data-ttu-id="00187-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00187-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00187-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00187-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00187-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="00187-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00187-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00187-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00187-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00187-115">Not supported.</span></span>    |
|<span data-ttu-id="00187-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00187-116">Application</span></span> | <span data-ttu-id="00187-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00187-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00187-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00187-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="00187-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00187-119">Request headers</span></span>

| <span data-ttu-id="00187-120">名称</span><span class="sxs-lookup"><span data-stu-id="00187-120">Name</span></span> | <span data-ttu-id="00187-121">说明</span><span class="sxs-lookup"><span data-stu-id="00187-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="00187-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00187-122">Authorization</span></span> | <span data-ttu-id="00187-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00187-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00187-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00187-125">Content-Type</span></span> | <span data-ttu-id="00187-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00187-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="00187-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00187-127">Request body</span></span>
<span data-ttu-id="00187-p104">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。但是，设置的显示名称将根据引用的设置模板名称进行设置。</span><span class="sxs-lookup"><span data-stu-id="00187-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="00187-130">响应</span><span class="sxs-lookup"><span data-stu-id="00187-130">Response</span></span>

<span data-ttu-id="00187-131">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00187-131">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00187-132">示例</span><span class="sxs-lookup"><span data-stu-id="00187-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="00187-133">请求</span><span class="sxs-lookup"><span data-stu-id="00187-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="00187-134">在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00187-134">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="00187-135">响应</span><span class="sxs-lookup"><span data-stu-id="00187-135">Response</span></span>

<span data-ttu-id="00187-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00187-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "groupSetting": {
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