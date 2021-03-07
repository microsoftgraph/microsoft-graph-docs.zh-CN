---
title: 列出打印机
description: 检索在租户中注册的打印机列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ff93eb5c598458c57126f0e8edda2a4f440dfc65
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517140"
---
# <a name="list-printers"></a><span data-ttu-id="bab89-103">列出打印机</span><span class="sxs-lookup"><span data-stu-id="bab89-103">List printers</span></span>
<span data-ttu-id="bab89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="bab89-105">检索在 **租户中** 注册的打印机列表。</span><span class="sxs-lookup"><span data-stu-id="bab89-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="bab89-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bab89-106">Permissions</span></span>
<span data-ttu-id="bab89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bab89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bab89-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="bab89-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="bab89-110">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="bab89-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="bab89-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bab89-111">Permission type</span></span> | <span data-ttu-id="bab89-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bab89-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bab89-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bab89-113">Delegated (work or school account)</span></span>| <span data-ttu-id="bab89-114">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="bab89-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="bab89-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bab89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bab89-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bab89-116">Not Supported.</span></span>|
|<span data-ttu-id="bab89-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bab89-117">Application</span></span>| <span data-ttu-id="bab89-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bab89-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bab89-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bab89-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab89-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bab89-120">Optional query parameters</span></span>
<span data-ttu-id="bab89-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bab89-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bab89-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bab89-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="bab89-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="bab89-123">Exceptions</span></span>
* <span data-ttu-id="bab89-124">和 `$expand` `select` 运算符受导航属性支持，但 `share` 不支持 `jobs` 。</span><span class="sxs-lookup"><span data-stu-id="bab89-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="bab89-125">不支持某些运算符： `$count` `$search` .</span><span class="sxs-lookup"><span data-stu-id="bab89-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bab89-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="bab89-126">Request headers</span></span>
|<span data-ttu-id="bab89-127">名称</span><span class="sxs-lookup"><span data-stu-id="bab89-127">Name</span></span>|<span data-ttu-id="bab89-128">说明</span><span class="sxs-lookup"><span data-stu-id="bab89-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bab89-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab89-129">Authorization</span></span>|<span data-ttu-id="bab89-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bab89-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bab89-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="bab89-132">Request body</span></span>
<span data-ttu-id="bab89-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bab89-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab89-134">响应</span><span class="sxs-lookup"><span data-stu-id="bab89-134">Response</span></span>

<span data-ttu-id="bab89-135">如果成功，此方法在响应正文中返回响应代码和打印机 `200 OK` 对象集合。 [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="bab89-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>

><span data-ttu-id="bab89-136">**注意**：响应将不包含"defaults"和"capabilities"属性。</span><span class="sxs-lookup"><span data-stu-id="bab89-136">**Note**: The response will not contain 'defaults' and 'capabilities' properties.</span></span> <span data-ttu-id="bab89-137">可以使用"获取打印机" [请求查询这些属性](printer-get.md) 。</span><span class="sxs-lookup"><span data-stu-id="bab89-137">These properties can be queried using [Get Printer](printer-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="bab89-138">示例</span><span class="sxs-lookup"><span data-stu-id="bab89-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bab89-139">请求</span><span class="sxs-lookup"><span data-stu-id="bab89-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printer"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers
```


### <a name="response"></a><span data-ttu-id="bab89-140">响应</span><span class="sxs-lookup"><span data-stu-id="bab89-140">Response</span></span>
<span data-ttu-id="bab89-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bab89-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "PrinterName",
      "manufacturer": "PrinterManufacturer",
      "model": "PrinterModel",
      "isShared": true,
      "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
      "isAcceptingJobs": true,
      "status": {
        "state": "stopped",
        "details": [
          "disconnected"
        ],
        "description": ""
      },
      "defaults": {
        "copiesPerJob": 1,
        "finishings": [
          "none"
        ],
        "mediaColor": "Unknown",
        "mediaType": "stationery",
        "mediaSize": "North America Letter",
        "pagesPerSheet": 1,
        "orientation": "portrait",
        "outputBin": "auto",
        "inputBin": "auto",
        "contentType": "application/oxps",
        "fitPdfToPage": false,
        "multipageLayout": null,
        "colorMode": "color",
        "quality": "medium",
        "duplexMode": "oneSided",
        "dpi": 600,
        "scaling": null
      },
      "location": {
        "latitude": 1.1,
        "longitude": 2.2,
        "altitudeInMeters": 3,
        "streetAddress": "One Microsoft Way",
        "subUnit": [
          "Main Plaza",
          "Unit 400"
        ],
        "city": "Redmond",
        "postalCode": "98052",
        "countryOrRegion": "USA",
        "site": "Puget Sound",
        "building": "Studio E",
        "floor": "1",
        "floorDescription": "First Floor",
        "roomName": "1234",
        "roomDescription": "First floor copy room",
        "organization": [
          "C+AI",
          "Microsoft Graph"
        ],
        "subdivision": [
          "King County",
          "Red West"
        ],
        "stateOrProvince": "Washington"
      }
    }
  ]
}
```

