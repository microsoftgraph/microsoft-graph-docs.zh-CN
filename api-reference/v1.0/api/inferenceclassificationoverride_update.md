# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="78f97-101">更新 inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="78f97-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="78f97-102">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="78f97-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="78f97-103">不能在 [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) 示例中使用 PATCH 更改任何其他字段。</span><span class="sxs-lookup"><span data-stu-id="78f97-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="78f97-104">如果发件人的替代存在，并且发件人更改了他/她的显示名称，可以使用 [POST](inferenceclassification_post_overrides.md) 强制更新现有替代中的名称字段。</span><span class="sxs-lookup"><span data-stu-id="78f97-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="78f97-105">如果发件人的替代存在，并且发件人更改了他/她的 SMTP 地址，“更新”此发件人的替代的唯一方法是：[删除](inferenceclassificationoverride_delete.md) 现有替代，然后使用新的 SMTP 地址 [创建](inferenceclassification_post_overrides.md) 新替代。</span><span class="sxs-lookup"><span data-stu-id="78f97-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78f97-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="78f97-106">Prerequisites</span></span>
<span data-ttu-id="78f97-107">要执行此 API，需要以下**范围**：*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="78f97-107">The following **scopes** are required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="78f97-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78f97-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="78f97-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="78f97-109">Request headers</span></span>
| <span data-ttu-id="78f97-110">名称</span><span class="sxs-lookup"><span data-stu-id="78f97-110">Name</span></span>       | <span data-ttu-id="78f97-111">类型</span><span class="sxs-lookup"><span data-stu-id="78f97-111">Type</span></span> | <span data-ttu-id="78f97-112">说明</span><span class="sxs-lookup"><span data-stu-id="78f97-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78f97-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f97-113">Authorization</span></span>  | <span data-ttu-id="78f97-114">string</span><span class="sxs-lookup"><span data-stu-id="78f97-114">string</span></span>  | <span data-ttu-id="78f97-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78f97-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78f97-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78f97-117">Content-Type</span></span> | <span data-ttu-id="78f97-118">string</span><span class="sxs-lookup"><span data-stu-id="78f97-118">string</span></span>  | <span data-ttu-id="78f97-p102">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="78f97-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78f97-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="78f97-121">Request body</span></span>
<span data-ttu-id="78f97-p103">在请求正文中，提供 **classifyAs** 的新值。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="78f97-p103">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="78f97-124">属性</span><span class="sxs-lookup"><span data-stu-id="78f97-124">Property</span></span>     | <span data-ttu-id="78f97-125">类型</span><span class="sxs-lookup"><span data-stu-id="78f97-125">Type</span></span>   |<span data-ttu-id="78f97-126">说明</span><span class="sxs-lookup"><span data-stu-id="78f97-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f97-127">classifyAs</span><span class="sxs-lookup"><span data-stu-id="78f97-127">classifyAs</span></span>|<span data-ttu-id="78f97-128">string</span><span class="sxs-lookup"><span data-stu-id="78f97-128">string</span></span>| <span data-ttu-id="78f97-p104">指定始终应如何对来自特定发件人的传入邮件进行分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="78f97-p104">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="78f97-131">响应</span><span class="sxs-lookup"><span data-stu-id="78f97-131">Response</span></span>

<span data-ttu-id="78f97-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78f97-132">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78f97-133">示例</span><span class="sxs-lookup"><span data-stu-id="78f97-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78f97-134">请求</span><span class="sxs-lookup"><span data-stu-id="78f97-134">Request</span></span>
<span data-ttu-id="78f97-135">以下示例将 SMTP 地址 randiw@adatum.onmicrosoft.com 的替代从 `other` 更改为 `focused`。</span><span class="sxs-lookup"><span data-stu-id="78f97-135">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="78f97-136">响应</span><span class="sxs-lookup"><span data-stu-id="78f97-136">Response</span></span>
<span data-ttu-id="78f97-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78f97-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->