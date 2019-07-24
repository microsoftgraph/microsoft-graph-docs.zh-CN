---
title: 更新 onPremisesPublishingProfile
description: 更新 onPremisesPublishingProfile 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2cdd2eafc51e5bd38aed41fcfcae259b5a9fe66
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841078"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="06bba-103">更新 onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="06bba-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06bba-104">更新[onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06bba-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="06bba-105">权限</span><span class="sxs-lookup"><span data-stu-id="06bba-105">Permissions</span></span>

<span data-ttu-id="06bba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06bba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="06bba-108">Permission type</span></span>                        | <span data-ttu-id="06bba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06bba-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="06bba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06bba-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="06bba-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="06bba-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="06bba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06bba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06bba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="06bba-113">Not supported.</span></span> |
| <span data-ttu-id="06bba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="06bba-114">Application</span></span>                            | <span data-ttu-id="06bba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06bba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06bba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06bba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="06bba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="06bba-117">Request headers</span></span>

| <span data-ttu-id="06bba-118">名称</span><span class="sxs-lookup"><span data-stu-id="06bba-118">Name</span></span>       | <span data-ttu-id="06bba-119">说明</span><span class="sxs-lookup"><span data-stu-id="06bba-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="06bba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="06bba-120">Authorization</span></span> | <span data-ttu-id="06bba-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="06bba-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="06bba-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="06bba-122">Request body</span></span>

<span data-ttu-id="06bba-123">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="06bba-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="06bba-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="06bba-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="06bba-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="06bba-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="06bba-126">属性</span><span class="sxs-lookup"><span data-stu-id="06bba-126">Property</span></span>     | <span data-ttu-id="06bba-127">类型</span><span class="sxs-lookup"><span data-stu-id="06bba-127">Type</span></span>        | <span data-ttu-id="06bba-128">说明</span><span class="sxs-lookup"><span data-stu-id="06bba-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="06bba-129">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="06bba-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="06bba-130">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="06bba-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="06bba-131">表示[hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="06bba-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="06bba-132">响应</span><span class="sxs-lookup"><span data-stu-id="06bba-132">Response</span></span>

<span data-ttu-id="06bba-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="06bba-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="06bba-134">示例</span><span class="sxs-lookup"><span data-stu-id="06bba-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="06bba-135">示例 1: 更新 hybridAgentUpdaterConfiguration 中的 updateWindow</span><span class="sxs-lookup"><span data-stu-id="06bba-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="06bba-136">下面的示例更新**hybridAgentUpdaterConfiguration**中的**updateWindow** 。</span><span class="sxs-lookup"><span data-stu-id="06bba-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="06bba-137">请求</span><span class="sxs-lookup"><span data-stu-id="06bba-137">Request</span></span>

<span data-ttu-id="06bba-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="06bba-138">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="06bba-139">响应</span><span class="sxs-lookup"><span data-stu-id="06bba-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="06bba-140">示例 2: 更新 hybridAgentUpdaterConfiguration 中的 deferUpdate</span><span class="sxs-lookup"><span data-stu-id="06bba-140">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="06bba-141">下面的示例更新**hybridAgentUpdaterConfiguration**中的**deferUpdate** 。</span><span class="sxs-lookup"><span data-stu-id="06bba-141">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="06bba-142">请求</span><span class="sxs-lookup"><span data-stu-id="06bba-142">Request</span></span>

<span data-ttu-id="06bba-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="06bba-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="06bba-144">响应</span><span class="sxs-lookup"><span data-stu-id="06bba-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="06bba-145">示例 3: 更新 hybridAgentUpdaterConfiguration 中的 allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="06bba-145">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="06bba-146">下面的示例更新**hybridAgentUpdaterConfiguration**中的**allowUpdateConfigurationOverride** 。</span><span class="sxs-lookup"><span data-stu-id="06bba-146">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="06bba-147">请求</span><span class="sxs-lookup"><span data-stu-id="06bba-147">Request</span></span>

<span data-ttu-id="06bba-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="06bba-148">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="06bba-149">响应</span><span class="sxs-lookup"><span data-stu-id="06bba-149">Response</span></span>

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
