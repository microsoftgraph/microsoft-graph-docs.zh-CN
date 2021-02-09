---
title: pstnCallLogRow 资源类型
description: 代表 PSTN 呼叫日志中公用电话交换 (中的) 行。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155578"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="39787-103">pstnCallLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="39787-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="39787-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="39787-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39787-105">代表 PSTN 呼叫日志中公用电话交换 (中的) 行。</span><span class="sxs-lookup"><span data-stu-id="39787-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="39787-106">每行映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="39787-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="39787-107">属性</span><span class="sxs-lookup"><span data-stu-id="39787-107">Properties</span></span>

|<span data-ttu-id="39787-108">属性</span><span class="sxs-lookup"><span data-stu-id="39787-108">Property</span></span>|<span data-ttu-id="39787-109">类型</span><span class="sxs-lookup"><span data-stu-id="39787-109">Type</span></span>|<span data-ttu-id="39787-110">说明</span><span class="sxs-lookup"><span data-stu-id="39787-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39787-111">id</span><span class="sxs-lookup"><span data-stu-id="39787-111">id</span></span>|<span data-ttu-id="39787-112">String</span><span class="sxs-lookup"><span data-stu-id="39787-112">String</span></span>|<span data-ttu-id="39787-113">唯一呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="39787-113">Unique call identifier.</span></span> <span data-ttu-id="39787-114">GUID。</span><span class="sxs-lookup"><span data-stu-id="39787-114">GUID.</span></span>|
|<span data-ttu-id="39787-115">callId</span><span class="sxs-lookup"><span data-stu-id="39787-115">callId</span></span>|<span data-ttu-id="39787-116">String</span><span class="sxs-lookup"><span data-stu-id="39787-116">String</span></span>|<span data-ttu-id="39787-117">呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="39787-117">Call identifier.</span></span> <span data-ttu-id="39787-118">不保证是唯一的。</span><span class="sxs-lookup"><span data-stu-id="39787-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="39787-119">userId</span><span class="sxs-lookup"><span data-stu-id="39787-119">userId</span></span>|<span data-ttu-id="39787-120">String</span><span class="sxs-lookup"><span data-stu-id="39787-120">String</span></span>|<span data-ttu-id="39787-121">在 Graph 中调用用户 ID。</span><span class="sxs-lookup"><span data-stu-id="39787-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="39787-122">GUID。</span><span class="sxs-lookup"><span data-stu-id="39787-122">GUID.</span></span> <span data-ttu-id="39787-123">对于自动程序呼叫类型，此信息和其他用户信息将为 null/ (ucap_in，ucap_out) 。</span><span class="sxs-lookup"><span data-stu-id="39787-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="39787-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39787-124">userPrincipalName</span></span>|<span data-ttu-id="39787-125">String</span><span class="sxs-lookup"><span data-stu-id="39787-125">String</span></span>|<span data-ttu-id="39787-126">UserPrincipalName (Azure Active Directory) 登录名。</span><span class="sxs-lookup"><span data-stu-id="39787-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="39787-127">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="39787-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="39787-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="39787-128">userDisplayName</span></span>|<span data-ttu-id="39787-129">String</span><span class="sxs-lookup"><span data-stu-id="39787-129">String</span></span>|<span data-ttu-id="39787-130">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="39787-130">Display name of the user.</span></span>|
|<span data-ttu-id="39787-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="39787-131">startDateTime</span></span>|<span data-ttu-id="39787-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39787-132">DateTimeOffset</span></span>|<span data-ttu-id="39787-133">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="39787-133">Call start time.</span></span>|
|<span data-ttu-id="39787-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="39787-134">endDateTime</span></span>|<span data-ttu-id="39787-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39787-135">DateTimeOffset</span></span>|<span data-ttu-id="39787-136">呼叫结束时间。</span><span class="sxs-lookup"><span data-stu-id="39787-136">Call end time.</span></span>|
|<span data-ttu-id="39787-137">duration</span><span class="sxs-lookup"><span data-stu-id="39787-137">duration</span></span>|<span data-ttu-id="39787-138">Int32</span><span class="sxs-lookup"><span data-stu-id="39787-138">Int32</span></span>|<span data-ttu-id="39787-139">呼叫连接时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="39787-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="39787-140">charge</span><span class="sxs-lookup"><span data-stu-id="39787-140">charge</span></span>|<span data-ttu-id="39787-141">双精度</span><span class="sxs-lookup"><span data-stu-id="39787-141">Double</span></span>|<span data-ttu-id="39787-142">向你的帐户收取的呼叫的金额或费用。</span><span class="sxs-lookup"><span data-stu-id="39787-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="39787-143">callType</span><span class="sxs-lookup"><span data-stu-id="39787-143">callType</span></span>|<span data-ttu-id="39787-144">String</span><span class="sxs-lookup"><span data-stu-id="39787-144">String</span></span>|<span data-ttu-id="39787-145">呼叫是 PSTN 出站呼叫还是入站呼叫以及呼叫类型，例如用户拨打的呼叫或音频会议。</span><span class="sxs-lookup"><span data-stu-id="39787-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="39787-146">currency</span><span class="sxs-lookup"><span data-stu-id="39787-146">currency</span></span>|<span data-ttu-id="39787-147">String</span><span class="sxs-lookup"><span data-stu-id="39787-147">String</span></span>|<span data-ttu-id="39787-148">用于计算 ISO [4217](https://en.wikipedia.org/wiki/ISO_4217) (呼叫成本的货币) 。</span><span class="sxs-lookup"><span data-stu-id="39787-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="39787-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="39787-149">calleeNumber</span></span>|<span data-ttu-id="39787-150">String</span><span class="sxs-lookup"><span data-stu-id="39787-150">String</span></span>|<span data-ttu-id="39787-151">[E.164 格式](https://en.wikipedia.org/wiki/E.164)拨打的号码。</span><span class="sxs-lookup"><span data-stu-id="39787-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="39787-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="39787-152">usageCountryCode</span></span>|<span data-ttu-id="39787-153">String</span><span class="sxs-lookup"><span data-stu-id="39787-153">String</span></span>|<span data-ttu-id="39787-154">用户的国家/地区代码[，ISO 3166-1 alpha-2。](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)</span><span class="sxs-lookup"><span data-stu-id="39787-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="39787-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="39787-155">tenantCountryCode</span></span>|<span data-ttu-id="39787-156">String</span><span class="sxs-lookup"><span data-stu-id="39787-156">String</span></span>|<span data-ttu-id="39787-157">租户的国家/地区代码 [，ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)。</span><span class="sxs-lookup"><span data-stu-id="39787-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="39787-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="39787-158">connectionCharge</span></span>|<span data-ttu-id="39787-159">双精度</span><span class="sxs-lookup"><span data-stu-id="39787-159">Double</span></span>|<span data-ttu-id="39787-160">连接费用价格。</span><span class="sxs-lookup"><span data-stu-id="39787-160">Connection fee price.</span></span>|
|<span data-ttu-id="39787-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="39787-161">callerNumber</span></span>|<span data-ttu-id="39787-162">String</span><span class="sxs-lookup"><span data-stu-id="39787-162">String</span></span>|<span data-ttu-id="39787-163">接收入站呼叫呼叫的号码或为出站呼叫拨打的号码。</span><span class="sxs-lookup"><span data-stu-id="39787-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="39787-164">E.164 格式。</span><span class="sxs-lookup"><span data-stu-id="39787-164">E.164 format.</span></span>|
|<span data-ttu-id="39787-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="39787-165">destinationContext</span></span>|<span data-ttu-id="39787-166">String</span><span class="sxs-lookup"><span data-stu-id="39787-166">String</span></span>|<span data-ttu-id="39787-167">呼叫是 (国家/地区) ，还是位于 (或) 地理位置之外的国际呼叫。</span><span class="sxs-lookup"><span data-stu-id="39787-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="39787-168">destinationName</span><span class="sxs-lookup"><span data-stu-id="39787-168">destinationName</span></span>|<span data-ttu-id="39787-169">String</span><span class="sxs-lookup"><span data-stu-id="39787-169">String</span></span>|<span data-ttu-id="39787-170">拨打的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="39787-170">Country or region dialed.</span></span>|
|<span data-ttu-id="39787-171">conferenceId</span><span class="sxs-lookup"><span data-stu-id="39787-171">conferenceId</span></span>|<span data-ttu-id="39787-172">String</span><span class="sxs-lookup"><span data-stu-id="39787-172">String</span></span>|<span data-ttu-id="39787-173">音频会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="39787-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="39787-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="39787-174">licenseCapability</span></span>|<span data-ttu-id="39787-175">String</span><span class="sxs-lookup"><span data-stu-id="39787-175">String</span></span>|<span data-ttu-id="39787-176">用于呼叫的许可证。</span><span class="sxs-lookup"><span data-stu-id="39787-176">The license used for the call.</span></span>|
|<span data-ttu-id="39787-177">inventoryType</span><span class="sxs-lookup"><span data-stu-id="39787-177">inventoryType</span></span>|<span data-ttu-id="39787-178">String</span><span class="sxs-lookup"><span data-stu-id="39787-178">String</span></span>|<span data-ttu-id="39787-179">用户的电话号码类型，如免费电话号码服务。</span><span class="sxs-lookup"><span data-stu-id="39787-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39787-180">关系</span><span class="sxs-lookup"><span data-stu-id="39787-180">Relationships</span></span>

<span data-ttu-id="39787-181">无。</span><span class="sxs-lookup"><span data-stu-id="39787-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39787-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39787-182">JSON representation</span></span>

<span data-ttu-id="39787-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39787-183">The following is a JSON representation of the resource.</span></span>

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
  "inventoryType": "String"
}
```


