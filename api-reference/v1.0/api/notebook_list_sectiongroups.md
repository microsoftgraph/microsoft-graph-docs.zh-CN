# <a name="list-sectiongroups"></a><span data-ttu-id="b8a39-101">列出 sectionGroups</span><span class="sxs-lookup"><span data-stu-id="b8a39-101">List sectionGroups</span></span>

<span data-ttu-id="b8a39-102">从指定笔记本中检索[分区组](../resources/sectiongroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="b8a39-102">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8a39-103">权限</span><span class="sxs-lookup"><span data-stu-id="b8a39-103">Permissions</span></span>
<span data-ttu-id="b8a39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b8a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8a39-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8a39-106">Permission type</span></span>      | <span data-ttu-id="b8a39-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8a39-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b8a39-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8a39-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b8a39-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a39-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b8a39-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8a39-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8a39-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8a39-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="b8a39-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8a39-112">Application</span></span> | <span data-ttu-id="b8a39-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a39-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8a39-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8a39-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8a39-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b8a39-115">Optional query parameters</span></span>
<span data-ttu-id="b8a39-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b8a39-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b8a39-117">默认排序顺序是 `name asc`。</span><span class="sxs-lookup"><span data-stu-id="b8a39-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="b8a39-p102">默认查询展开 `parentNotebook`，并选择其 `id`、`displayName` 和 `self` 属性。分区组的有效 `expand` 值为 `sections`、`sectionGroups`、`parentNotebook` 和 `parentSectionGroup`。</span><span class="sxs-lookup"><span data-stu-id="b8a39-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8a39-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8a39-120">Request headers</span></span>
| <span data-ttu-id="b8a39-121">名称</span><span class="sxs-lookup"><span data-stu-id="b8a39-121">Name</span></span>       | <span data-ttu-id="b8a39-122">类型</span><span class="sxs-lookup"><span data-stu-id="b8a39-122">Type</span></span> | <span data-ttu-id="b8a39-123">说明</span><span class="sxs-lookup"><span data-stu-id="b8a39-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8a39-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8a39-124">Authorization</span></span>  | <span data-ttu-id="b8a39-125">string</span><span class="sxs-lookup"><span data-stu-id="b8a39-125">string</span></span>  | <span data-ttu-id="b8a39-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8a39-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8a39-128">接受</span><span class="sxs-lookup"><span data-stu-id="b8a39-128">Accept</span></span> | <span data-ttu-id="b8a39-129">string</span><span class="sxs-lookup"><span data-stu-id="b8a39-129">string</span></span> | `application/json` |  

## <a name="request-body"></a><span data-ttu-id="b8a39-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8a39-130">Request body</span></span>
<span data-ttu-id="b8a39-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b8a39-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8a39-132">响应</span><span class="sxs-lookup"><span data-stu-id="b8a39-132">Response</span></span>

<span data-ttu-id="b8a39-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sectionGroup](../resources/sectiongroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b8a39-133">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8a39-134">示例</span><span class="sxs-lookup"><span data-stu-id="b8a39-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8a39-135">请求</span><span class="sxs-lookup"><span data-stu-id="b8a39-135">Request</span></span>
<span data-ttu-id="b8a39-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8a39-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="b8a39-137">响应</span><span class="sxs-lookup"><span data-stu-id="b8a39-137">Response</span></span>
<span data-ttu-id="b8a39-p104">下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8a39-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "displayName": "name-value",
      "createdBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "lastModifiedBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
       }
     }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
