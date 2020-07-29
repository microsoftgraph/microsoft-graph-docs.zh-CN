---
title: pstnCallLogRow 资源类型
description: 表示公共交换机电话网络（PSTN）呼叫日志中的数据行。
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdcaaa311ea3d1f875bd3933420cfed058ef7808
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510028"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="97efc-103">pstnCallLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="97efc-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="97efc-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="97efc-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97efc-105">表示公共交换机电话网络（PSTN）呼叫日志中的数据行。</span><span class="sxs-lookup"><span data-stu-id="97efc-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="97efc-106">每行都映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="97efc-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="97efc-107">属性</span><span class="sxs-lookup"><span data-stu-id="97efc-107">Properties</span></span>

|<span data-ttu-id="97efc-108">属性</span><span class="sxs-lookup"><span data-stu-id="97efc-108">Property</span></span>|<span data-ttu-id="97efc-109">类型</span><span class="sxs-lookup"><span data-stu-id="97efc-109">Type</span></span>|<span data-ttu-id="97efc-110">说明</span><span class="sxs-lookup"><span data-stu-id="97efc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97efc-111">id</span><span class="sxs-lookup"><span data-stu-id="97efc-111">id</span></span>|<span data-ttu-id="97efc-112">String</span><span class="sxs-lookup"><span data-stu-id="97efc-112">String</span></span>|<span data-ttu-id="97efc-113">唯一的呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="97efc-113">Unique call identifier.</span></span> <span data-ttu-id="97efc-114">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="97efc-114">GUID.</span></span>|
|<span data-ttu-id="97efc-115">callId</span><span class="sxs-lookup"><span data-stu-id="97efc-115">callId</span></span>|<span data-ttu-id="97efc-116">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-116">String</span></span>|<span data-ttu-id="97efc-117">呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="97efc-117">Call identifier.</span></span> <span data-ttu-id="97efc-118">不保证是唯一的。</span><span class="sxs-lookup"><span data-stu-id="97efc-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="97efc-119">userId</span><span class="sxs-lookup"><span data-stu-id="97efc-119">userId</span></span>|<span data-ttu-id="97efc-120">String</span><span class="sxs-lookup"><span data-stu-id="97efc-120">String</span></span>|<span data-ttu-id="97efc-121">在 Graph 中调用用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="97efc-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="97efc-122">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="97efc-122">GUID.</span></span> <span data-ttu-id="97efc-123">对于 bot 呼叫类型（ucap_in、ucap_out），此信息和其他用户信息将为 null/空。</span><span class="sxs-lookup"><span data-stu-id="97efc-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="97efc-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97efc-124">userPrincipalName</span></span>|<span data-ttu-id="97efc-125">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-125">String</span></span>|<span data-ttu-id="97efc-126">Azure Active Directory 中的 UserPrincipalName （登录名）。</span><span class="sxs-lookup"><span data-stu-id="97efc-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="97efc-127">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="97efc-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="97efc-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="97efc-128">userDisplayName</span></span>|<span data-ttu-id="97efc-129">String</span><span class="sxs-lookup"><span data-stu-id="97efc-129">String</span></span>|<span data-ttu-id="97efc-130">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="97efc-130">Display name of the user.</span></span>|
|<span data-ttu-id="97efc-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="97efc-131">startDateTime</span></span>|<span data-ttu-id="97efc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97efc-132">DateTimeOffset</span></span>|<span data-ttu-id="97efc-133">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="97efc-133">Call start time.</span></span>|
|<span data-ttu-id="97efc-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="97efc-134">endDateTime</span></span>|<span data-ttu-id="97efc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97efc-135">DateTimeOffset</span></span>|<span data-ttu-id="97efc-136">呼叫结束时间。</span><span class="sxs-lookup"><span data-stu-id="97efc-136">Call end time.</span></span>|
|<span data-ttu-id="97efc-137">duration</span><span class="sxs-lookup"><span data-stu-id="97efc-137">duration</span></span>|<span data-ttu-id="97efc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="97efc-138">Int32</span></span>|<span data-ttu-id="97efc-139">呼叫的连接时间，以秒为单位。</span><span class="sxs-lookup"><span data-stu-id="97efc-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="97efc-140">帐</span><span class="sxs-lookup"><span data-stu-id="97efc-140">charge</span></span>|<span data-ttu-id="97efc-141">双精度</span><span class="sxs-lookup"><span data-stu-id="97efc-141">Double</span></span>|<span data-ttu-id="97efc-142">向您的帐户收取的通话的金额或成本。</span><span class="sxs-lookup"><span data-stu-id="97efc-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="97efc-143">callType</span><span class="sxs-lookup"><span data-stu-id="97efc-143">callType</span></span>|<span data-ttu-id="97efc-144">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-144">String</span></span>|<span data-ttu-id="97efc-145">呼叫是 PSTN 出站呼叫还是入站呼叫，例如用户发出的呼叫或音频会议的呼叫类型。</span><span class="sxs-lookup"><span data-stu-id="97efc-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="97efc-146">currency</span><span class="sxs-lookup"><span data-stu-id="97efc-146">currency</span></span>|<span data-ttu-id="97efc-147">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-147">String</span></span>|<span data-ttu-id="97efc-148">用于计算呼叫开销的货币类型（[ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)）。</span><span class="sxs-lookup"><span data-stu-id="97efc-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="97efc-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="97efc-149">calleeNumber</span></span>|<span data-ttu-id="97efc-150">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-150">String</span></span>|<span data-ttu-id="97efc-151">以[164](https://en.wikipedia.org/wiki/E.164)格式拨打的号码。</span><span class="sxs-lookup"><span data-stu-id="97efc-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="97efc-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="97efc-152">usageCountryCode</span></span>|<span data-ttu-id="97efc-153">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-153">String</span></span>|<span data-ttu-id="97efc-154">用户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="97efc-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="97efc-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="97efc-155">tenantCountryCode</span></span>|<span data-ttu-id="97efc-156">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-156">String</span></span>|<span data-ttu-id="97efc-157">租户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="97efc-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="97efc-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="97efc-158">connectionCharge</span></span>|<span data-ttu-id="97efc-159">双精度</span><span class="sxs-lookup"><span data-stu-id="97efc-159">Double</span></span>|<span data-ttu-id="97efc-160">连接费价格。</span><span class="sxs-lookup"><span data-stu-id="97efc-160">Connection fee price.</span></span>|
|<span data-ttu-id="97efc-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="97efc-161">callerNumber</span></span>|<span data-ttu-id="97efc-162">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-162">String</span></span>|<span data-ttu-id="97efc-163">为入站呼叫接收呼叫或拨打出站呼叫的电话号码的号码。</span><span class="sxs-lookup"><span data-stu-id="97efc-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="97efc-164">. 164 格式。</span><span class="sxs-lookup"><span data-stu-id="97efc-164">E.164 format.</span></span>|
|<span data-ttu-id="97efc-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="97efc-165">destinationContext</span></span>|<span data-ttu-id="97efc-166">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-166">String</span></span>|<span data-ttu-id="97efc-167">呼叫是国内的（在国家或地区内）还是国际（在国家或地区之外）基于用户的位置。</span><span class="sxs-lookup"><span data-stu-id="97efc-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="97efc-168">destinationName</span><span class="sxs-lookup"><span data-stu-id="97efc-168">destinationName</span></span>|<span data-ttu-id="97efc-169">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-169">String</span></span>|<span data-ttu-id="97efc-170">拨打的国家或地区。</span><span class="sxs-lookup"><span data-stu-id="97efc-170">Country or region dialed.</span></span>|
|<span data-ttu-id="97efc-171">conferenceId</span><span class="sxs-lookup"><span data-stu-id="97efc-171">conferenceId</span></span>|<span data-ttu-id="97efc-172">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-172">String</span></span>|<span data-ttu-id="97efc-173">音频会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="97efc-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="97efc-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="97efc-174">licenseCapability</span></span>|<span data-ttu-id="97efc-175">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-175">String</span></span>|<span data-ttu-id="97efc-176">用于呼叫的许可证。</span><span class="sxs-lookup"><span data-stu-id="97efc-176">The license used for the call.</span></span>|
|<span data-ttu-id="97efc-177">inventoryType</span><span class="sxs-lookup"><span data-stu-id="97efc-177">inventoryType</span></span>|<span data-ttu-id="97efc-178">字符串</span><span class="sxs-lookup"><span data-stu-id="97efc-178">String</span></span>|<span data-ttu-id="97efc-179">用户的电话号码类型，如免费电话号码的服务。</span><span class="sxs-lookup"><span data-stu-id="97efc-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97efc-180">关系</span><span class="sxs-lookup"><span data-stu-id="97efc-180">Relationships</span></span>

<span data-ttu-id="97efc-181">无。</span><span class="sxs-lookup"><span data-stu-id="97efc-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97efc-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97efc-182">JSON representation</span></span>

<span data-ttu-id="97efc-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97efc-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```
