# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="61bff-101">删除 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="61bff-101">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="61bff-102">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="61bff-102">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="61bff-103">权限</span><span class="sxs-lookup"><span data-stu-id="61bff-103">Permissions</span></span>
<span data-ttu-id="61bff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="61bff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61bff-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="61bff-106">Permission type</span></span>      | <span data-ttu-id="61bff-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61bff-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="61bff-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61bff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="61bff-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61bff-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="61bff-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61bff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61bff-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61bff-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="61bff-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="61bff-112">Application</span></span> | <span data-ttu-id="61bff-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="61bff-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61bff-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61bff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="61bff-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="61bff-115">Request headers</span></span>
| <span data-ttu-id="61bff-116">名称</span><span class="sxs-lookup"><span data-stu-id="61bff-116">Name</span></span>       | <span data-ttu-id="61bff-117">类型</span><span class="sxs-lookup"><span data-stu-id="61bff-117">Type</span></span> | <span data-ttu-id="61bff-118">说明</span><span class="sxs-lookup"><span data-stu-id="61bff-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61bff-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="61bff-119">Authorization</span></span>  | <span data-ttu-id="61bff-120">string</span><span class="sxs-lookup"><span data-stu-id="61bff-120">string</span></span>  | <span data-ttu-id="61bff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61bff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61bff-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="61bff-123">Request body</span></span>
<span data-ttu-id="61bff-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="61bff-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61bff-125">响应</span><span class="sxs-lookup"><span data-stu-id="61bff-125">Response</span></span>

<span data-ttu-id="61bff-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="61bff-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61bff-128">示例</span><span class="sxs-lookup"><span data-stu-id="61bff-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61bff-129">请求</span><span class="sxs-lookup"><span data-stu-id="61bff-129">Request</span></span>
<span data-ttu-id="61bff-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="61bff-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="61bff-131">响应</span><span class="sxs-lookup"><span data-stu-id="61bff-131">Response</span></span>
<span data-ttu-id="61bff-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="61bff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->