---
title: pstnCallLogRow 资源类型
description: 代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 584efcd6e320a95dc6e62f59b112d1041535f054
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697170"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="23886-103">pstnCallLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="23886-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="23886-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="23886-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23886-105">代表公用电话交换网或 PSTN 呼叫日志中 (一) 行。</span><span class="sxs-lookup"><span data-stu-id="23886-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="23886-106">每行映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="23886-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="23886-107">属性</span><span class="sxs-lookup"><span data-stu-id="23886-107">Properties</span></span>

|<span data-ttu-id="23886-108">属性</span><span class="sxs-lookup"><span data-stu-id="23886-108">Property</span></span>|<span data-ttu-id="23886-109">类型</span><span class="sxs-lookup"><span data-stu-id="23886-109">Type</span></span>|<span data-ttu-id="23886-110">说明</span><span class="sxs-lookup"><span data-stu-id="23886-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23886-111">callDurationSource</span><span class="sxs-lookup"><span data-stu-id="23886-111">callDurationSource</span></span>|<span data-ttu-id="23886-112">pstnCallDurationSource</span><span class="sxs-lookup"><span data-stu-id="23886-112">pstnCallDurationSource</span></span>|<span data-ttu-id="23886-113">呼叫持续时间数据源。</span><span class="sxs-lookup"><span data-stu-id="23886-113">The source of the call duration data.</span></span> <span data-ttu-id="23886-114">如果呼叫通过 Operator Connect 计划使用第三方电信运营商，则运营商可能会提供其自己的呼叫持续时间数据。</span><span class="sxs-lookup"><span data-stu-id="23886-114">If the call uses a third-party telecommunications operator via the Operator Connect Program, the operator may provide their own call duration data.</span></span> <span data-ttu-id="23886-115">在这种情况下，属性值为 `operator` 。</span><span class="sxs-lookup"><span data-stu-id="23886-115">In this case, the property value is `operator`.</span></span> <span data-ttu-id="23886-116">否则，值为 `microsoft` 。</span><span class="sxs-lookup"><span data-stu-id="23886-116">Otherwise, the value is `microsoft`.</span></span>|
|<span data-ttu-id="23886-117">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="23886-117">calleeNumber</span></span>|<span data-ttu-id="23886-118">String</span><span class="sxs-lookup"><span data-stu-id="23886-118">String</span></span>|<span data-ttu-id="23886-119">以 [E.164 格式拨打的](https://en.wikipedia.org/wiki/E.164) 号码。</span><span class="sxs-lookup"><span data-stu-id="23886-119">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="23886-120">callerNumber</span><span class="sxs-lookup"><span data-stu-id="23886-120">callerNumber</span></span>|<span data-ttu-id="23886-121">String</span><span class="sxs-lookup"><span data-stu-id="23886-121">String</span></span>|<span data-ttu-id="23886-122">接收入站呼叫呼叫的号码或为出站呼叫拨打的号码。</span><span class="sxs-lookup"><span data-stu-id="23886-122">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="23886-123">E.164 格式。</span><span class="sxs-lookup"><span data-stu-id="23886-123">E.164 format.</span></span>|
|<span data-ttu-id="23886-124">callId</span><span class="sxs-lookup"><span data-stu-id="23886-124">callId</span></span>|<span data-ttu-id="23886-125">String</span><span class="sxs-lookup"><span data-stu-id="23886-125">String</span></span>|<span data-ttu-id="23886-126">呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="23886-126">Call identifier.</span></span> <span data-ttu-id="23886-127">不保证是唯一的。</span><span class="sxs-lookup"><span data-stu-id="23886-127">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="23886-128">callType</span><span class="sxs-lookup"><span data-stu-id="23886-128">callType</span></span>|<span data-ttu-id="23886-129">String</span><span class="sxs-lookup"><span data-stu-id="23886-129">String</span></span>|<span data-ttu-id="23886-130">该呼叫是 PSTN 出站呼叫还是入站呼叫以及呼叫类型，例如用户拨打的呼叫还是音频会议呼叫。</span><span class="sxs-lookup"><span data-stu-id="23886-130">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="23886-131">charge</span><span class="sxs-lookup"><span data-stu-id="23886-131">charge</span></span>|<span data-ttu-id="23886-132">双精度</span><span class="sxs-lookup"><span data-stu-id="23886-132">Double</span></span>|<span data-ttu-id="23886-133">向你的帐户收取的呼叫的金额或费用。</span><span class="sxs-lookup"><span data-stu-id="23886-133">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="23886-134">conferenceId</span><span class="sxs-lookup"><span data-stu-id="23886-134">conferenceId</span></span>|<span data-ttu-id="23886-135">String</span><span class="sxs-lookup"><span data-stu-id="23886-135">String</span></span>|<span data-ttu-id="23886-136">音频会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="23886-136">ID of the audio conference.</span></span>|
|<span data-ttu-id="23886-137">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="23886-137">connectionCharge</span></span>|<span data-ttu-id="23886-138">双精度</span><span class="sxs-lookup"><span data-stu-id="23886-138">Double</span></span>|<span data-ttu-id="23886-139">连接费用价格。</span><span class="sxs-lookup"><span data-stu-id="23886-139">Connection fee price.</span></span>|
|<span data-ttu-id="23886-140">currency</span><span class="sxs-lookup"><span data-stu-id="23886-140">currency</span></span>|<span data-ttu-id="23886-141">String</span><span class="sxs-lookup"><span data-stu-id="23886-141">String</span></span>|<span data-ttu-id="23886-142">用于计算 [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) (开销的货币) 。</span><span class="sxs-lookup"><span data-stu-id="23886-142">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="23886-143">destinationContext</span><span class="sxs-lookup"><span data-stu-id="23886-143">destinationContext</span></span>|<span data-ttu-id="23886-144">String</span><span class="sxs-lookup"><span data-stu-id="23886-144">String</span></span>|<span data-ttu-id="23886-145">呼叫是国内呼叫 (或地区内) 或 (或地区外部的) 用户位置进行呼叫。</span><span class="sxs-lookup"><span data-stu-id="23886-145">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="23886-146">destinationName</span><span class="sxs-lookup"><span data-stu-id="23886-146">destinationName</span></span>|<span data-ttu-id="23886-147">String</span><span class="sxs-lookup"><span data-stu-id="23886-147">String</span></span>|<span data-ttu-id="23886-148">拨打的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="23886-148">Country or region dialed.</span></span>|
|<span data-ttu-id="23886-149">duration</span><span class="sxs-lookup"><span data-stu-id="23886-149">duration</span></span>|<span data-ttu-id="23886-150">Int32</span><span class="sxs-lookup"><span data-stu-id="23886-150">Int32</span></span>|<span data-ttu-id="23886-151">呼叫连接时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="23886-151">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="23886-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="23886-152">endDateTime</span></span>|<span data-ttu-id="23886-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23886-153">DateTimeOffset</span></span>|<span data-ttu-id="23886-154">呼叫结束时间。</span><span class="sxs-lookup"><span data-stu-id="23886-154">Call end time.</span></span>|
|<span data-ttu-id="23886-155">id</span><span class="sxs-lookup"><span data-stu-id="23886-155">id</span></span>|<span data-ttu-id="23886-156">String</span><span class="sxs-lookup"><span data-stu-id="23886-156">String</span></span>|<span data-ttu-id="23886-157">唯一呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="23886-157">Unique call identifier.</span></span> <span data-ttu-id="23886-158">GUID。</span><span class="sxs-lookup"><span data-stu-id="23886-158">GUID.</span></span>|
|<span data-ttu-id="23886-159">inventoryType</span><span class="sxs-lookup"><span data-stu-id="23886-159">inventoryType</span></span>|<span data-ttu-id="23886-160">String</span><span class="sxs-lookup"><span data-stu-id="23886-160">String</span></span>|<span data-ttu-id="23886-161">用户的电话号码类型，如免费电话号码服务。</span><span class="sxs-lookup"><span data-stu-id="23886-161">User's phone number type, such as a service of toll-free number.</span></span>|
|<span data-ttu-id="23886-162">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="23886-162">licenseCapability</span></span>|<span data-ttu-id="23886-163">String</span><span class="sxs-lookup"><span data-stu-id="23886-163">String</span></span>|<span data-ttu-id="23886-164">用于呼叫的许可证。</span><span class="sxs-lookup"><span data-stu-id="23886-164">The license used for the call.</span></span>|
|<span data-ttu-id="23886-165">operator</span><span class="sxs-lookup"><span data-stu-id="23886-165">operator</span></span>|<span data-ttu-id="23886-166">String</span><span class="sxs-lookup"><span data-stu-id="23886-166">String</span></span>|<span data-ttu-id="23886-167">为此呼叫提供 PSTN 服务的电信运营商。</span><span class="sxs-lookup"><span data-stu-id="23886-167">The telecommunications operator which provided PSTN services for this call.</span></span> <span data-ttu-id="23886-168">这可能是 Microsoft，或者可能是通过 Operator Connect Program 的第三 [方运营商](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)。</span><span class="sxs-lookup"><span data-stu-id="23886-168">This may be Microsoft, or it may be a third-party operator via the [Operator Connect Program](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398).</span></span>|
|<span data-ttu-id="23886-169">startDateTime</span><span class="sxs-lookup"><span data-stu-id="23886-169">startDateTime</span></span>|<span data-ttu-id="23886-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23886-170">DateTimeOffset</span></span>|<span data-ttu-id="23886-171">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="23886-171">Call start time.</span></span>|
|<span data-ttu-id="23886-172">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="23886-172">tenantCountryCode</span></span>|<span data-ttu-id="23886-173">String</span><span class="sxs-lookup"><span data-stu-id="23886-173">String</span></span>|<span data-ttu-id="23886-174">租户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="23886-174">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="23886-175">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="23886-175">usageCountryCode</span></span>|<span data-ttu-id="23886-176">String</span><span class="sxs-lookup"><span data-stu-id="23886-176">String</span></span>|<span data-ttu-id="23886-177">用户的国家/地区代码 [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="23886-177">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="23886-178">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="23886-178">userDisplayName</span></span>|<span data-ttu-id="23886-179">String</span><span class="sxs-lookup"><span data-stu-id="23886-179">String</span></span>|<span data-ttu-id="23886-180">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="23886-180">Display name of the user.</span></span>|
|<span data-ttu-id="23886-181">userId</span><span class="sxs-lookup"><span data-stu-id="23886-181">userId</span></span>|<span data-ttu-id="23886-182">String</span><span class="sxs-lookup"><span data-stu-id="23886-182">String</span></span>|<span data-ttu-id="23886-183">在 Graph 中调用用户 ID。</span><span class="sxs-lookup"><span data-stu-id="23886-183">Calling user's ID in Graph.</span></span> <span data-ttu-id="23886-184">GUID。</span><span class="sxs-lookup"><span data-stu-id="23886-184">GUID.</span></span> <span data-ttu-id="23886-185">对于自动程序呼叫类型，此信息和其他用户信息将为 null/空 (ucap_in ucap_out) 。</span><span class="sxs-lookup"><span data-stu-id="23886-185">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="23886-186">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23886-186">userPrincipalName</span></span>|<span data-ttu-id="23886-187">String</span><span class="sxs-lookup"><span data-stu-id="23886-187">String</span></span>|<span data-ttu-id="23886-188">UserPrincipalName (Azure Active Directory) 登录名。</span><span class="sxs-lookup"><span data-stu-id="23886-188">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="23886-189">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="23886-189">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23886-190">关系</span><span class="sxs-lookup"><span data-stu-id="23886-190">Relationships</span></span>

<span data-ttu-id="23886-191">无。</span><span class="sxs-lookup"><span data-stu-id="23886-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23886-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23886-192">JSON representation</span></span>

<span data-ttu-id="23886-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23886-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


