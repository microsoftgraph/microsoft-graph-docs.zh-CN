---
title: 'workbookRangeView: range'
description: 返回与 rangeView 资源相关联的范围。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8c116a80e01c0b649ff1846de3e324874e7dd837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863418"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="cd1d0-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="cd1d0-103">workbookRangeView: range</span></span>

> <span data-ttu-id="cd1d0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd1d0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd1d0-106">返回与 rangeView 资源相关联的范围。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-106">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd1d0-107">权限</span><span class="sxs-lookup"><span data-stu-id="cd1d0-107">Permissions</span></span>
<span data-ttu-id="cd1d0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd1d0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd1d0-110">Permission type</span></span>      | <span data-ttu-id="cd1d0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd1d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd1d0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd1d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd1d0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd1d0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd1d0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd1d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd1d0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd1d0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cd1d0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd1d0-116">Application</span></span> | <span data-ttu-id="cd1d0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd1d0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd1d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="cd1d0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd1d0-119">Request headers</span></span>
| <span data-ttu-id="cd1d0-120">名称</span><span class="sxs-lookup"><span data-stu-id="cd1d0-120">Name</span></span>       | <span data-ttu-id="cd1d0-121">说明</span><span class="sxs-lookup"><span data-stu-id="cd1d0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd1d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd1d0-122">Authorization</span></span>  | <span data-ttu-id="cd1d0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd1d0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd1d0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd1d0-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd1d0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd1d0-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cd1d0-129">响应</span><span class="sxs-lookup"><span data-stu-id="cd1d0-129">Response</span></span>

<span data-ttu-id="cd1d0-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-130">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd1d0-131">示例</span><span class="sxs-lookup"><span data-stu-id="cd1d0-131">Example</span></span>
<span data-ttu-id="cd1d0-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cd1d0-133">请求</span><span class="sxs-lookup"><span data-stu-id="cd1d0-133">Request</span></span>
<span data-ttu-id="cd1d0-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="cd1d0-135">响应</span><span class="sxs-lookup"><span data-stu-id="cd1d0-135">Response</span></span>
<span data-ttu-id="cd1d0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd1d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
