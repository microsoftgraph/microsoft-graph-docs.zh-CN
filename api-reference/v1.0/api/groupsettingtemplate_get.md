# <a name="get-a-group-setting-template"></a><span data-ttu-id="97f64-101">获取组设置模板</span><span class="sxs-lookup"><span data-stu-id="97f64-101">Get a group setting template</span></span>

<span data-ttu-id="97f64-p101">组设置模板表示用于在租户内创建设置的设置模板。此操作允许检索 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象的属性，包括可用设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="97f64-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="97f64-104">权限</span><span class="sxs-lookup"><span data-stu-id="97f64-104">Permissions</span></span>

<span data-ttu-id="97f64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="97f64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="97f64-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="97f64-107">Permission type</span></span>      | <span data-ttu-id="97f64-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97f64-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="97f64-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97f64-109">Delegated (work or school account)</span></span> | <span data-ttu-id="97f64-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97f64-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="97f64-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97f64-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f64-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="97f64-112">Not supported.</span></span>    | 
|<span data-ttu-id="97f64-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="97f64-113">Application</span></span> | <span data-ttu-id="97f64-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97f64-114">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="97f64-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97f64-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97f64-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97f64-116">Optional query parameters</span></span>
<span data-ttu-id="97f64-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97f64-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97f64-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="97f64-118">Request headers</span></span>
| <span data-ttu-id="97f64-119">名称</span><span class="sxs-lookup"><span data-stu-id="97f64-119">Name</span></span> | <span data-ttu-id="97f64-120">说明</span><span class="sxs-lookup"><span data-stu-id="97f64-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="97f64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f64-121">Authorization</span></span> | <span data-ttu-id="97f64-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97f64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97f64-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="97f64-124">Request body</span></span>
<span data-ttu-id="97f64-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97f64-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97f64-126">响应</span><span class="sxs-lookup"><span data-stu-id="97f64-126">Response</span></span>

<span data-ttu-id="97f64-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97f64-127">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97f64-128">示例</span><span class="sxs-lookup"><span data-stu-id="97f64-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97f64-129">请求</span><span class="sxs-lookup"><span data-stu-id="97f64-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="97f64-130">响应</span><span class="sxs-lookup"><span data-stu-id="97f64-130">Response</span></span>

<span data-ttu-id="97f64-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97f64-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->