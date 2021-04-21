---
title: 更新 printConnector
description: 更新 printConnector 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 740884e815a3006929d2fcd15b62a2cd6cae8139
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921885"
---
# <a name="update-printconnector"></a><span data-ttu-id="525a3-103">更新 printConnector</span><span class="sxs-lookup"><span data-stu-id="525a3-103">Update printConnector</span></span>

<span data-ttu-id="525a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="525a3-105">更新 **printConnector 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="525a3-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="525a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="525a3-106">Permissions</span></span>
<span data-ttu-id="525a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="525a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="525a3-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="525a3-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="525a3-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="525a3-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="525a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="525a3-111">Permission type</span></span> | <span data-ttu-id="525a3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="525a3-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="525a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="525a3-113">Delegated (work or school account)</span></span>| <span data-ttu-id="525a3-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="525a3-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="525a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="525a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="525a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="525a3-116">Not Supported.</span></span>|
|<span data-ttu-id="525a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="525a3-117">Application</span></span>|<span data-ttu-id="525a3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="525a3-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="525a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="525a3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="525a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="525a3-120">Request headers</span></span>
| <span data-ttu-id="525a3-121">名称</span><span class="sxs-lookup"><span data-stu-id="525a3-121">Name</span></span>       | <span data-ttu-id="525a3-122">说明</span><span class="sxs-lookup"><span data-stu-id="525a3-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="525a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="525a3-123">Authorization</span></span> | <span data-ttu-id="525a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="525a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="525a3-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="525a3-126">Content-type</span></span>  | <span data-ttu-id="525a3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="525a3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="525a3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="525a3-129">Request body</span></span>
<span data-ttu-id="525a3-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="525a3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="525a3-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="525a3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="525a3-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="525a3-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="525a3-133">属性</span><span class="sxs-lookup"><span data-stu-id="525a3-133">Property</span></span>     | <span data-ttu-id="525a3-134">类型</span><span class="sxs-lookup"><span data-stu-id="525a3-134">Type</span></span>        | <span data-ttu-id="525a3-135">说明</span><span class="sxs-lookup"><span data-stu-id="525a3-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="525a3-136">name</span><span class="sxs-lookup"><span data-stu-id="525a3-136">name</span></span>|<span data-ttu-id="525a3-137">String</span><span class="sxs-lookup"><span data-stu-id="525a3-137">String</span></span>|<span data-ttu-id="525a3-138">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="525a3-138">The name of the connector.</span></span>|
|<span data-ttu-id="525a3-139">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="525a3-139">fullyQualifiedDomainName</span></span>|<span data-ttu-id="525a3-140">String</span><span class="sxs-lookup"><span data-stu-id="525a3-140">String</span></span>|<span data-ttu-id="525a3-141">连接器计算机主机名。</span><span class="sxs-lookup"><span data-stu-id="525a3-141">The connector machine's hostname.</span></span>|
|<span data-ttu-id="525a3-142">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="525a3-142">operatingSystem</span></span>|<span data-ttu-id="525a3-143">String</span><span class="sxs-lookup"><span data-stu-id="525a3-143">String</span></span>|<span data-ttu-id="525a3-144">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="525a3-144">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="525a3-145">appVersion</span><span class="sxs-lookup"><span data-stu-id="525a3-145">appVersion</span></span>|<span data-ttu-id="525a3-146">String</span><span class="sxs-lookup"><span data-stu-id="525a3-146">String</span></span>|<span data-ttu-id="525a3-147">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="525a3-147">The connector's version.</span></span>|
|<span data-ttu-id="525a3-148">位置</span><span class="sxs-lookup"><span data-stu-id="525a3-148">location</span></span>|[<span data-ttu-id="525a3-149">printerLocation</span><span class="sxs-lookup"><span data-stu-id="525a3-149">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="525a3-150">连接器的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="525a3-150">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="525a3-151">响应</span><span class="sxs-lookup"><span data-stu-id="525a3-151">Response</span></span>
<span data-ttu-id="525a3-152">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [printConnector](../resources/printConnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="525a3-152">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="525a3-153">示例</span><span class="sxs-lookup"><span data-stu-id="525a3-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="525a3-154">请求</span><span class="sxs-lookup"><span data-stu-id="525a3-154">Request</span></span>
<span data-ttu-id="525a3-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="525a3-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="525a3-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="525a3-156">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="525a3-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="525a3-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

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
# <a name="c"></a>[<span data-ttu-id="525a3-158">C#</span><span class="sxs-lookup"><span data-stu-id="525a3-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="525a3-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="525a3-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="525a3-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="525a3-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="525a3-161">Java</span><span class="sxs-lookup"><span data-stu-id="525a3-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="525a3-162">响应</span><span class="sxs-lookup"><span data-stu-id="525a3-162">Response</span></span>
<span data-ttu-id="525a3-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="525a3-163">The following is an example of the response.</span></span>
><span data-ttu-id="525a3-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="525a3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 406

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
