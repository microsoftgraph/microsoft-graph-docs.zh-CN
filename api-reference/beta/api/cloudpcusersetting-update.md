---
title: 更新 cloudPcUserSetting
description: 更新 cloudPcUserSetting 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2ea5b8f7084f2be8f4fd5d79345a69ee656f1fbb
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993646"
---
# <a name="update-cloudpcusersetting"></a><span data-ttu-id="a611a-103">更新 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="a611a-103">Update cloudPcUserSetting</span></span>

<span data-ttu-id="a611a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a611a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a611a-105">更新 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a611a-105">Update the properties of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="a611a-106">权限</span><span class="sxs-lookup"><span data-stu-id="a611a-106">Permissions</span></span>

<span data-ttu-id="a611a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a611a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a611a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a611a-109">Permission type</span></span>|<span data-ttu-id="a611a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a611a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a611a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a611a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a611a-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a611a-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a611a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a611a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a611a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a611a-114">Not supported.</span></span>|
|<span data-ttu-id="a611a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a611a-115">Application</span></span>|<span data-ttu-id="a611a-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a611a-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a611a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a611a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a611a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a611a-118">Request headers</span></span>

| <span data-ttu-id="a611a-119">名称</span><span class="sxs-lookup"><span data-stu-id="a611a-119">Name</span></span>          | <span data-ttu-id="a611a-120">说明</span><span class="sxs-lookup"><span data-stu-id="a611a-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="a611a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a611a-121">Authorization</span></span> | <span data-ttu-id="a611a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a611a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a611a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a611a-124">Content-Type</span></span>  | <span data-ttu-id="a611a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a611a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a611a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a611a-127">Request body</span></span>

<span data-ttu-id="a611a-128">在请求正文中，提供 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a611a-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="a611a-129">下表显示更新 [cloudPcUserSetting](../resources/cloudpcusersetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a611a-129">The following table shows the properties that are required when you update the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="a611a-130">属性</span><span class="sxs-lookup"><span data-stu-id="a611a-130">Property</span></span>|<span data-ttu-id="a611a-131">类型</span><span class="sxs-lookup"><span data-stu-id="a611a-131">Type</span></span>|<span data-ttu-id="a611a-132">说明</span><span class="sxs-lookup"><span data-stu-id="a611a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a611a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a611a-133">displayName</span></span>|<span data-ttu-id="a611a-134">String</span><span class="sxs-lookup"><span data-stu-id="a611a-134">String</span></span>|<span data-ttu-id="a611a-135">用户界面中显示的设置名称。</span><span class="sxs-lookup"><span data-stu-id="a611a-135">The setting name displayed in the user interface.</span></span>|
|<span data-ttu-id="a611a-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="a611a-136">localAdminEnabled</span></span>|<span data-ttu-id="a611a-137">布尔</span><span class="sxs-lookup"><span data-stu-id="a611a-137">Boolean</span></span>|<span data-ttu-id="a611a-138">若要启用本地管理员选项，将此设置更改为 `True` 。 </span><span class="sxs-lookup"><span data-stu-id="a611a-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="a611a-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="a611a-139">selfServiceEnabled</span></span>|<span data-ttu-id="a611a-140">布尔</span><span class="sxs-lookup"><span data-stu-id="a611a-140">Boolean</span></span>|<span data-ttu-id="a611a-141">若要启用自助服务选项，将此设置更改为 `True` 。 </span><span class="sxs-lookup"><span data-stu-id="a611a-141">To turn on the self-service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="a611a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a611a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="a611a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a611a-143">DateTimeOffset</span></span>|<span data-ttu-id="a611a-144">上次修改设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a611a-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="a611a-145">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a611a-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a611a-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="a611a-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |



## <a name="response"></a><span data-ttu-id="a611a-147">响应</span><span class="sxs-lookup"><span data-stu-id="a611a-147">Response</span></span>

<span data-ttu-id="a611a-148">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a611a-148">If successful, this method returns a `200 OK` response code and an updated [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a611a-149">示例</span><span class="sxs-lookup"><span data-stu-id="a611a-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a611a-150">请求</span><span class="sxs-lookup"><span data-stu-id="a611a-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_cloudpcusersetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": true,
  "localAdminEnabled": false
}
```


### <a name="response"></a><span data-ttu-id="a611a-151">响应</span><span class="sxs-lookup"><span data-stu-id="a611a-151">Response</span></span>
><span data-ttu-id="a611a-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a611a-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
