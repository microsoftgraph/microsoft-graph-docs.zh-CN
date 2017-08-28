# <a name="list-groupsettingtemplates"></a><span data-ttu-id="a1496-101">List groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="a1496-101">List groupSettingTemplates</span></span>

<span data-ttu-id="a1496-p101">组设置模板表示一组模板，用于创建组设置并在租户内使用。此操作将检索可用 groupSettingTemplates 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a1496-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1496-104">权限</span><span class="sxs-lookup"><span data-stu-id="a1496-104">Permissions</span></span>

<span data-ttu-id="a1496-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1496-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a1496-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1496-107">Permission type</span></span>      | <span data-ttu-id="a1496-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1496-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1496-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1496-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a1496-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1496-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1496-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1496-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1496-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1496-112">Not supported.</span></span>    |
|<span data-ttu-id="a1496-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1496-113">Application</span></span> | <span data-ttu-id="a1496-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1496-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1496-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1496-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a1496-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1496-116">Optional query parameters</span></span>
<span data-ttu-id="a1496-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1496-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="a1496-118">**注意：**不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="a1496-118">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1496-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1496-119">Request headers</span></span>
| <span data-ttu-id="a1496-120">名称</span><span class="sxs-lookup"><span data-stu-id="a1496-120">Name</span></span> | <span data-ttu-id="a1496-121">说明</span><span class="sxs-lookup"><span data-stu-id="a1496-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a1496-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1496-122">Authorization</span></span>  | <span data-ttu-id="a1496-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1496-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1496-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1496-125">Request body</span></span>
<span data-ttu-id="a1496-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1496-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1496-127">响应</span><span class="sxs-lookup"><span data-stu-id="a1496-127">Response</span></span>

<span data-ttu-id="a1496-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSettingTemplate](../resources/groupsettingtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a1496-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1496-129">示例</span><span class="sxs-lookup"><span data-stu-id="a1496-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1496-130">请求</span><span class="sxs-lookup"><span data-stu-id="a1496-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="a1496-131">响应</span><span class="sxs-lookup"><span data-stu-id="a1496-131">Response</span></span>

<span data-ttu-id="a1496-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1496-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
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
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->