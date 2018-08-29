# <a name="get-educationclass"></a><span data-ttu-id="968de-101">获取 educationClass</span><span class="sxs-lookup"><span data-stu-id="968de-101">Get educationClass</span></span>

<span data-ttu-id="968de-102">从系统检索课程。</span><span class="sxs-lookup"><span data-stu-id="968de-102">Retrieve a class from the system.</span></span> <span data-ttu-id="968de-103">课程是带特殊属性的通用组，向系统表明该组是课程。</span><span class="sxs-lookup"><span data-stu-id="968de-103">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="968de-104">组成员表示学生；组管理员代表课程教师。</span><span class="sxs-lookup"><span data-stu-id="968de-104">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="968de-105">如果使用的是委派令牌，用户只会看到他们作为成员的课程。</span><span class="sxs-lookup"><span data-stu-id="968de-105">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="968de-106">权限</span><span class="sxs-lookup"><span data-stu-id="968de-106">Permissions</span></span>
<span data-ttu-id="968de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="968de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="968de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="968de-109">Permission type</span></span>      | <span data-ttu-id="968de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="968de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="968de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="968de-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="968de-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="968de-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="968de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="968de-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="968de-114">不支持</span><span class="sxs-lookup"><span data-stu-id="968de-114">Not supported</span></span>  |
|<span data-ttu-id="968de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="968de-115">Application</span></span> | <span data-ttu-id="968de-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="968de-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="968de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="968de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="968de-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="968de-118">Optional query parameters</span></span>
<span data-ttu-id="968de-119">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="968de-119">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="968de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="968de-120">Request headers</span></span>
| <span data-ttu-id="968de-121">标头</span><span class="sxs-lookup"><span data-stu-id="968de-121">Header</span></span>       | <span data-ttu-id="968de-122">值</span><span class="sxs-lookup"><span data-stu-id="968de-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="968de-123">授权</span><span class="sxs-lookup"><span data-stu-id="968de-123">Authorization</span></span>  | <span data-ttu-id="968de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="968de-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="968de-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="968de-126">Request body</span></span>
<span data-ttu-id="968de-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="968de-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="968de-128">响应</span><span class="sxs-lookup"><span data-stu-id="968de-128">Response</span></span>
<span data-ttu-id="968de-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="968de-129">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="968de-130">示例</span><span class="sxs-lookup"><span data-stu-id="968de-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="968de-131">请求</span><span class="sxs-lookup"><span data-stu-id="968de-131">Request</span></span>
<span data-ttu-id="968de-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="968de-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
##### <a name="response"></a><span data-ttu-id="968de-133">响应</span><span class="sxs-lookup"><span data-stu-id="968de-133">Response</span></span>
<span data-ttu-id="968de-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="968de-134">The following is an example of the response.</span></span> 

><span data-ttu-id="968de-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="968de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->