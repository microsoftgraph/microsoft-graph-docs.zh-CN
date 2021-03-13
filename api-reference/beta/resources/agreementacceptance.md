---
title: agreementAcceptance 资源类型
description: 表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 4e00ae32078bd004ad4063a0f73ebb94b6a77f9c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761098"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="4392c-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="4392c-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="4392c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4392c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4392c-105">表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。</span><span class="sxs-lookup"><span data-stu-id="4392c-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="4392c-106">属性</span><span class="sxs-lookup"><span data-stu-id="4392c-106">Properties</span></span>
| <span data-ttu-id="4392c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4392c-107">Property</span></span>     | <span data-ttu-id="4392c-108">类型</span><span class="sxs-lookup"><span data-stu-id="4392c-108">Type</span></span>        | <span data-ttu-id="4392c-109">说明</span><span class="sxs-lookup"><span data-stu-id="4392c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4392c-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="4392c-110">agreementFileId</span></span>|<span data-ttu-id="4392c-111">String</span><span class="sxs-lookup"><span data-stu-id="4392c-111">String</span></span>|<span data-ttu-id="4392c-112">用户接受的协议文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="4392c-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="4392c-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="4392c-113">agreementId</span></span>|<span data-ttu-id="4392c-114">String</span><span class="sxs-lookup"><span data-stu-id="4392c-114">String</span></span>|<span data-ttu-id="4392c-115">协议的 ID。</span><span class="sxs-lookup"><span data-stu-id="4392c-115">ID of the agreement.</span></span>|
|<span data-ttu-id="4392c-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4392c-116">deviceDisplayName</span></span>|<span data-ttu-id="4392c-117">String</span><span class="sxs-lookup"><span data-stu-id="4392c-117">String</span></span>|<span data-ttu-id="4392c-118">用于显示名称协议的设备的设备组。</span><span class="sxs-lookup"><span data-stu-id="4392c-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="4392c-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="4392c-119">deviceId</span></span>|<span data-ttu-id="4392c-120">String</span><span class="sxs-lookup"><span data-stu-id="4392c-120">String</span></span>|<span data-ttu-id="4392c-121">用于接受协议的设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4392c-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="4392c-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="4392c-122">deviceOSType</span></span>|<span data-ttu-id="4392c-123">String</span><span class="sxs-lookup"><span data-stu-id="4392c-123">String</span></span>|<span data-ttu-id="4392c-124">用于接受协议的操作系统。</span><span class="sxs-lookup"><span data-stu-id="4392c-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="4392c-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="4392c-125">deviceOSVersion</span></span>|<span data-ttu-id="4392c-126">String</span><span class="sxs-lookup"><span data-stu-id="4392c-126">String</span></span>|<span data-ttu-id="4392c-127">用于接受协议的设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4392c-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="4392c-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4392c-128">expirationDateTime</span></span>|<span data-ttu-id="4392c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4392c-129">DateTimeOffset</span></span>|<span data-ttu-id="4392c-130">接受的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="4392c-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="4392c-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4392c-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4392c-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="4392c-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4392c-133">id</span><span class="sxs-lookup"><span data-stu-id="4392c-133">id</span></span>|<span data-ttu-id="4392c-134">String</span><span class="sxs-lookup"><span data-stu-id="4392c-134">String</span></span>| <span data-ttu-id="4392c-135">只读。</span><span class="sxs-lookup"><span data-stu-id="4392c-135">Read-only.</span></span>|
|<span data-ttu-id="4392c-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="4392c-136">recordedDateTime</span></span>|<span data-ttu-id="4392c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4392c-137">DateTimeOffset</span></span>|<span data-ttu-id="4392c-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4392c-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4392c-139">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="4392c-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4392c-140">state</span><span class="sxs-lookup"><span data-stu-id="4392c-140">state</span></span>|<span data-ttu-id="4392c-141">string</span><span class="sxs-lookup"><span data-stu-id="4392c-141">string</span></span>| <span data-ttu-id="4392c-142">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="4392c-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="4392c-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4392c-143">userDisplayName</span></span>|<span data-ttu-id="4392c-144">String</span><span class="sxs-lookup"><span data-stu-id="4392c-144">String</span></span>|<span data-ttu-id="4392c-145">记录接受时用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4392c-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4392c-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="4392c-146">userEmail</span></span>|<span data-ttu-id="4392c-147">String</span><span class="sxs-lookup"><span data-stu-id="4392c-147">String</span></span>|<span data-ttu-id="4392c-148">记录接受时用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4392c-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4392c-149">userId</span><span class="sxs-lookup"><span data-stu-id="4392c-149">userId</span></span>|<span data-ttu-id="4392c-150">String</span><span class="sxs-lookup"><span data-stu-id="4392c-150">String</span></span>|<span data-ttu-id="4392c-151">接受该协议的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="4392c-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="4392c-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4392c-152">userPrincipalName</span></span>|<span data-ttu-id="4392c-153">String</span><span class="sxs-lookup"><span data-stu-id="4392c-153">String</span></span>|<span data-ttu-id="4392c-154">记录接受时用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4392c-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4392c-155">关系</span><span class="sxs-lookup"><span data-stu-id="4392c-155">Relationships</span></span>
<span data-ttu-id="4392c-156">无。</span><span class="sxs-lookup"><span data-stu-id="4392c-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4392c-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4392c-157">JSON representation</span></span>

<span data-ttu-id="4392c-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4392c-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


