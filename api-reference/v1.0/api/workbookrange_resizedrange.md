# <a name="workbookrange-resizedrange"></a><span data-ttu-id="2f661-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="2f661-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="2f661-102">获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。</span><span class="sxs-lookup"><span data-stu-id="2f661-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f661-103">权限</span><span class="sxs-lookup"><span data-stu-id="2f661-103">Permissions</span></span>
<span data-ttu-id="2f661-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2f661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f661-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f661-106">Permission type</span></span>      | <span data-ttu-id="2f661-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f661-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f661-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f661-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2f661-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f661-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2f661-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f661-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f661-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f661-111">Not supported.</span></span>    |
|<span data-ttu-id="2f661-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f661-112">Application</span></span> | <span data-ttu-id="2f661-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f661-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f661-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f661-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="2f661-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f661-115">Request headers</span></span>
| <span data-ttu-id="2f661-116">名称</span><span class="sxs-lookup"><span data-stu-id="2f661-116">Name</span></span>       | <span data-ttu-id="2f661-117">说明</span><span class="sxs-lookup"><span data-stu-id="2f661-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f661-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f661-118">Authorization</span></span>  | <span data-ttu-id="2f661-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f661-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f661-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2f661-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2f661-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2f661-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="2f661-124">参数</span><span class="sxs-lookup"><span data-stu-id="2f661-124">Parameters</span></span>

| <span data-ttu-id="2f661-125">参数</span><span class="sxs-lookup"><span data-stu-id="2f661-125">Parameter</span></span>    | <span data-ttu-id="2f661-126">类型</span><span class="sxs-lookup"><span data-stu-id="2f661-126">Type</span></span>   |<span data-ttu-id="2f661-127">说明</span><span class="sxs-lookup"><span data-stu-id="2f661-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f661-128">deltarows</span><span class="sxs-lookup"><span data-stu-id="2f661-128">deltarows</span></span>|<span data-ttu-id="2f661-129">Int32</span><span class="sxs-lookup"><span data-stu-id="2f661-129">Int32</span></span>|<span data-ttu-id="2f661-p104">相对于当前范围，右下角展开的行数。使用正数可展开范围，使用负数可合拢范围</span><span class="sxs-lookup"><span data-stu-id="2f661-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="2f661-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="2f661-132">deltaColumns</span></span>|<span data-ttu-id="2f661-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2f661-133">Int32</span></span>|<span data-ttu-id="2f661-p105">相对于当前范围，右下角展开的列数。使用正数可展开范围，使用负数可合拢范围。</span><span class="sxs-lookup"><span data-stu-id="2f661-p105">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f661-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f661-136">Request body</span></span>
<span data-ttu-id="2f661-137">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="2f661-137">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="2f661-138">参数</span><span class="sxs-lookup"><span data-stu-id="2f661-138">Parameter</span></span>    | <span data-ttu-id="2f661-139">类型</span><span class="sxs-lookup"><span data-stu-id="2f661-139">Type</span></span>   |<span data-ttu-id="2f661-140">说明</span><span class="sxs-lookup"><span data-stu-id="2f661-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f661-141">deltaRows</span><span class="sxs-lookup"><span data-stu-id="2f661-141">deltaRows</span></span>|<span data-ttu-id="2f661-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2f661-142">Int32</span></span>||
|<span data-ttu-id="2f661-143">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="2f661-143">deltaColumns</span></span>|<span data-ttu-id="2f661-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2f661-144">Int32</span></span>||

### <a name="response"></a><span data-ttu-id="2f661-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f661-145">Response</span></span>
<span data-ttu-id="2f661-146">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f661-146">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f661-147">示例</span><span class="sxs-lookup"><span data-stu-id="2f661-147">Example</span></span>
<span data-ttu-id="2f661-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2f661-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f661-149">请求</span><span class="sxs-lookup"><span data-stu-id="2f661-149">Request</span></span>
<span data-ttu-id="2f661-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f661-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="2f661-151">响应</span><span class="sxs-lookup"><span data-stu-id="2f661-151">Response</span></span>
<span data-ttu-id="2f661-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f661-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
