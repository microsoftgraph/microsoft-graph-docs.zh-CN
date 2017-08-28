# <a name="get-a-group-setting"></a><span data-ttu-id="d9484-101">获取组设置</span><span class="sxs-lookup"><span data-stu-id="d9484-101">Get a group setting</span></span>

<span data-ttu-id="d9484-102">检索特定组设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9484-102">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9484-103">权限</span><span class="sxs-lookup"><span data-stu-id="d9484-103">Permissions</span></span>

<span data-ttu-id="d9484-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d9484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="d9484-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9484-106">Permission type</span></span>      | <span data-ttu-id="d9484-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9484-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9484-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9484-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d9484-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9484-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9484-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9484-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9484-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9484-111">Not supported.</span></span>    |
|<span data-ttu-id="d9484-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9484-112">Application</span></span> | <span data-ttu-id="d9484-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9484-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9484-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9484-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="d9484-115">获取特定租户范围或组设置。</span><span class="sxs-lookup"><span data-stu-id="d9484-115">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9484-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9484-116">Optional query parameters</span></span>
<span data-ttu-id="d9484-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d9484-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="d9484-118">注意：不支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="d9484-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9484-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9484-119">Request headers</span></span>
| <span data-ttu-id="d9484-120">名称</span><span class="sxs-lookup"><span data-stu-id="d9484-120">Name</span></span> | <span data-ttu-id="d9484-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9484-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="d9484-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9484-122">Authorization</span></span> | <span data-ttu-id="d9484-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d9484-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9484-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9484-125">Request body</span></span>

<span data-ttu-id="d9484-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9484-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9484-127">响应</span><span class="sxs-lookup"><span data-stu-id="d9484-127">Response</span></span>

<span data-ttu-id="d9484-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9484-128">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9484-129">示例</span><span class="sxs-lookup"><span data-stu-id="d9484-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9484-130">请求</span><span class="sxs-lookup"><span data-stu-id="d9484-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="d9484-131">响应</span><span class="sxs-lookup"><span data-stu-id="d9484-131">Response</span></span>

<span data-ttu-id="d9484-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9484-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

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
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->