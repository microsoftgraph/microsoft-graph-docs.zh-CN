---
title: agreementAcceptance 资源类型
description: 表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ac0e6d67e10e7d7b81fc1c5c21e93251f84cab0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722618"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="4e863-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e863-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="4e863-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e863-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e863-105">表示 Azure Active Directory 支持 Azure AD) 受 Azure Active Directory 支持的公司可自定义使用条款范围内的 (状态。</span><span class="sxs-lookup"><span data-stu-id="4e863-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="4e863-106">属性</span><span class="sxs-lookup"><span data-stu-id="4e863-106">Properties</span></span>
| <span data-ttu-id="4e863-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e863-107">Property</span></span>     | <span data-ttu-id="4e863-108">类型</span><span class="sxs-lookup"><span data-stu-id="4e863-108">Type</span></span>        | <span data-ttu-id="4e863-109">说明</span><span class="sxs-lookup"><span data-stu-id="4e863-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4e863-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="4e863-110">agreementFileId</span></span>|<span data-ttu-id="4e863-111">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-111">String</span></span>|<span data-ttu-id="4e863-112">用户接受的协议文件的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e863-112">The identifier of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="4e863-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="4e863-113">agreementId</span></span>|<span data-ttu-id="4e863-114">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-114">String</span></span>|<span data-ttu-id="4e863-115">协议的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e863-115">The identifier of the agreement.</span></span>|
|<span data-ttu-id="4e863-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4e863-116">deviceDisplayName</span></span>|<span data-ttu-id="4e863-117">String</span><span class="sxs-lookup"><span data-stu-id="4e863-117">String</span></span>|<span data-ttu-id="4e863-118">用于显示名称协议的设备的设备组。</span><span class="sxs-lookup"><span data-stu-id="4e863-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="4e863-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="4e863-119">deviceId</span></span>|<span data-ttu-id="4e863-120">String</span><span class="sxs-lookup"><span data-stu-id="4e863-120">String</span></span>|<span data-ttu-id="4e863-121">用于接受协议的设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4e863-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="4e863-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="4e863-122">deviceOSType</span></span>|<span data-ttu-id="4e863-123">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-123">String</span></span>|<span data-ttu-id="4e863-124">用于接受协议的操作系统。</span><span class="sxs-lookup"><span data-stu-id="4e863-124">The operating system used to accept the agreement.</span></span>|
|<span data-ttu-id="4e863-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="4e863-125">deviceOSVersion</span></span>|<span data-ttu-id="4e863-126">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-126">String</span></span>|<span data-ttu-id="4e863-127">用于接受协议的设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4e863-127">The operating system version of the device used to accept the agreement.</span></span>    |
|<span data-ttu-id="4e863-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4e863-128">expirationDateTime</span></span>|<span data-ttu-id="4e863-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e863-129">DateTimeOffset</span></span>|<span data-ttu-id="4e863-130">接受的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="4e863-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="4e863-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4e863-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4e863-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4e863-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4e863-133">id</span><span class="sxs-lookup"><span data-stu-id="4e863-133">id</span></span>|<span data-ttu-id="4e863-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-134">String</span></span>| <span data-ttu-id="4e863-135">协议接受的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e863-135">The identifier of the agreement acceptance.</span></span> <span data-ttu-id="4e863-136">只读。</span><span class="sxs-lookup"><span data-stu-id="4e863-136">Read-only.</span></span>|
|<span data-ttu-id="4e863-137">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e863-137">recordedDateTime</span></span>|<span data-ttu-id="4e863-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e863-138">DateTimeOffset</span></span>|<span data-ttu-id="4e863-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4e863-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4e863-141">state</span><span class="sxs-lookup"><span data-stu-id="4e863-141">state</span></span>|<span data-ttu-id="4e863-142">string</span><span class="sxs-lookup"><span data-stu-id="4e863-142">string</span></span>| <span data-ttu-id="4e863-143">协议接受的状态。</span><span class="sxs-lookup"><span data-stu-id="4e863-143">The state of the agreement acceptance.</span></span> <span data-ttu-id="4e863-144">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="4e863-144">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="4e863-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4e863-145">userDisplayName</span></span>|<span data-ttu-id="4e863-146">String</span><span class="sxs-lookup"><span data-stu-id="4e863-146">String</span></span>|<span data-ttu-id="4e863-147">记录接受时用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4e863-147">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4e863-148">userEmail</span><span class="sxs-lookup"><span data-stu-id="4e863-148">userEmail</span></span>|<span data-ttu-id="4e863-149">String</span><span class="sxs-lookup"><span data-stu-id="4e863-149">String</span></span>|<span data-ttu-id="4e863-150">记录接受时用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4e863-150">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="4e863-151">userId</span><span class="sxs-lookup"><span data-stu-id="4e863-151">userId</span></span>|<span data-ttu-id="4e863-152">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-152">String</span></span>|<span data-ttu-id="4e863-153">接受该协议的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e863-153">The identifier of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="4e863-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e863-154">userPrincipalName</span></span>|<span data-ttu-id="4e863-155">字符串</span><span class="sxs-lookup"><span data-stu-id="4e863-155">String</span></span>|<span data-ttu-id="4e863-156">记录接受时用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="4e863-156">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e863-157">关系</span><span class="sxs-lookup"><span data-stu-id="4e863-157">Relationships</span></span>
<span data-ttu-id="4e863-158">无。</span><span class="sxs-lookup"><span data-stu-id="4e863-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4e863-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e863-159">JSON representation</span></span>

<span data-ttu-id="4e863-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e863-160">The following is a JSON representation of the resource.</span></span>

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


