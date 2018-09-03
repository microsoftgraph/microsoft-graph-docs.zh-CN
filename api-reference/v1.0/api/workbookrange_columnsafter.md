# <a name="workbookrange-columnsafter"></a><span data-ttu-id="06dcc-101">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="06dcc-101">workbookRange: columnsAfter</span></span>

<span data-ttu-id="06dcc-102">获取给定范围右侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="06dcc-102">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="06dcc-103">权限</span><span class="sxs-lookup"><span data-stu-id="06dcc-103">Permissions</span></span>
<span data-ttu-id="06dcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="06dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06dcc-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="06dcc-106">Permission type</span></span>      | <span data-ttu-id="06dcc-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06dcc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06dcc-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06dcc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="06dcc-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06dcc-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="06dcc-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06dcc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06dcc-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="06dcc-111">Not supported.</span></span>    |
|<span data-ttu-id="06dcc-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="06dcc-112">Application</span></span> | <span data-ttu-id="06dcc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="06dcc-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06dcc-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06dcc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="06dcc-115">函数参数</span><span class="sxs-lookup"><span data-stu-id="06dcc-115">Function parameters</span></span>

| <span data-ttu-id="06dcc-116">参数</span><span class="sxs-lookup"><span data-stu-id="06dcc-116">Parameter</span></span>    | <span data-ttu-id="06dcc-117">类型</span><span class="sxs-lookup"><span data-stu-id="06dcc-117">Type</span></span>   |<span data-ttu-id="06dcc-118">说明</span><span class="sxs-lookup"><span data-stu-id="06dcc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06dcc-119">计数</span><span class="sxs-lookup"><span data-stu-id="06dcc-119">count</span></span>|<span data-ttu-id="06dcc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="06dcc-120">Int32</span></span>|<span data-ttu-id="06dcc-121">可选。</span><span class="sxs-lookup"><span data-stu-id="06dcc-121">Optional.</span></span> <span data-ttu-id="06dcc-122">生成的范围中要包含的列数。</span><span class="sxs-lookup"><span data-stu-id="06dcc-122">The number of rows to include in the resulting range.</span></span> <span data-ttu-id="06dcc-123">一般来说，使用正数可以在当前区域之外创建一个区域。</span><span class="sxs-lookup"><span data-stu-id="06dcc-123">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="06dcc-124">也可以使用负数在当前区域之内创建一个区域。</span><span class="sxs-lookup"><span data-stu-id="06dcc-124">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="06dcc-125">默认值为 1</span><span class="sxs-lookup"><span data-stu-id="06dcc-125">The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="06dcc-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="06dcc-126">Request headers</span></span>
| <span data-ttu-id="06dcc-127">名称</span><span class="sxs-lookup"><span data-stu-id="06dcc-127">Name</span></span>       | <span data-ttu-id="06dcc-128">说明</span><span class="sxs-lookup"><span data-stu-id="06dcc-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="06dcc-129">授权</span><span class="sxs-lookup"><span data-stu-id="06dcc-129">Authorization</span></span>  | <span data-ttu-id="06dcc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06dcc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="06dcc-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="06dcc-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="06dcc-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="06dcc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06dcc-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="06dcc-135">Request body</span></span>
<span data-ttu-id="06dcc-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06dcc-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06dcc-137">响应</span><span class="sxs-lookup"><span data-stu-id="06dcc-137">Response</span></span>
<span data-ttu-id="06dcc-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06dcc-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06dcc-139">示例</span><span class="sxs-lookup"><span data-stu-id="06dcc-139">Example</span></span>
<span data-ttu-id="06dcc-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="06dcc-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06dcc-141">请求</span><span class="sxs-lookup"><span data-stu-id="06dcc-141">Request</span></span>
<span data-ttu-id="06dcc-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06dcc-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="06dcc-143">响应</span><span class="sxs-lookup"><span data-stu-id="06dcc-143">Response</span></span>
<span data-ttu-id="06dcc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06dcc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
