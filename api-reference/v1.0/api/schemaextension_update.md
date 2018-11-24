# <a name="update-schemaextension"></a><span data-ttu-id="e334b-101">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e334b-101">Update schemaExtension</span></span>

<span data-ttu-id="e334b-102">更新指定 [schemaExtension](../resources/schemaextension.md) 的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="e334b-102">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="e334b-p101">此更新适用于该扩展的 **targetTypes** 属性中包含的所有资源。这些资源属于[支持的资源类型](../../../concepts/extensibility_overview.md#supported-resources)。</span><span class="sxs-lookup"><span data-stu-id="e334b-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="e334b-p102">仅在该扩展处于 **InDevelopment** 或 **Available** 状态时创建架构扩展的应用（所有者应用）可以对扩展进行增量更新。这表示该应用无法删除定义中的自定义属性或目标资源类型。但是此应用可以更改扩展说明。</span><span class="sxs-lookup"><span data-stu-id="e334b-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="e334b-108">权限</span><span class="sxs-lookup"><span data-stu-id="e334b-108">Permissions</span></span>
<span data-ttu-id="e334b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e334b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e334b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e334b-111">Permission type</span></span>      | <span data-ttu-id="e334b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e334b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e334b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e334b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e334b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e334b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e334b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e334b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e334b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e334b-116">Not supported.</span></span>    |
|<span data-ttu-id="e334b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e334b-117">Application</span></span> | <span data-ttu-id="e334b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e334b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e334b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e334b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="e334b-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e334b-120">Optional request headers</span></span>

| <span data-ttu-id="e334b-121">名称</span><span class="sxs-lookup"><span data-stu-id="e334b-121">Name</span></span>      |<span data-ttu-id="e334b-122">说明</span><span class="sxs-lookup"><span data-stu-id="e334b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e334b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e334b-123">Authorization</span></span>  | <span data-ttu-id="e334b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e334b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e334b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e334b-126">Content-Type</span></span>   | <span data-ttu-id="e334b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e334b-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e334b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e334b-128">Request body</span></span>

<span data-ttu-id="e334b-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e334b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e334b-132">属性</span><span class="sxs-lookup"><span data-stu-id="e334b-132">Property</span></span>   | <span data-ttu-id="e334b-133">类型</span><span class="sxs-lookup"><span data-stu-id="e334b-133">Type</span></span> |<span data-ttu-id="e334b-134">说明</span><span class="sxs-lookup"><span data-stu-id="e334b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e334b-135">说明</span><span class="sxs-lookup"><span data-stu-id="e334b-135">description</span></span>|<span data-ttu-id="e334b-136">String</span><span class="sxs-lookup"><span data-stu-id="e334b-136">String</span></span>|<span data-ttu-id="e334b-137">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="e334b-137">Description for the schema extension.</span></span>|
|<span data-ttu-id="e334b-138">properties</span><span class="sxs-lookup"><span data-stu-id="e334b-138">properties</span></span>|<span data-ttu-id="e334b-139">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e334b-139">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="e334b-p106">构成架构扩展定义的属性名称和类型的集合。仅允许增量更改。</span><span class="sxs-lookup"><span data-stu-id="e334b-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="e334b-142">status</span><span class="sxs-lookup"><span data-stu-id="e334b-142">status</span></span>|<span data-ttu-id="e334b-143">String</span><span class="sxs-lookup"><span data-stu-id="e334b-143">String</span></span>|<span data-ttu-id="e334b-144">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="e334b-144">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="e334b-145">在创建时的初始状态是**InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="e334b-145">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="e334b-146">可能的状态切换为**InDevelopment**到**有空**和到**已否决**的**有空**。</span><span class="sxs-lookup"><span data-stu-id="e334b-146">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="e334b-147">targetTypes</span><span class="sxs-lookup"><span data-stu-id="e334b-147">targetTypes</span></span>|<span data-ttu-id="e334b-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e334b-148">String collection</span></span>|<span data-ttu-id="e334b-p108">架构扩展适用的支持扩展的 Microsoft Graph 类型集。仅允许增量更改。</span><span class="sxs-lookup"><span data-stu-id="e334b-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="e334b-151">响应</span><span class="sxs-lookup"><span data-stu-id="e334b-151">Response</span></span>

<span data-ttu-id="e334b-152">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e334b-152">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e334b-153">示例</span><span class="sxs-lookup"><span data-stu-id="e334b-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e334b-154">请求</span><span class="sxs-lookup"><span data-stu-id="e334b-154">Request</span></span>

<span data-ttu-id="e334b-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e334b-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a><span data-ttu-id="e334b-156">响应</span><span class="sxs-lookup"><span data-stu-id="e334b-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="e334b-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e334b-157">See also</span></span>

- [<span data-ttu-id="e334b-158">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e334b-158">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e334b-159">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e334b-159">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->