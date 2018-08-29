# <a name="update-outlook-category"></a><span data-ttu-id="f9929-101">更新 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="f9929-101">Update Outlook category</span></span>


<span data-ttu-id="f9929-102">更新指定 [outlookCategory](../resources/outlookCategory.md) 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="f9929-102">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span> <span data-ttu-id="f9929-103">创建类别后，不能修改 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="f9929-103">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9929-104">权限</span><span class="sxs-lookup"><span data-stu-id="f9929-104">Permissions</span></span>
<span data-ttu-id="f9929-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f9929-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9929-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9929-107">Permission type</span></span>      | <span data-ttu-id="f9929-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9929-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9929-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9929-109">Delegated (work or school account)</span></span> | <span data-ttu-id="f9929-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9929-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f9929-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9929-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9929-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9929-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f9929-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9929-113">Application</span></span> | <span data-ttu-id="f9929-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9929-114">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9929-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9929-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9929-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9929-116">Optional query parameters</span></span>
<span data-ttu-id="f9929-117">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9929-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9929-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9929-118">Request headers</span></span>
| <span data-ttu-id="f9929-119">名称</span><span class="sxs-lookup"><span data-stu-id="f9929-119">Name</span></span>      |<span data-ttu-id="f9929-120">说明</span><span class="sxs-lookup"><span data-stu-id="f9929-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9929-121">授权</span><span class="sxs-lookup"><span data-stu-id="f9929-121">Authorization</span></span>  | <span data-ttu-id="f9929-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9929-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9929-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9929-124">Request body</span></span>
<span data-ttu-id="f9929-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f9929-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f9929-128">属性</span><span class="sxs-lookup"><span data-stu-id="f9929-128">Property</span></span>     | <span data-ttu-id="f9929-129">类型</span><span class="sxs-lookup"><span data-stu-id="f9929-129">Type</span></span>   |<span data-ttu-id="f9929-130">说明</span><span class="sxs-lookup"><span data-stu-id="f9929-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9929-131">color</span><span class="sxs-lookup"><span data-stu-id="f9929-131">color</span></span>|<span data-ttu-id="f9929-132">String</span><span class="sxs-lookup"><span data-stu-id="f9929-132">String</span></span>|<span data-ttu-id="f9929-133">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="f9929-133">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="f9929-134">响应</span><span class="sxs-lookup"><span data-stu-id="f9929-134">Response</span></span>

<span data-ttu-id="f9929-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [outlookCategory](../resources/outlookCategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9929-135">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9929-136">示例</span><span class="sxs-lookup"><span data-stu-id="f9929-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9929-137">请求</span><span class="sxs-lookup"><span data-stu-id="f9929-137">Request</span></span>
<span data-ttu-id="f9929-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9929-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["bac262b7-485d-4739-b436-e31467d64fac"],
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="f9929-139">响应</span><span class="sxs-lookup"><span data-stu-id="f9929-139">Response</span></span>
<span data-ttu-id="f9929-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9929-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->