---
title: NamedItem：Range
description: 返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。
localization_priority: Normal
ms.openlocfilehash: 283eadbe423fad415534bb4e355f7926e24628be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540362"
---
# <a name="nameditem-range"></a><span data-ttu-id="df97b-104">NamedItem：Range</span><span class="sxs-lookup"><span data-stu-id="df97b-104">NamedItem: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df97b-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="df97b-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="df97b-107">权限</span><span class="sxs-lookup"><span data-stu-id="df97b-107">Permissions</span></span>
<span data-ttu-id="df97b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df97b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df97b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="df97b-110">Permission type</span></span>      | <span data-ttu-id="df97b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df97b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df97b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df97b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="df97b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df97b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df97b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df97b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df97b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df97b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df97b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="df97b-116">Application</span></span> | <span data-ttu-id="df97b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df97b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df97b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df97b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/Range

```
## <a name="request-headers"></a><span data-ttu-id="df97b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="df97b-119">Request headers</span></span>
| <span data-ttu-id="df97b-120">名称</span><span class="sxs-lookup"><span data-stu-id="df97b-120">Name</span></span>       | <span data-ttu-id="df97b-121">说明</span><span class="sxs-lookup"><span data-stu-id="df97b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="df97b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df97b-122">Authorization</span></span>  | <span data-ttu-id="df97b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df97b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df97b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="df97b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="df97b-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="df97b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df97b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="df97b-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="df97b-129">响应</span><span class="sxs-lookup"><span data-stu-id="df97b-129">Response</span></span>

<span data-ttu-id="df97b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df97b-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df97b-131">示例</span><span class="sxs-lookup"><span data-stu-id="df97b-131">Example</span></span>
<span data-ttu-id="df97b-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="df97b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="df97b-133">请求</span><span class="sxs-lookup"><span data-stu-id="df97b-133">Request</span></span>
<span data-ttu-id="df97b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df97b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/Range
```

##### <a name="response"></a><span data-ttu-id="df97b-135">响应</span><span class="sxs-lookup"><span data-stu-id="df97b-135">Response</span></span>
<span data-ttu-id="df97b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df97b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-range.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
