# <a name="update-calendargroup"></a><span data-ttu-id="49c2c-101">更新 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="49c2c-101">Update calendargroup</span></span>

<span data-ttu-id="49c2c-102">更新 calendargroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49c2c-102">Update the properties of calendargroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49c2c-103">权限</span><span class="sxs-lookup"><span data-stu-id="49c2c-103">Permissions</span></span>
<span data-ttu-id="49c2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="49c2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="49c2c-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="49c2c-106">Permission type</span></span>      | <span data-ttu-id="49c2c-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49c2c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49c2c-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49c2c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="49c2c-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c2c-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="49c2c-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49c2c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49c2c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c2c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="49c2c-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="49c2c-112">Application</span></span> | <span data-ttu-id="49c2c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49c2c-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="49c2c-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49c2c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="49c2c-115">用户的任意 [calendarGroup](../resources/calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="49c2c-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="49c2c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="49c2c-116">Request headers</span></span>
| <span data-ttu-id="49c2c-117">标头</span><span class="sxs-lookup"><span data-stu-id="49c2c-117">Header</span></span>       | <span data-ttu-id="49c2c-118">值</span><span class="sxs-lookup"><span data-stu-id="49c2c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="49c2c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="49c2c-119">Authorization</span></span>  | <span data-ttu-id="49c2c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49c2c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49c2c-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49c2c-122">Content-Type</span></span>  | <span data-ttu-id="49c2c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="49c2c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49c2c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49c2c-125">Request body</span></span>
<span data-ttu-id="49c2c-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="49c2c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="49c2c-129">属性</span><span class="sxs-lookup"><span data-stu-id="49c2c-129">Property</span></span>     | <span data-ttu-id="49c2c-130">类型</span><span class="sxs-lookup"><span data-stu-id="49c2c-130">Type</span></span>   |<span data-ttu-id="49c2c-131">说明</span><span class="sxs-lookup"><span data-stu-id="49c2c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49c2c-132">名称</span><span class="sxs-lookup"><span data-stu-id="49c2c-132">name</span></span>|<span data-ttu-id="49c2c-133">String</span><span class="sxs-lookup"><span data-stu-id="49c2c-133">String</span></span>|<span data-ttu-id="49c2c-134">组名称。</span><span class="sxs-lookup"><span data-stu-id="49c2c-134">The group name.</span></span>|

## <a name="response"></a><span data-ttu-id="49c2c-135">响应</span><span class="sxs-lookup"><span data-stu-id="49c2c-135">Response</span></span>

<span data-ttu-id="49c2c-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [calendarGroup](../resources/calendargroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49c2c-136">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49c2c-137">示例</span><span class="sxs-lookup"><span data-stu-id="49c2c-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49c2c-138">请求</span><span class="sxs-lookup"><span data-stu-id="49c2c-138">Request</span></span>
<span data-ttu-id="49c2c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49c2c-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
##### <a name="response"></a><span data-ttu-id="49c2c-140">响应</span><span class="sxs-lookup"><span data-stu-id="49c2c-140">Response</span></span>
<span data-ttu-id="49c2c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49c2c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
