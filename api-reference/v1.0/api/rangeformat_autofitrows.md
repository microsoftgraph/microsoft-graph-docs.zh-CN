# <a name="rangeformat-autofitrows"></a><span data-ttu-id="5eb50-101">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="5eb50-101">RangeFormat: autofitRows</span></span>

<span data-ttu-id="5eb50-102">根据列中的当前数据，更改当前范围的行高以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="5eb50-102">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="5eb50-103">权限</span><span class="sxs-lookup"><span data-stu-id="5eb50-103">Permissions</span></span>
<span data-ttu-id="5eb50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5eb50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5eb50-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eb50-106">Permission type</span></span>      | <span data-ttu-id="5eb50-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eb50-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eb50-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eb50-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5eb50-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eb50-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5eb50-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eb50-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eb50-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eb50-111">Not supported.</span></span>    |
|<span data-ttu-id="5eb50-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="5eb50-112">Application</span></span> | <span data-ttu-id="5eb50-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5eb50-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eb50-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5eb50-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(<address>)/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="5eb50-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="5eb50-115">Request headers</span></span>
| <span data-ttu-id="5eb50-116">名称</span><span class="sxs-lookup"><span data-stu-id="5eb50-116">Name</span></span>       | <span data-ttu-id="5eb50-117">说明</span><span class="sxs-lookup"><span data-stu-id="5eb50-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5eb50-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eb50-118">Authorization</span></span>  | <span data-ttu-id="5eb50-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5eb50-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eb50-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="5eb50-121">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5eb50-122">响应</span><span class="sxs-lookup"><span data-stu-id="5eb50-122">Response</span></span>

<span data-ttu-id="5eb50-p103">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5eb50-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb50-125">示例</span><span class="sxs-lookup"><span data-stu-id="5eb50-125">Example</span></span>
<span data-ttu-id="5eb50-126">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5eb50-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5eb50-127">请求</span><span class="sxs-lookup"><span data-stu-id="5eb50-127">Request</span></span>
<span data-ttu-id="5eb50-128">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5eb50-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="5eb50-129">响应</span><span class="sxs-lookup"><span data-stu-id="5eb50-129">Response</span></span>
<span data-ttu-id="5eb50-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5eb50-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->