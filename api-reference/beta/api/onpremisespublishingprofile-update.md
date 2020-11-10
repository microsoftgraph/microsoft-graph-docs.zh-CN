---
title: 更新 onPremisesPublishingProfile
description: 更新 onPremisesPublishingProfile 对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfcd5ffb5cc2665559d0b74c9a2722424d3ee3be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968784"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="56165-103">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="56165-103">Update onPremisesPublishingProfile</span></span>

<span data-ttu-id="56165-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56165-105">更新 [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56165-105">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56165-106">权限</span><span class="sxs-lookup"><span data-stu-id="56165-106">Permissions</span></span>

<span data-ttu-id="56165-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56165-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56165-109">Permission type</span></span>                        | <span data-ttu-id="56165-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56165-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="56165-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56165-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56165-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56165-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="56165-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56165-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56165-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="56165-114">Not supported.</span></span> |
| <span data-ttu-id="56165-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56165-115">Application</span></span>                            | <span data-ttu-id="56165-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56165-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56165-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56165-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="56165-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="56165-118">Request headers</span></span>

| <span data-ttu-id="56165-119">名称</span><span class="sxs-lookup"><span data-stu-id="56165-119">Name</span></span>       | <span data-ttu-id="56165-120">说明</span><span class="sxs-lookup"><span data-stu-id="56165-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="56165-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56165-121">Authorization</span></span> | <span data-ttu-id="56165-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="56165-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="56165-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="56165-123">Request body</span></span>

<span data-ttu-id="56165-124">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="56165-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="56165-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="56165-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="56165-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="56165-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="56165-127">属性</span><span class="sxs-lookup"><span data-stu-id="56165-127">Property</span></span>     | <span data-ttu-id="56165-128">类型</span><span class="sxs-lookup"><span data-stu-id="56165-128">Type</span></span>        | <span data-ttu-id="56165-129">说明</span><span class="sxs-lookup"><span data-stu-id="56165-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56165-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="56165-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="56165-131">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="56165-131">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="56165-132">表示 [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="56165-132">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="56165-133">响应</span><span class="sxs-lookup"><span data-stu-id="56165-133">Response</span></span>

<span data-ttu-id="56165-134">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="56165-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56165-135">示例</span><span class="sxs-lookup"><span data-stu-id="56165-135">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="56165-136">示例1：更新 hybridAgentUpdaterConfiguration 中的 updateWindow</span><span class="sxs-lookup"><span data-stu-id="56165-136">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="56165-137">下面的示例更新 **hybridAgentUpdaterConfiguration** 中的 **updateWindow** 。</span><span class="sxs-lookup"><span data-stu-id="56165-137">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="56165-138">请求</span><span class="sxs-lookup"><span data-stu-id="56165-138">Request</span></span>

<span data-ttu-id="56165-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56165-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56165-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="56165-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="56165-141">C#</span><span class="sxs-lookup"><span data-stu-id="56165-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56165-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56165-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56165-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56165-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56165-144">Java</span><span class="sxs-lookup"><span data-stu-id="56165-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56165-145">响应</span><span class="sxs-lookup"><span data-stu-id="56165-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="56165-146">示例2：更新 hybridAgentUpdaterConfiguration 中的 deferUpdate</span><span class="sxs-lookup"><span data-stu-id="56165-146">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="56165-147">下面的示例更新 **hybridAgentUpdaterConfiguration** 中的 **deferUpdate** 。</span><span class="sxs-lookup"><span data-stu-id="56165-147">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="56165-148">请求</span><span class="sxs-lookup"><span data-stu-id="56165-148">Request</span></span>

<span data-ttu-id="56165-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56165-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="56165-150">响应</span><span class="sxs-lookup"><span data-stu-id="56165-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="56165-151">示例3：更新 hybridAgentUpdaterConfiguration 中的 allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="56165-151">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="56165-152">下面的示例更新 **hybridAgentUpdaterConfiguration** 中的 **allowUpdateConfigurationOverride** 。</span><span class="sxs-lookup"><span data-stu-id="56165-152">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="56165-153">请求</span><span class="sxs-lookup"><span data-stu-id="56165-153">Request</span></span>

<span data-ttu-id="56165-154">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56165-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="56165-155">响应</span><span class="sxs-lookup"><span data-stu-id="56165-155">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


