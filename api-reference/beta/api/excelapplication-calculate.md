---
title: 应用程序： 计算
description: 重新计算 Excel 中当前打开的所有工作簿。
localization_priority: Normal
ms.openlocfilehash: 3d80fc89c002d7c89fcc5d68920895b9b1fe1c4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818331"
---
# <a name="application-calculate"></a><span data-ttu-id="99dcb-103">应用程序： 计算</span><span class="sxs-lookup"><span data-stu-id="99dcb-103">Application: calculate</span></span>

> <span data-ttu-id="99dcb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99dcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99dcb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99dcb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99dcb-106">重新计算 Excel 中当前打开的所有工作簿。</span><span class="sxs-lookup"><span data-stu-id="99dcb-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="99dcb-107">权限</span><span class="sxs-lookup"><span data-stu-id="99dcb-107">Permissions</span></span>
<span data-ttu-id="99dcb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99dcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99dcb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="99dcb-110">Permission type</span></span>      | <span data-ttu-id="99dcb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99dcb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99dcb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99dcb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99dcb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="99dcb-113">Not supported.</span></span>    |
|<span data-ttu-id="99dcb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99dcb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99dcb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="99dcb-115">Not supported.</span></span>    |
|<span data-ttu-id="99dcb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="99dcb-116">Application</span></span> | <span data-ttu-id="99dcb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="99dcb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99dcb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99dcb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="99dcb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="99dcb-119">Request headers</span></span>
| <span data-ttu-id="99dcb-120">名称</span><span class="sxs-lookup"><span data-stu-id="99dcb-120">Name</span></span>       | <span data-ttu-id="99dcb-121">说明</span><span class="sxs-lookup"><span data-stu-id="99dcb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99dcb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99dcb-122">Authorization</span></span>  | <span data-ttu-id="99dcb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99dcb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99dcb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="99dcb-125">Request body</span></span>
<span data-ttu-id="99dcb-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="99dcb-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99dcb-127">参数</span><span class="sxs-lookup"><span data-stu-id="99dcb-127">Parameter</span></span>    | <span data-ttu-id="99dcb-128">类型</span><span class="sxs-lookup"><span data-stu-id="99dcb-128">Type</span></span>   |<span data-ttu-id="99dcb-129">说明</span><span class="sxs-lookup"><span data-stu-id="99dcb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99dcb-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="99dcb-130">calculationType</span></span>|<span data-ttu-id="99dcb-131">string</span><span class="sxs-lookup"><span data-stu-id="99dcb-131">string</span></span>|<span data-ttu-id="99dcb-132">指定要使用的计算类型。</span><span class="sxs-lookup"><span data-stu-id="99dcb-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="99dcb-133">可取值为：`Recalculate`、`Full`、`FullRebuild`。</span><span class="sxs-lookup"><span data-stu-id="99dcb-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="99dcb-134">响应</span><span class="sxs-lookup"><span data-stu-id="99dcb-134">Response</span></span>

<span data-ttu-id="99dcb-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="99dcb-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99dcb-137">示例</span><span class="sxs-lookup"><span data-stu-id="99dcb-137">Example</span></span>
<span data-ttu-id="99dcb-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="99dcb-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99dcb-139">请求</span><span class="sxs-lookup"><span data-stu-id="99dcb-139">Request</span></span>
<span data-ttu-id="99dcb-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99dcb-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="99dcb-141">响应</span><span class="sxs-lookup"><span data-stu-id="99dcb-141">Response</span></span>
<span data-ttu-id="99dcb-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99dcb-142">Here is an example of the response.</span></span> 
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
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
