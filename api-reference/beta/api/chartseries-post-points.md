---
title: 创建 ChartPoints
description: 使用此 API 创建新 ChartPoints。
ms.openlocfilehash: be10973510b053b30178a3c5b35a866f828bf927
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041690"
---
# <a name="create-chartpoints"></a><span data-ttu-id="5e202-103">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="5e202-103">Create ChartPoints</span></span>

> <span data-ttu-id="5e202-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e202-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e202-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e202-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e202-106">使用此 API 创建新 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="5e202-106">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e202-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e202-107">Permissions</span></span>
<span data-ttu-id="5e202-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e202-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e202-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e202-110">Permission type</span></span>      | <span data-ttu-id="5e202-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e202-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e202-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e202-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e202-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e202-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e202-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e202-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e202-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e202-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5e202-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e202-116">Application</span></span> | <span data-ttu-id="5e202-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e202-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e202-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e202-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="5e202-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e202-119">Request headers</span></span>
| <span data-ttu-id="5e202-120">名称</span><span class="sxs-lookup"><span data-stu-id="5e202-120">Name</span></span>       | <span data-ttu-id="5e202-121">说明</span><span class="sxs-lookup"><span data-stu-id="5e202-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5e202-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e202-122">Authorization</span></span>  | <span data-ttu-id="5e202-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e202-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e202-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5e202-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5e202-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5e202-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e202-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e202-128">Request body</span></span>
<span data-ttu-id="5e202-129">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e202-129">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e202-130">响应</span><span class="sxs-lookup"><span data-stu-id="5e202-130">Response</span></span>

<span data-ttu-id="5e202-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [ChartPoints](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e202-131">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e202-132">示例</span><span class="sxs-lookup"><span data-stu-id="5e202-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e202-133">请求</span><span class="sxs-lookup"><span data-stu-id="5e202-133">Request</span></span>
<span data-ttu-id="5e202-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e202-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="5e202-135">在请求正文中，提供 [ChartPoints](../resources/chartpoint.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e202-135">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5e202-136">响应</span><span class="sxs-lookup"><span data-stu-id="5e202-136">Response</span></span>
<span data-ttu-id="5e202-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e202-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->