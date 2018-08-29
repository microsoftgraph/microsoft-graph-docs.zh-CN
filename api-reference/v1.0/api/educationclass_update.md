# <a name="update-educationclass-properties"></a><span data-ttu-id="498ab-101">更新 educationclass 属性</span><span class="sxs-lookup"><span data-stu-id="498ab-101">Update educationclass properties</span></span>

<span data-ttu-id="498ab-102">更新课程属性。</span><span class="sxs-lookup"><span data-stu-id="498ab-102">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="498ab-103">权限</span><span class="sxs-lookup"><span data-stu-id="498ab-103">Permissions</span></span>
<span data-ttu-id="498ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="498ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="498ab-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="498ab-106">Permission type</span></span>      | <span data-ttu-id="498ab-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="498ab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="498ab-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="498ab-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="498ab-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="498ab-109">Not supported.</span></span>  |
|<span data-ttu-id="498ab-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="498ab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="498ab-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="498ab-111">Not supported.</span></span>   |
|<span data-ttu-id="498ab-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="498ab-112">Application</span></span> | <span data-ttu-id="498ab-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="498ab-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="498ab-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="498ab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="498ab-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="498ab-115">Request headers</span></span>
| <span data-ttu-id="498ab-116">标头</span><span class="sxs-lookup"><span data-stu-id="498ab-116">Header</span></span>       | <span data-ttu-id="498ab-117">值</span><span class="sxs-lookup"><span data-stu-id="498ab-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="498ab-118">授权</span><span class="sxs-lookup"><span data-stu-id="498ab-118">Authorization</span></span>  | <span data-ttu-id="498ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="498ab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="498ab-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="498ab-121">Content-Type</span></span>  | <span data-ttu-id="498ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="498ab-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="498ab-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="498ab-123">Request body</span></span>
<span data-ttu-id="498ab-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="498ab-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="498ab-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="498ab-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="498ab-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="498ab-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="498ab-127">属性</span><span class="sxs-lookup"><span data-stu-id="498ab-127">Property</span></span>     | <span data-ttu-id="498ab-128">类型</span><span class="sxs-lookup"><span data-stu-id="498ab-128">Type</span></span>   |<span data-ttu-id="498ab-129">说明</span><span class="sxs-lookup"><span data-stu-id="498ab-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="498ab-130">说明</span><span class="sxs-lookup"><span data-stu-id="498ab-130">description</span></span>|<span data-ttu-id="498ab-131">String</span><span class="sxs-lookup"><span data-stu-id="498ab-131">String</span></span>| <span data-ttu-id="498ab-132">课程说明。</span><span class="sxs-lookup"><span data-stu-id="498ab-132">Description of the class.</span></span>|
|<span data-ttu-id="498ab-133">displayName</span><span class="sxs-lookup"><span data-stu-id="498ab-133">displayName</span></span>|<span data-ttu-id="498ab-134">String</span><span class="sxs-lookup"><span data-stu-id="498ab-134">String</span></span>| <span data-ttu-id="498ab-135">课程名称。</span><span class="sxs-lookup"><span data-stu-id="498ab-135">Name of the class.</span></span>|
|<span data-ttu-id="498ab-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="498ab-136">mailNickname</span></span>|<span data-ttu-id="498ab-137">String</span><span class="sxs-lookup"><span data-stu-id="498ab-137">String</span></span>| <span data-ttu-id="498ab-138">用于向所有用户发送电子邮件的电子邮件别名（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="498ab-138">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="498ab-139"><!-- Please verify the revised description here. --> |classCode|String| 由学校使用的课程代码。| |externalId|String| 来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="498ab-139"><!-- Please verify the revised description here. -->|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="498ab-140">| |externalName|String|同步系统中的课程名称。| |externalSource|string| 此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="498ab-140">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="498ab-141">可取值为：`sis`、`manual`、`enum_sentinel`。|</span><span class="sxs-lookup"><span data-stu-id="498ab-141">The possible values are , , , , , , , , , , , or .</span></span>

## <a name="response"></a><span data-ttu-id="498ab-142">响应</span><span class="sxs-lookup"><span data-stu-id="498ab-142">Response</span></span>
<span data-ttu-id="498ab-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="498ab-143">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="498ab-144">示例</span><span class="sxs-lookup"><span data-stu-id="498ab-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="498ab-145">请求</span><span class="sxs-lookup"><span data-stu-id="498ab-145">Request</span></span>
<span data-ttu-id="498ab-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="498ab-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="498ab-147">响应</span><span class="sxs-lookup"><span data-stu-id="498ab-147">Response</span></span>
<span data-ttu-id="498ab-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="498ab-148">The following is an example of the response.</span></span> 

><span data-ttu-id="498ab-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="498ab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->