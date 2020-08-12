---
title: agreementAcceptance 资源类型
description: 表示在受 Azure Active Directory (Azure AD) 支持的公司自定义使用条款的范围内的用户的当前状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 18bcf00cad681d3003faf2dce442e4ea1f58bdb0
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643973"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="bcb46-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="bcb46-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="bcb46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcb46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcb46-105">表示在受 Azure Active Directory (Azure AD) 支持的公司自定义使用条款的范围内的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="bcb46-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="bcb46-106">属性</span><span class="sxs-lookup"><span data-stu-id="bcb46-106">Properties</span></span>
| <span data-ttu-id="bcb46-107">属性</span><span class="sxs-lookup"><span data-stu-id="bcb46-107">Property</span></span>     | <span data-ttu-id="bcb46-108">类型</span><span class="sxs-lookup"><span data-stu-id="bcb46-108">Type</span></span>        | <span data-ttu-id="bcb46-109">说明</span><span class="sxs-lookup"><span data-stu-id="bcb46-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bcb46-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="bcb46-110">agreementFileId</span></span>|<span data-ttu-id="bcb46-111">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-111">String</span></span>|<span data-ttu-id="bcb46-112">用户接受的协议文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcb46-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="bcb46-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="bcb46-113">agreementId</span></span>|<span data-ttu-id="bcb46-114">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-114">String</span></span>|<span data-ttu-id="bcb46-115">协议的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcb46-115">ID of the agreement.</span></span>|
|<span data-ttu-id="bcb46-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcb46-116">deviceDisplayName</span></span>|<span data-ttu-id="bcb46-117">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-117">String</span></span>|<span data-ttu-id="bcb46-118">用于接受协议的设备的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bcb46-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="bcb46-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="bcb46-119">deviceId</span></span>|<span data-ttu-id="bcb46-120">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-120">String</span></span>|<span data-ttu-id="bcb46-121">用于接受协议的设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bcb46-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="bcb46-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="bcb46-122">deviceOSType</span></span>|<span data-ttu-id="bcb46-123">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-123">String</span></span>|<span data-ttu-id="bcb46-124">用于接受协议的操作系统。</span><span class="sxs-lookup"><span data-stu-id="bcb46-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="bcb46-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="bcb46-125">deviceOSVersion</span></span>|<span data-ttu-id="bcb46-126">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-126">String</span></span>|<span data-ttu-id="bcb46-127">用于接受协议的设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="bcb46-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="bcb46-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb46-128">expirationDateTime</span></span>|<span data-ttu-id="bcb46-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb46-129">DateTimeOffset</span></span>|<span data-ttu-id="bcb46-130">接受的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="bcb46-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="bcb46-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="bcb46-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bcb46-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bcb46-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcb46-133">id</span><span class="sxs-lookup"><span data-stu-id="bcb46-133">id</span></span>|<span data-ttu-id="bcb46-134">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-134">String</span></span>| <span data-ttu-id="bcb46-135">只读。</span><span class="sxs-lookup"><span data-stu-id="bcb46-135">Read-only.</span></span>|
|<span data-ttu-id="bcb46-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb46-136">recordedDateTime</span></span>|<span data-ttu-id="bcb46-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb46-137">DateTimeOffset</span></span>|<span data-ttu-id="bcb46-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bcb46-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bcb46-140">state</span><span class="sxs-lookup"><span data-stu-id="bcb46-140">state</span></span>|<span data-ttu-id="bcb46-141">string</span><span class="sxs-lookup"><span data-stu-id="bcb46-141">string</span></span>| <span data-ttu-id="bcb46-142">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="bcb46-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="bcb46-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcb46-143">userDisplayName</span></span>|<span data-ttu-id="bcb46-144">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-144">String</span></span>|<span data-ttu-id="bcb46-145">记录接受时的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bcb46-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="bcb46-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="bcb46-146">userEmail</span></span>|<span data-ttu-id="bcb46-147">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-147">String</span></span>|<span data-ttu-id="bcb46-148">记录接受时用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="bcb46-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="bcb46-149">userId</span><span class="sxs-lookup"><span data-stu-id="bcb46-149">userId</span></span>|<span data-ttu-id="bcb46-150">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-150">String</span></span>|<span data-ttu-id="bcb46-151">接受协议的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="bcb46-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="bcb46-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcb46-152">userPrincipalName</span></span>|<span data-ttu-id="bcb46-153">String</span><span class="sxs-lookup"><span data-stu-id="bcb46-153">String</span></span>|<span data-ttu-id="bcb46-154">记录接受时的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="bcb46-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcb46-155">关系</span><span class="sxs-lookup"><span data-stu-id="bcb46-155">Relationships</span></span>
<span data-ttu-id="bcb46-156">无。</span><span class="sxs-lookup"><span data-stu-id="bcb46-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bcb46-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcb46-157">JSON representation</span></span>

<span data-ttu-id="bcb46-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bcb46-158">The following is a JSON representation of the resource.</span></span>

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
