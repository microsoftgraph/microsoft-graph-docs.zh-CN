---
title: 创建 cloudPcUserSetting
description: 创建新的 cloudPcUserSetting 。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3edffeab1a7eaf4cac05200093d0f7a49d840614
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208497"
---
# <a name="create-cloudpcusersetting"></a><span data-ttu-id="bfb4b-103">创建 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="bfb4b-103">Create cloudPcUserSetting</span></span>

<span data-ttu-id="bfb4b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfb4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb4b-105">创建新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-105">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="bfb4b-106">权限</span><span class="sxs-lookup"><span data-stu-id="bfb4b-106">Permissions</span></span>

<span data-ttu-id="bfb4b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb4b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfb4b-109">Permission type</span></span>|<span data-ttu-id="bfb4b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfb4b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfb4b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bfb4b-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb4b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="bfb4b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfb4b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-114">Not supported.</span></span>|
|<span data-ttu-id="bfb4b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfb4b-115">Application</span></span>|<span data-ttu-id="bfb4b-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb4b-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfb4b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfb4b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings
```

## <a name="request-headers"></a><span data-ttu-id="bfb4b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfb4b-118">Request headers</span></span>

| <span data-ttu-id="bfb4b-119">名称</span><span class="sxs-lookup"><span data-stu-id="bfb4b-119">Name</span></span>          | <span data-ttu-id="bfb4b-120">说明</span><span class="sxs-lookup"><span data-stu-id="bfb4b-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="bfb4b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfb4b-121">Authorization</span></span> | <span data-ttu-id="bfb4b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bfb4b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfb4b-124">Content-Type</span></span>  | <span data-ttu-id="bfb4b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bfb4b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfb4b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfb4b-127">Request body</span></span>

<span data-ttu-id="bfb4b-128">在请求正文中，提供 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="bfb4b-129">下表显示创建 [cloudPcUserSetting](../resources/cloudpcusersetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-129">The following table shows the properties that are required when you create the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="bfb4b-130">属性</span><span class="sxs-lookup"><span data-stu-id="bfb4b-130">Property</span></span>|<span data-ttu-id="bfb4b-131">类型</span><span class="sxs-lookup"><span data-stu-id="bfb4b-131">Type</span></span>|<span data-ttu-id="bfb4b-132">说明</span><span class="sxs-lookup"><span data-stu-id="bfb4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfb4b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bfb4b-133">displayName</span></span>|<span data-ttu-id="bfb4b-134">String</span><span class="sxs-lookup"><span data-stu-id="bfb4b-134">String</span></span>|<span data-ttu-id="bfb4b-135">显示在 UI 中的设置名称。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-135">The setting name as it appears in the UI.</span></span> |
|<span data-ttu-id="bfb4b-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="bfb4b-136">localAdminEnabled</span></span>|<span data-ttu-id="bfb4b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb4b-137">Boolean</span></span>|<span data-ttu-id="bfb4b-138">若要启用本地管理员选项，将此设置更改为 `True` 。 </span><span class="sxs-lookup"><span data-stu-id="bfb4b-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="bfb4b-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="bfb4b-139">selfServiceEnabled</span></span>|<span data-ttu-id="bfb4b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfb4b-140">Boolean</span></span>|<span data-ttu-id="bfb4b-141">若要启用自助服务选项，将此设置更改为 `True` 。 </span><span class="sxs-lookup"><span data-stu-id="bfb4b-141">To turn on the self service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="bfb4b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfb4b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bfb4b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfb4b-143">DateTimeOffset</span></span>|<span data-ttu-id="bfb4b-144">上次修改设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="bfb4b-145">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bfb4b-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="response"></a><span data-ttu-id="bfb4b-147">响应</span><span class="sxs-lookup"><span data-stu-id="bfb4b-147">Response</span></span>

<span data-ttu-id="bfb4b-148">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-148">If successful, this method returns a `201 Created` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfb4b-149">示例</span><span class="sxs-lookup"><span data-stu-id="bfb4b-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfb4b-150">请求</span><span class="sxs-lookup"><span data-stu-id="bfb4b-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bfb4b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb4b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcusersetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="bfb4b-152">C#</span><span class="sxs-lookup"><span data-stu-id="bfb4b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcusersetting-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfb4b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb4b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcusersetting-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfb4b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfb4b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcusersetting-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfb4b-155">Java</span><span class="sxs-lookup"><span data-stu-id="bfb4b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcusersetting-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bfb4b-156">响应</span><span class="sxs-lookup"><span data-stu-id="bfb4b-156">Response</span></span>
><span data-ttu-id="bfb4b-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bfb4b-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "556092f8-92f8-5560-f892-6055f8926055",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true,
  "lastModifiedDateTime": "2021-02-01T10:29:57Z"  
}
```

