# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="81f2f-101">**列出由用户拥有的已删除项目**</span><span class="sxs-lookup"><span data-stu-id="81f2f-101">Added **List deleted items owned by a user** action to directory (deleted items) resource</span></span>

<span data-ttu-id="81f2f-102">检索由指定用户拥有的最近已删除项目。</span><span class="sxs-lookup"><span data-stu-id="81f2f-102">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="81f2f-103">目前，列出已删除项目功能仅支持用户所拥有的 [group](../resources/group.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="81f2f-103">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="81f2f-104">这是服务操作，这意味着它不支持分页。</span><span class="sxs-lookup"><span data-stu-id="81f2f-104">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="81f2f-105">API 返回多达 1,000 个由用户删除的对象，它们按 ID 排序。</span><span class="sxs-lookup"><span data-stu-id="81f2f-105">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="81f2f-106">权限</span><span class="sxs-lookup"><span data-stu-id="81f2f-106">Permissions</span></span>

<span data-ttu-id="81f2f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="81f2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="81f2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="81f2f-109">Permission type</span></span> | <span data-ttu-id="81f2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81f2f-110">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="81f2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81f2f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81f2f-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f2f-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="81f2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81f2f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="81f2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="81f2f-114">Not supported.</span></span> |
| <span data-ttu-id="81f2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="81f2f-115">Application</span></span> | <span data-ttu-id="81f2f-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f2f-116">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="81f2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81f2f-117">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="81f2f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="81f2f-118">Request headers</span></span>

| <span data-ttu-id="81f2f-119">名称</span><span class="sxs-lookup"><span data-stu-id="81f2f-119">Name</span></span>          | <span data-ttu-id="81f2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="81f2f-120">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="81f2f-121">授权</span><span class="sxs-lookup"><span data-stu-id="81f2f-121">Authorization</span></span> | <span data-ttu-id="81f2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81f2f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81f2f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="81f2f-124">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="81f2f-125">请求正文需要以下参数：</span><span class="sxs-lookup"><span data-stu-id="81f2f-125">The request body can contain the following parameters.</span></span>

| <span data-ttu-id="81f2f-126">参数</span><span class="sxs-lookup"><span data-stu-id="81f2f-126">Parameter</span></span>    | <span data-ttu-id="81f2f-127">类型</span><span class="sxs-lookup"><span data-stu-id="81f2f-127">Type</span></span> |<span data-ttu-id="81f2f-128">说明</span><span class="sxs-lookup"><span data-stu-id="81f2f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81f2f-129">userId</span><span class="sxs-lookup"><span data-stu-id="81f2f-129">userId</span></span>|<span data-ttu-id="81f2f-130">字符串</span><span class="sxs-lookup"><span data-stu-id="81f2f-130">String</span></span>|<span data-ttu-id="81f2f-131">所有者的 ID。</span><span class="sxs-lookup"><span data-stu-id="81f2f-131">ID of the owner.</span></span>|
|<span data-ttu-id="81f2f-132">type</span><span class="sxs-lookup"><span data-stu-id="81f2f-132">type</span></span>|<span data-ttu-id="81f2f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="81f2f-133">String</span></span>|<span data-ttu-id="81f2f-134">要返回对象的类型；`Group` 是目前唯一受支持的值。</span><span class="sxs-lookup"><span data-stu-id="81f2f-134">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="81f2f-135">响应</span><span class="sxs-lookup"><span data-stu-id="81f2f-135">Response</span></span>

<span data-ttu-id="81f2f-136">成功的请求返回 `200 OK` 响应代码；响应对象包含 [directory（已删除项）](../resources/directory.md)属性。</span><span class="sxs-lookup"><span data-stu-id="81f2f-136">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="81f2f-137">示例</span><span class="sxs-lookup"><span data-stu-id="81f2f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81f2f-138">请求</span><span class="sxs-lookup"><span data-stu-id="81f2f-138">Request</span></span>

<span data-ttu-id="81f2f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81f2f-139">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="81f2f-140">响应</span><span class="sxs-lookup"><span data-stu-id="81f2f-140">Response</span></span>

<span data-ttu-id="81f2f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81f2f-141">Here is an example of the response.</span></span> <span data-ttu-id="81f2f-142">注意：为了简单起见，此响应对象可能被截断。</span><span class="sxs-lookup"><span data-stu-id="81f2f-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="81f2f-143">从实际的调用返回所有支持的属性。</span><span class="sxs-lookup"><span data-stu-id="81f2f-143">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


