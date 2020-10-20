---
title: pstnCallLogRow 资源类型
description: 表示公共交换机电话网络 (PSTN) 呼叫日志中的数据行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc83f3304eeb918d665b2651fda9809fd8a05880
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601669"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="59a6a-103">pstnCallLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="59a6a-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="59a6a-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="59a6a-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59a6a-105">表示公共交换机电话网络 (PSTN) 呼叫日志中的数据行。</span><span class="sxs-lookup"><span data-stu-id="59a6a-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="59a6a-106">每行都映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="59a6a-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="59a6a-107">属性</span><span class="sxs-lookup"><span data-stu-id="59a6a-107">Properties</span></span>

|<span data-ttu-id="59a6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="59a6a-108">Property</span></span>|<span data-ttu-id="59a6a-109">类型</span><span class="sxs-lookup"><span data-stu-id="59a6a-109">Type</span></span>|<span data-ttu-id="59a6a-110">说明</span><span class="sxs-lookup"><span data-stu-id="59a6a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a6a-111">id</span><span class="sxs-lookup"><span data-stu-id="59a6a-111">id</span></span>|<span data-ttu-id="59a6a-112">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-112">String</span></span>|<span data-ttu-id="59a6a-113">唯一的呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="59a6a-113">Unique call identifier.</span></span> <span data-ttu-id="59a6a-114">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="59a6a-114">GUID.</span></span>|
|<span data-ttu-id="59a6a-115">callId</span><span class="sxs-lookup"><span data-stu-id="59a6a-115">callId</span></span>|<span data-ttu-id="59a6a-116">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-116">String</span></span>|<span data-ttu-id="59a6a-117">呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="59a6a-117">Call identifier.</span></span> <span data-ttu-id="59a6a-118">不保证是唯一的。</span><span class="sxs-lookup"><span data-stu-id="59a6a-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="59a6a-119">userId</span><span class="sxs-lookup"><span data-stu-id="59a6a-119">userId</span></span>|<span data-ttu-id="59a6a-120">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-120">String</span></span>|<span data-ttu-id="59a6a-121">在 Graph 中调用用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="59a6a-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="59a6a-122">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="59a6a-122">GUID.</span></span> <span data-ttu-id="59a6a-123">对于 bot 呼叫类型 (ucap_in ucap_out) ，此信息和其他用户信息将为 null/空。</span><span class="sxs-lookup"><span data-stu-id="59a6a-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="59a6a-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="59a6a-124">userPrincipalName</span></span>|<span data-ttu-id="59a6a-125">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-125">String</span></span>|<span data-ttu-id="59a6a-126">在 Azure Active Directory 中) 的 UserPrincipalName (登录名。</span><span class="sxs-lookup"><span data-stu-id="59a6a-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="59a6a-127">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="59a6a-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="59a6a-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="59a6a-128">userDisplayName</span></span>|<span data-ttu-id="59a6a-129">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-129">String</span></span>|<span data-ttu-id="59a6a-130">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="59a6a-130">Display name of the user.</span></span>|
|<span data-ttu-id="59a6a-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59a6a-131">startDateTime</span></span>|<span data-ttu-id="59a6a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a6a-132">DateTimeOffset</span></span>|<span data-ttu-id="59a6a-133">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="59a6a-133">Call start time.</span></span>|
|<span data-ttu-id="59a6a-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59a6a-134">endDateTime</span></span>|<span data-ttu-id="59a6a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a6a-135">DateTimeOffset</span></span>|<span data-ttu-id="59a6a-136">呼叫结束时间。</span><span class="sxs-lookup"><span data-stu-id="59a6a-136">Call end time.</span></span>|
|<span data-ttu-id="59a6a-137">duration</span><span class="sxs-lookup"><span data-stu-id="59a6a-137">duration</span></span>|<span data-ttu-id="59a6a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="59a6a-138">Int32</span></span>|<span data-ttu-id="59a6a-139">呼叫的连接时间，以秒为单位。</span><span class="sxs-lookup"><span data-stu-id="59a6a-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="59a6a-140">帐</span><span class="sxs-lookup"><span data-stu-id="59a6a-140">charge</span></span>|<span data-ttu-id="59a6a-141">双精度</span><span class="sxs-lookup"><span data-stu-id="59a6a-141">Double</span></span>|<span data-ttu-id="59a6a-142">向您的帐户收取的通话的金额或成本。</span><span class="sxs-lookup"><span data-stu-id="59a6a-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="59a6a-143">callType</span><span class="sxs-lookup"><span data-stu-id="59a6a-143">callType</span></span>|<span data-ttu-id="59a6a-144">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-144">String</span></span>|<span data-ttu-id="59a6a-145">呼叫是 PSTN 出站呼叫还是入站呼叫，例如用户发出的呼叫或音频会议的呼叫类型。</span><span class="sxs-lookup"><span data-stu-id="59a6a-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="59a6a-146">currency</span><span class="sxs-lookup"><span data-stu-id="59a6a-146">currency</span></span>|<span data-ttu-id="59a6a-147">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-147">String</span></span>|<span data-ttu-id="59a6a-148">用于计算 ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)) 的呼叫成本的货币类型。</span><span class="sxs-lookup"><span data-stu-id="59a6a-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="59a6a-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="59a6a-149">calleeNumber</span></span>|<span data-ttu-id="59a6a-150">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-150">String</span></span>|<span data-ttu-id="59a6a-151">以 [164](https://en.wikipedia.org/wiki/E.164) 格式拨打的号码。</span><span class="sxs-lookup"><span data-stu-id="59a6a-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="59a6a-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="59a6a-152">usageCountryCode</span></span>|<span data-ttu-id="59a6a-153">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-153">String</span></span>|<span data-ttu-id="59a6a-154">用户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="59a6a-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="59a6a-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="59a6a-155">tenantCountryCode</span></span>|<span data-ttu-id="59a6a-156">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-156">String</span></span>|<span data-ttu-id="59a6a-157">租户的国家/地区代码， [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="59a6a-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="59a6a-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="59a6a-158">connectionCharge</span></span>|<span data-ttu-id="59a6a-159">双精度</span><span class="sxs-lookup"><span data-stu-id="59a6a-159">Double</span></span>|<span data-ttu-id="59a6a-160">连接费价格。</span><span class="sxs-lookup"><span data-stu-id="59a6a-160">Connection fee price.</span></span>|
|<span data-ttu-id="59a6a-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="59a6a-161">callerNumber</span></span>|<span data-ttu-id="59a6a-162">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-162">String</span></span>|<span data-ttu-id="59a6a-163">为入站呼叫接收呼叫或拨打出站呼叫的电话号码的号码。</span><span class="sxs-lookup"><span data-stu-id="59a6a-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="59a6a-164">. 164 格式。</span><span class="sxs-lookup"><span data-stu-id="59a6a-164">E.164 format.</span></span>|
|<span data-ttu-id="59a6a-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="59a6a-165">destinationContext</span></span>|<span data-ttu-id="59a6a-166">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-166">String</span></span>|<span data-ttu-id="59a6a-167">呼叫是否为国家或地区内 () 或国际 (之外的国家或地区) 基于用户的位置。</span><span class="sxs-lookup"><span data-stu-id="59a6a-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="59a6a-168">destinationName</span><span class="sxs-lookup"><span data-stu-id="59a6a-168">destinationName</span></span>|<span data-ttu-id="59a6a-169">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-169">String</span></span>|<span data-ttu-id="59a6a-170">拨打的国家或地区。</span><span class="sxs-lookup"><span data-stu-id="59a6a-170">Country or region dialed.</span></span>|
|<span data-ttu-id="59a6a-171">conferenceId</span><span class="sxs-lookup"><span data-stu-id="59a6a-171">conferenceId</span></span>|<span data-ttu-id="59a6a-172">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-172">String</span></span>|<span data-ttu-id="59a6a-173">音频会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="59a6a-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="59a6a-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="59a6a-174">licenseCapability</span></span>|<span data-ttu-id="59a6a-175">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-175">String</span></span>|<span data-ttu-id="59a6a-176">用于呼叫的许可证。</span><span class="sxs-lookup"><span data-stu-id="59a6a-176">The license used for the call.</span></span>|
|<span data-ttu-id="59a6a-177">inventoryType</span><span class="sxs-lookup"><span data-stu-id="59a6a-177">inventoryType</span></span>|<span data-ttu-id="59a6a-178">String</span><span class="sxs-lookup"><span data-stu-id="59a6a-178">String</span></span>|<span data-ttu-id="59a6a-179">用户的电话号码类型，如免费电话号码的服务。</span><span class="sxs-lookup"><span data-stu-id="59a6a-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59a6a-180">关系</span><span class="sxs-lookup"><span data-stu-id="59a6a-180">Relationships</span></span>

<span data-ttu-id="59a6a-181">无。</span><span class="sxs-lookup"><span data-stu-id="59a6a-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59a6a-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59a6a-182">JSON representation</span></span>

<span data-ttu-id="59a6a-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59a6a-183">The following is a JSON representation of the resource.</span></span>

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


