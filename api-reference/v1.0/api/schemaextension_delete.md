# <a name="delete-schemaextension"></a><span data-ttu-id="e2bb4-101">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e2bb4-101">Delete schemaExtension</span></span>

<span data-ttu-id="e2bb4-102">删除[架构扩展](../resources/schemaExtension.md)定义。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-102">Delete the definition of a [schema extension](../resources/schemaExtension.md).</span></span>

<span data-ttu-id="e2bb4-p101">仅创建架构扩展的应用（所有者应用）可以删除架构扩展定义，并且仅在该扩展处于 **InDevelopment** 状态下时才可以将其删除。删除架构扩展定义不会影响访问基于此定义已添加到资源实例的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="e2bb4-105">权限</span><span class="sxs-lookup"><span data-stu-id="e2bb4-105">Permissions</span></span>
<span data-ttu-id="e2bb4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e2bb4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2bb4-108">Permission type</span></span>      | <span data-ttu-id="e2bb4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2bb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2bb4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2bb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2bb4-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2bb4-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2bb4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2bb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2bb4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-113">Not supported.</span></span>    |
|<span data-ttu-id="e2bb4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2bb4-114">Application</span></span> | <span data-ttu-id="e2bb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2bb4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2bb4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e2bb4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2bb4-117">Request headers</span></span>
| <span data-ttu-id="e2bb4-118">名称</span><span class="sxs-lookup"><span data-stu-id="e2bb4-118">Name</span></span>      |<span data-ttu-id="e2bb4-119">说明</span><span class="sxs-lookup"><span data-stu-id="e2bb4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e2bb4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2bb4-120">Authorization</span></span>  | <span data-ttu-id="e2bb4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2bb4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2bb4-123">Request body</span></span>
<span data-ttu-id="e2bb4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2bb4-125">响应</span><span class="sxs-lookup"><span data-stu-id="e2bb4-125">Response</span></span>

<span data-ttu-id="e2bb4-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2bb4-128">示例</span><span class="sxs-lookup"><span data-stu-id="e2bb4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2bb4-129">请求</span><span class="sxs-lookup"><span data-stu-id="e2bb4-129">Request</span></span>
<span data-ttu-id="e2bb4-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="e2bb4-131">响应</span><span class="sxs-lookup"><span data-stu-id="e2bb4-131">Response</span></span>
<span data-ttu-id="e2bb4-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e2bb4-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="e2bb4-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e2bb4-133">See also</span></span>

- [<span data-ttu-id="e2bb4-134">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e2bb4-134">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e2bb4-135">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e2bb4-135">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->