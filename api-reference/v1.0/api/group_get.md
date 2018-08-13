# <a name="get-group"></a><span data-ttu-id="70733-101">获取组</span><span class="sxs-lookup"><span data-stu-id="70733-101">Get group</span></span>
<span data-ttu-id="70733-102">获取组对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="70733-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="70733-103">默认属性</span><span class="sxs-lookup"><span data-stu-id="70733-103">Default properties</span></span>

<span data-ttu-id="70733-p101">下面展示了在获取或列出组时返回的一组默认属性。这些默认属性是所有可用属性中的一部分。</span><span class="sxs-lookup"><span data-stu-id="70733-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="70733-106">说明</span><span class="sxs-lookup"><span data-stu-id="70733-106">description</span></span>
* <span data-ttu-id="70733-107">displayName</span><span class="sxs-lookup"><span data-stu-id="70733-107">displayName</span></span>
* <span data-ttu-id="70733-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="70733-108">groupTypes</span></span>
* <span data-ttu-id="70733-109">id</span><span class="sxs-lookup"><span data-stu-id="70733-109">id</span></span>
* <span data-ttu-id="70733-110">mail</span><span class="sxs-lookup"><span data-stu-id="70733-110">mail</span></span>
* <span data-ttu-id="70733-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="70733-111">mailEnabled</span></span>
* <span data-ttu-id="70733-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="70733-112">mailNickname</span></span>
* <span data-ttu-id="70733-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="70733-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="70733-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="70733-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="70733-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="70733-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="70733-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="70733-116">proxyAddresses</span></span>
* <span data-ttu-id="70733-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="70733-117">securityEnabled</span></span>
* <span data-ttu-id="70733-118">visibility</span><span class="sxs-lookup"><span data-stu-id="70733-118">visibility</span></span>

<span data-ttu-id="70733-119">默认情况下，不返回下列组属性：</span><span class="sxs-lookup"><span data-stu-id="70733-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="70733-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="70733-120">allowExternalSenders</span></span>
* <span data-ttu-id="70733-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="70733-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="70733-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="70733-122">isSubscribedByMail</span></span>
* <span data-ttu-id="70733-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="70733-123">unseenCount</span></span>

<span data-ttu-id="70733-p102">若要获取这些属性，请使用 **$select** 查询参数。示例如下：</span><span class="sxs-lookup"><span data-stu-id="70733-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="70733-126">权限</span><span class="sxs-lookup"><span data-stu-id="70733-126">Permissions</span></span>
<span data-ttu-id="70733-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="70733-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70733-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="70733-129">Permission type</span></span>      | <span data-ttu-id="70733-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70733-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70733-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70733-131">Delegated (work or school account)</span></span> | <span data-ttu-id="70733-132">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70733-132">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="70733-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70733-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70733-134">不支持。</span><span class="sxs-lookup"><span data-stu-id="70733-134">Not supported.</span></span>    |
|<span data-ttu-id="70733-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="70733-135">Application</span></span> | <span data-ttu-id="70733-136">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70733-136">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70733-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70733-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70733-138">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70733-138">Optional query parameters</span></span>
<span data-ttu-id="70733-139">此方法支持 [OData 查询参数](../../../concepts/query_parameters.md) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="70733-139">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70733-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="70733-140">Request headers</span></span>
| <span data-ttu-id="70733-141">名称</span><span class="sxs-lookup"><span data-stu-id="70733-141">Name</span></span>       | <span data-ttu-id="70733-142">类型</span><span class="sxs-lookup"><span data-stu-id="70733-142">Type</span></span> | <span data-ttu-id="70733-143">说明</span><span class="sxs-lookup"><span data-stu-id="70733-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70733-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="70733-144">Authorization</span></span>  | <span data-ttu-id="70733-145">string</span><span class="sxs-lookup"><span data-stu-id="70733-145">string</span></span>  | <span data-ttu-id="70733-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70733-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70733-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="70733-148">Request body</span></span>
<span data-ttu-id="70733-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70733-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70733-150">响应</span><span class="sxs-lookup"><span data-stu-id="70733-150">Response</span></span>
<span data-ttu-id="70733-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70733-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70733-152">示例</span><span class="sxs-lookup"><span data-stu-id="70733-152">Example</span></span>
#### <a name="request"></a><span data-ttu-id="70733-153">请求</span><span class="sxs-lookup"><span data-stu-id="70733-153">Request</span></span>
<span data-ttu-id="70733-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70733-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="70733-155">响应</span><span class="sxs-lookup"><span data-stu-id="70733-155">Response</span></span>
<span data-ttu-id="70733-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="70733-156">The following is an example of the response.</span></span>

><span data-ttu-id="70733-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70733-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="70733-158">如上所述，默认属性将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="70733-158">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
