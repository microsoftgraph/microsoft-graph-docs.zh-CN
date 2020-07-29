---
title: directRoutingLogRow 资源类型
description: 表示直接路由呼叫日志中的数据行。
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a01ed8410532264fceb0164ef4f703b636ccdef
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510164"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="4e3ad-103">directRoutingLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e3ad-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="4e3ad-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4e3ad-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e3ad-105">表示直接路由呼叫日志中的数据行。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="4e3ad-106">每行都映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="4e3ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e3ad-107">Properties</span></span>

|<span data-ttu-id="4e3ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e3ad-108">Property</span></span>|<span data-ttu-id="4e3ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e3ad-109">Type</span></span>|<span data-ttu-id="4e3ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e3ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3ad-111">id</span><span class="sxs-lookup"><span data-stu-id="4e3ad-111">id</span></span>|<span data-ttu-id="4e3ad-112">String</span><span class="sxs-lookup"><span data-stu-id="4e3ad-112">String</span></span>|<span data-ttu-id="4e3ad-113">唯一的呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-113">Unique call identifier.</span></span> <span data-ttu-id="4e3ad-114">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-114">GUID.</span></span>|
|<span data-ttu-id="4e3ad-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="4e3ad-115">correlationId</span></span>|<span data-ttu-id="4e3ad-116">String</span><span class="sxs-lookup"><span data-stu-id="4e3ad-116">String</span></span>|<span data-ttu-id="4e3ad-117">调用 Microsoft 支持时可使用的呼叫的标识符。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="4e3ad-118">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-118">GUID.</span></span>|
|<span data-ttu-id="4e3ad-119">userId</span><span class="sxs-lookup"><span data-stu-id="4e3ad-119">userId</span></span>|<span data-ttu-id="4e3ad-120">String</span><span class="sxs-lookup"><span data-stu-id="4e3ad-120">String</span></span>|<span data-ttu-id="4e3ad-121">在 Graph 中调用用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="4e3ad-122">对于 bot 呼叫类型，此信息和其他用户信息将为 null/空。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="4e3ad-123">Containerparentjob.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-123">GUID.</span></span>|
|<span data-ttu-id="4e3ad-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e3ad-124">userPrincipalName</span></span>|<span data-ttu-id="4e3ad-125">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-125">String</span></span>|<span data-ttu-id="4e3ad-126">Azure Active Directory 中的 UserPrincipalName （登录名）。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="4e3ad-127">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="4e3ad-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4e3ad-128">userDisplayName</span></span>|<span data-ttu-id="4e3ad-129">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-129">String</span></span>|<span data-ttu-id="4e3ad-130">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-130">Display name of the user.</span></span>|
|<span data-ttu-id="4e3ad-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e3ad-131">startDateTime</span></span>|<span data-ttu-id="4e3ad-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e3ad-132">DateTimeOffset</span></span>|<span data-ttu-id="4e3ad-133">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-133">Call start time.</span></span><br/><span data-ttu-id="4e3ad-134">对于失败和未应答的呼叫，这可能等于 "邀请" 或 "失败时间"。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="4e3ad-135">inviteDateTime</span><span class="sxs-lookup"><span data-stu-id="4e3ad-135">inviteDateTime</span></span>|<span data-ttu-id="4e3ad-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e3ad-136">DateTimeOffset</span></span>| <span data-ttu-id="4e3ad-137">发送初始邀请时。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="4e3ad-138">failureDateTime</span><span class="sxs-lookup"><span data-stu-id="4e3ad-138">failureDateTime</span></span>|<span data-ttu-id="4e3ad-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e3ad-139">DateTimeOffset</span></span>| <span data-ttu-id="4e3ad-140">仅存在失败（未完全建立）呼叫的情况。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="4e3ad-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4e3ad-141">endDateTime</span></span>|<span data-ttu-id="4e3ad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e3ad-142">DateTimeOffset</span></span>| <span data-ttu-id="4e3ad-143">仅存在成功（完全建立）的呼叫。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="4e3ad-144">呼叫结束的时间。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-144">Time when call ended.</span></span>|
|<span data-ttu-id="4e3ad-145">duration</span><span class="sxs-lookup"><span data-stu-id="4e3ad-145">duration</span></span>|<span data-ttu-id="4e3ad-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4e3ad-146">Int32</span></span>| <span data-ttu-id="4e3ad-147">呼叫的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="4e3ad-148">callType</span><span class="sxs-lookup"><span data-stu-id="4e3ad-148">callType</span></span>|<span data-ttu-id="4e3ad-149">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-149">String</span></span>| <span data-ttu-id="4e3ad-150">呼叫类型和方向。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-150">Call type and direction.</span></span>|
|<span data-ttu-id="4e3ad-151">successfulCall</span><span class="sxs-lookup"><span data-stu-id="4e3ad-151">successfulCall</span></span>|<span data-ttu-id="4e3ad-152">布尔</span><span class="sxs-lookup"><span data-stu-id="4e3ad-152">Boolean</span></span>| <span data-ttu-id="4e3ad-153">成功或尝试。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-153">Success or attempt.</span></span>|
|<span data-ttu-id="4e3ad-154">callerNumber</span><span class="sxs-lookup"><span data-stu-id="4e3ad-154">callerNumber</span></span>|<span data-ttu-id="4e3ad-155">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-155">String</span></span>| <span data-ttu-id="4e3ad-156">发出呼叫的用户或机器人的号码。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="4e3ad-157">E.164[格式，](https://en.wikipedia.org/wiki/E.164)但可能包含其他数据。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="4e3ad-158">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="4e3ad-158">calleeNumber</span></span>|<span data-ttu-id="4e3ad-159">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-159">String</span></span>| <span data-ttu-id="4e3ad-160">接收呼叫的用户或机器人的号码。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="4e3ad-161">E.164[格式，](https://en.wikipedia.org/wiki/E.164)但可能包含其他数据。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="4e3ad-162">mediaPathLocation</span><span class="sxs-lookup"><span data-stu-id="4e3ad-162">mediaPathLocation</span></span>|<span data-ttu-id="4e3ad-163">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-163">String</span></span>| <span data-ttu-id="4e3ad-164">用于非旁路呼叫中的媒体路径的数据中心。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="4e3ad-165">signalingLocation</span><span class="sxs-lookup"><span data-stu-id="4e3ad-165">signalingLocation</span></span>|<span data-ttu-id="4e3ad-166">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-166">String</span></span>| <span data-ttu-id="4e3ad-167">用于对绕过和非绕过呼叫发出信号的数据中心。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="4e3ad-168">finalSipCode</span><span class="sxs-lookup"><span data-stu-id="4e3ad-168">finalSipCode</span></span>|<span data-ttu-id="4e3ad-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4e3ad-169">Int32</span></span>| <span data-ttu-id="4e3ad-170">调用结束的代码（ [RFC 3261](https://tools.ietf.org/html/rfc3261)）。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="4e3ad-171">callEndSubReason</span><span class="sxs-lookup"><span data-stu-id="4e3ad-171">callEndSubReason</span></span>|<span data-ttu-id="4e3ad-172">Int32</span><span class="sxs-lookup"><span data-stu-id="4e3ad-172">Int32</span></span>| <span data-ttu-id="4e3ad-173">除了 SIP 代码之外，Microsoft 还提供了指示特定问题的子代码。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="4e3ad-174">finalSipCodePhrase</span><span class="sxs-lookup"><span data-stu-id="4e3ad-174">finalSipCodePhrase</span></span>|<span data-ttu-id="4e3ad-175">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-175">String</span></span>| <span data-ttu-id="4e3ad-176">SIP 代码和 Microsoft 子代码的说明。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="4e3ad-177">trunkFullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="4e3ad-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="4e3ad-178">字符串</span><span class="sxs-lookup"><span data-stu-id="4e3ad-178">String</span></span>| <span data-ttu-id="4e3ad-179">会话边界控制器的完全限定的域名称。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="4e3ad-180">mediaBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="4e3ad-180">mediaBypassEnabled</span></span>|<span data-ttu-id="4e3ad-181">布尔</span><span class="sxs-lookup"><span data-stu-id="4e3ad-181">Boolean</span></span>| <span data-ttu-id="4e3ad-182">指示是否为媒体旁路启用了中继。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e3ad-183">关系</span><span class="sxs-lookup"><span data-stu-id="4e3ad-183">Relationships</span></span>

<span data-ttu-id="4e3ad-184">无。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e3ad-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e3ad-185">JSON representation</span></span>

<span data-ttu-id="4e3ad-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e3ad-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```
