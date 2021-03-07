---
title: 更新 printConnector
description: 更新 printConnector 对象的属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1fea6a1fe18012dcca1c266304e4430b1adcd660
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516970"
---
# <a name="update-printconnector"></a><span data-ttu-id="67e14-103">更新 printConnector</span><span class="sxs-lookup"><span data-stu-id="67e14-103">Update printConnector</span></span>
<span data-ttu-id="67e14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="67e14-105">更新 **printConnector 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="67e14-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67e14-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="67e14-106">Permissions</span></span>
<span data-ttu-id="67e14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67e14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67e14-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="67e14-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="67e14-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="67e14-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="67e14-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="67e14-111">Permission type</span></span> | <span data-ttu-id="67e14-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67e14-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="67e14-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67e14-113">Delegated (work or school account)</span></span>| <span data-ttu-id="67e14-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e14-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="67e14-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67e14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67e14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e14-116">Not Supported.</span></span>|
|<span data-ttu-id="67e14-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="67e14-117">Application</span></span>|<span data-ttu-id="67e14-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e14-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67e14-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67e14-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="67e14-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="67e14-120">Request headers</span></span>
|<span data-ttu-id="67e14-121">名称</span><span class="sxs-lookup"><span data-stu-id="67e14-121">Name</span></span>|<span data-ttu-id="67e14-122">说明</span><span class="sxs-lookup"><span data-stu-id="67e14-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="67e14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e14-123">Authorization</span></span>|<span data-ttu-id="67e14-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67e14-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67e14-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67e14-126">Content-Type</span></span>|<span data-ttu-id="67e14-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="67e14-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67e14-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="67e14-129">Request body</span></span>
<span data-ttu-id="67e14-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="67e14-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="67e14-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="67e14-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="67e14-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="67e14-132">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="67e14-133">响应</span><span class="sxs-lookup"><span data-stu-id="67e14-133">Response</span></span>
<span data-ttu-id="67e14-134">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [printConnector](../resources/printConnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67e14-134">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67e14-135">示例</span><span class="sxs-lookup"><span data-stu-id="67e14-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67e14-136">请求</span><span class="sxs-lookup"><span data-stu-id="67e14-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printconnector"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
Content-Type: application/json
Content-length: 308

{
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a><span data-ttu-id="67e14-137">响应</span><span class="sxs-lookup"><span data-stu-id="67e14-137">Response</span></span>
<span data-ttu-id="67e14-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="67e14-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "displayName": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
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
```

