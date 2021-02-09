---
title: directRoutingLogRow 资源类型
description: 表示直接路由呼叫日志中的一行数据。
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159652"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="62028-103">directRoutingLogRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="62028-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="62028-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="62028-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62028-105">表示直接路由呼叫日志中的一行数据。</span><span class="sxs-lookup"><span data-stu-id="62028-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="62028-106">每行映射到一个调用。</span><span class="sxs-lookup"><span data-stu-id="62028-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="62028-107">属性</span><span class="sxs-lookup"><span data-stu-id="62028-107">Properties</span></span>

|<span data-ttu-id="62028-108">属性</span><span class="sxs-lookup"><span data-stu-id="62028-108">Property</span></span>|<span data-ttu-id="62028-109">类型</span><span class="sxs-lookup"><span data-stu-id="62028-109">Type</span></span>|<span data-ttu-id="62028-110">说明</span><span class="sxs-lookup"><span data-stu-id="62028-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62028-111">id</span><span class="sxs-lookup"><span data-stu-id="62028-111">id</span></span>|<span data-ttu-id="62028-112">String</span><span class="sxs-lookup"><span data-stu-id="62028-112">String</span></span>|<span data-ttu-id="62028-113">唯一呼叫标识符。</span><span class="sxs-lookup"><span data-stu-id="62028-113">Unique call identifier.</span></span> <span data-ttu-id="62028-114">GUID。</span><span class="sxs-lookup"><span data-stu-id="62028-114">GUID.</span></span>|
|<span data-ttu-id="62028-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="62028-115">correlationId</span></span>|<span data-ttu-id="62028-116">String</span><span class="sxs-lookup"><span data-stu-id="62028-116">String</span></span>|<span data-ttu-id="62028-117">调用 Microsoft 支持时可以使用的呼叫的标识符。</span><span class="sxs-lookup"><span data-stu-id="62028-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="62028-118">GUID。</span><span class="sxs-lookup"><span data-stu-id="62028-118">GUID.</span></span>|
|<span data-ttu-id="62028-119">userId</span><span class="sxs-lookup"><span data-stu-id="62028-119">userId</span></span>|<span data-ttu-id="62028-120">String</span><span class="sxs-lookup"><span data-stu-id="62028-120">String</span></span>|<span data-ttu-id="62028-121">在 Graph 中调用用户 ID。</span><span class="sxs-lookup"><span data-stu-id="62028-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="62028-122">对于机器人呼叫类型，此信息和其他用户信息将为 null/空。</span><span class="sxs-lookup"><span data-stu-id="62028-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="62028-123">GUID。</span><span class="sxs-lookup"><span data-stu-id="62028-123">GUID.</span></span>|
|<span data-ttu-id="62028-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62028-124">userPrincipalName</span></span>|<span data-ttu-id="62028-125">String</span><span class="sxs-lookup"><span data-stu-id="62028-125">String</span></span>|<span data-ttu-id="62028-126">UserPrincipalName (Azure Active Directory) 登录名。</span><span class="sxs-lookup"><span data-stu-id="62028-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="62028-127">这通常与用户的 SIP 地址相同，并且可以与用户的电子邮件地址相同。</span><span class="sxs-lookup"><span data-stu-id="62028-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="62028-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="62028-128">userDisplayName</span></span>|<span data-ttu-id="62028-129">String</span><span class="sxs-lookup"><span data-stu-id="62028-129">String</span></span>|<span data-ttu-id="62028-130">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="62028-130">Display name of the user.</span></span>|
|<span data-ttu-id="62028-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="62028-131">startDateTime</span></span>|<span data-ttu-id="62028-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62028-132">DateTimeOffset</span></span>|<span data-ttu-id="62028-133">呼叫开始时间。</span><span class="sxs-lookup"><span data-stu-id="62028-133">Call start time.</span></span><br/><span data-ttu-id="62028-134">对于失败和未接听的呼叫，这等于邀请或失败时间。</span><span class="sxs-lookup"><span data-stu-id="62028-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="62028-135">inviteDateTime</span><span class="sxs-lookup"><span data-stu-id="62028-135">inviteDateTime</span></span>|<span data-ttu-id="62028-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62028-136">DateTimeOffset</span></span>| <span data-ttu-id="62028-137">发送初始邀请时。</span><span class="sxs-lookup"><span data-stu-id="62028-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="62028-138">failureDateTime</span><span class="sxs-lookup"><span data-stu-id="62028-138">failureDateTime</span></span>|<span data-ttu-id="62028-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62028-139">DateTimeOffset</span></span>| <span data-ttu-id="62028-140">仅对未完全建立 (失败) 存在。</span><span class="sxs-lookup"><span data-stu-id="62028-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="62028-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="62028-141">endDateTime</span></span>|<span data-ttu-id="62028-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62028-142">DateTimeOffset</span></span>| <span data-ttu-id="62028-143">只有成功建立 (调用) 存在。</span><span class="sxs-lookup"><span data-stu-id="62028-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="62028-144">呼叫结束的时间。</span><span class="sxs-lookup"><span data-stu-id="62028-144">Time when call ended.</span></span>|
|<span data-ttu-id="62028-145">duration</span><span class="sxs-lookup"><span data-stu-id="62028-145">duration</span></span>|<span data-ttu-id="62028-146">Int32</span><span class="sxs-lookup"><span data-stu-id="62028-146">Int32</span></span>| <span data-ttu-id="62028-147">呼叫的持续时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="62028-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="62028-148">callType</span><span class="sxs-lookup"><span data-stu-id="62028-148">callType</span></span>|<span data-ttu-id="62028-149">String</span><span class="sxs-lookup"><span data-stu-id="62028-149">String</span></span>| <span data-ttu-id="62028-150">呼叫类型和方向。</span><span class="sxs-lookup"><span data-stu-id="62028-150">Call type and direction.</span></span>|
|<span data-ttu-id="62028-151">successfulCall</span><span class="sxs-lookup"><span data-stu-id="62028-151">successfulCall</span></span>|<span data-ttu-id="62028-152">布尔</span><span class="sxs-lookup"><span data-stu-id="62028-152">Boolean</span></span>| <span data-ttu-id="62028-153">成功或尝试。</span><span class="sxs-lookup"><span data-stu-id="62028-153">Success or attempt.</span></span>|
|<span data-ttu-id="62028-154">callerNumber</span><span class="sxs-lookup"><span data-stu-id="62028-154">callerNumber</span></span>|<span data-ttu-id="62028-155">String</span><span class="sxs-lookup"><span data-stu-id="62028-155">String</span></span>| <span data-ttu-id="62028-156">进行呼叫的用户或机器人的号码。</span><span class="sxs-lookup"><span data-stu-id="62028-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="62028-157">[E.164](https://en.wikipedia.org/wiki/E.164) 格式，但可能包括其他数据。</span><span class="sxs-lookup"><span data-stu-id="62028-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="62028-158">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="62028-158">calleeNumber</span></span>|<span data-ttu-id="62028-159">String</span><span class="sxs-lookup"><span data-stu-id="62028-159">String</span></span>| <span data-ttu-id="62028-160">收到呼叫的用户或自动程序的数量。</span><span class="sxs-lookup"><span data-stu-id="62028-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="62028-161">[E.164](https://en.wikipedia.org/wiki/E.164) 格式，但可能包括其他数据。</span><span class="sxs-lookup"><span data-stu-id="62028-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="62028-162">mediaPathLocation</span><span class="sxs-lookup"><span data-stu-id="62028-162">mediaPathLocation</span></span>|<span data-ttu-id="62028-163">String</span><span class="sxs-lookup"><span data-stu-id="62028-163">String</span></span>| <span data-ttu-id="62028-164">用于非旁路呼叫中的媒体路径的数据中心。</span><span class="sxs-lookup"><span data-stu-id="62028-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="62028-165">signalingLocation</span><span class="sxs-lookup"><span data-stu-id="62028-165">signalingLocation</span></span>|<span data-ttu-id="62028-166">String</span><span class="sxs-lookup"><span data-stu-id="62028-166">String</span></span>| <span data-ttu-id="62028-167">用于对旁路和非旁路呼叫发出信号的数据中心。</span><span class="sxs-lookup"><span data-stu-id="62028-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="62028-168">finalSipCode</span><span class="sxs-lookup"><span data-stu-id="62028-168">finalSipCode</span></span>|<span data-ttu-id="62028-169">Int32</span><span class="sxs-lookup"><span data-stu-id="62028-169">Int32</span></span>| <span data-ttu-id="62028-170">结束呼叫的代码[RFC 3261。](https://tools.ietf.org/html/rfc3261)</span><span class="sxs-lookup"><span data-stu-id="62028-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="62028-171">callEndSubReason</span><span class="sxs-lookup"><span data-stu-id="62028-171">callEndSubReason</span></span>|<span data-ttu-id="62028-172">Int32</span><span class="sxs-lookup"><span data-stu-id="62028-172">Int32</span></span>| <span data-ttu-id="62028-173">除了 SIP 代码之外，Microsoft 还有自己的指示特定问题的子代码。</span><span class="sxs-lookup"><span data-stu-id="62028-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="62028-174">finalSipCodePhrase</span><span class="sxs-lookup"><span data-stu-id="62028-174">finalSipCodePhrase</span></span>|<span data-ttu-id="62028-175">String</span><span class="sxs-lookup"><span data-stu-id="62028-175">String</span></span>| <span data-ttu-id="62028-176">SIP 代码和 Microsoft 子代码的说明。</span><span class="sxs-lookup"><span data-stu-id="62028-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="62028-177">trunkFullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="62028-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="62028-178">String</span><span class="sxs-lookup"><span data-stu-id="62028-178">String</span></span>| <span data-ttu-id="62028-179">会话边界控制器的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="62028-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="62028-180">mediaBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="62028-180">mediaBypassEnabled</span></span>|<span data-ttu-id="62028-181">布尔</span><span class="sxs-lookup"><span data-stu-id="62028-181">Boolean</span></span>| <span data-ttu-id="62028-182">指示中继是否已启用媒体旁路。</span><span class="sxs-lookup"><span data-stu-id="62028-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62028-183">关系</span><span class="sxs-lookup"><span data-stu-id="62028-183">Relationships</span></span>

<span data-ttu-id="62028-184">无。</span><span class="sxs-lookup"><span data-stu-id="62028-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62028-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62028-185">JSON representation</span></span>

<span data-ttu-id="62028-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62028-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
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


