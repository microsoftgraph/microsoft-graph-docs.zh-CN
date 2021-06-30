---
title: 获取 cloudPcUserSetting
description: 读取 cloudPcUserSetting 对象的属性和关系。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7b3361b2c0ed7fdf2d97890aec78ef336912aeb2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207290"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="9dde1-103">获取 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="9dde1-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="9dde1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dde1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dde1-105">读取 [cloudPcUserSetting 对象的属性和](../resources/cloudpcusersetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9dde1-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="9dde1-106">权限</span><span class="sxs-lookup"><span data-stu-id="9dde1-106">Permissions</span></span>

<span data-ttu-id="9dde1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dde1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dde1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dde1-109">Permission type</span></span>|<span data-ttu-id="9dde1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dde1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dde1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dde1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9dde1-112">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dde1-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9dde1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dde1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dde1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dde1-114">Not supported.</span></span>|
|<span data-ttu-id="9dde1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dde1-115">Application</span></span>|<span data-ttu-id="9dde1-116">CloudPC.Read.All、CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dde1-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dde1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dde1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9dde1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9dde1-118">Optional query parameters</span></span>

<span data-ttu-id="9dde1-119">此方法支持 `$select` `$expand` 和 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9dde1-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9dde1-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9dde1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9dde1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dde1-121">Request headers</span></span>

| <span data-ttu-id="9dde1-122">名称</span><span class="sxs-lookup"><span data-stu-id="9dde1-122">Name</span></span>          | <span data-ttu-id="9dde1-123">说明</span><span class="sxs-lookup"><span data-stu-id="9dde1-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9dde1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dde1-124">Authorization</span></span> | <span data-ttu-id="9dde1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9dde1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dde1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dde1-127">Request body</span></span>

<span data-ttu-id="9dde1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dde1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dde1-129">响应</span><span class="sxs-lookup"><span data-stu-id="9dde1-129">Response</span></span>

<span data-ttu-id="9dde1-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9dde1-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9dde1-131">示例</span><span class="sxs-lookup"><span data-stu-id="9dde1-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="9dde1-132">示例 1：获取指定用户设置的属性</span><span class="sxs-lookup"><span data-stu-id="9dde1-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="9dde1-133">请求</span><span class="sxs-lookup"><span data-stu-id="9dde1-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9dde1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dde1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```
# <a name="c"></a>[<span data-ttu-id="9dde1-135">C#</span><span class="sxs-lookup"><span data-stu-id="9dde1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dde1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dde1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dde1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dde1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dde1-138">Java</span><span class="sxs-lookup"><span data-stu-id="9dde1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="9dde1-139">响应</span><span class="sxs-lookup"><span data-stu-id="9dde1-139">Response</span></span>
><span data-ttu-id="9dde1-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9dde1-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "556092f8-92f8-5560-f892-6055f8926055",
    "displayName": "String",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="9dde1-141">示例 2：获取指定用户设置的属性，然后展开工作分配</span><span class="sxs-lookup"><span data-stu-id="9dde1-141">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="9dde1-142">请求</span><span class="sxs-lookup"><span data-stu-id="9dde1-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9dde1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dde1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="9dde1-144">C#</span><span class="sxs-lookup"><span data-stu-id="9dde1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dde1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dde1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dde1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dde1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dde1-147">Java</span><span class="sxs-lookup"><span data-stu-id="9dde1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="9dde1-148">响应</span><span class="sxs-lookup"><span data-stu-id="9dde1-148">Response</span></span>

<span data-ttu-id="9dde1-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9dde1-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "createdDateTime": "2021-02-01T10:29:57Z",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
