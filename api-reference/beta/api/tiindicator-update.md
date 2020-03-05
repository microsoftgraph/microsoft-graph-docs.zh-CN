---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0db1441030dc75d60dcbb1bd3d3eab2b09a5aad4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452340"
---
# <a name="update-tiindicator"></a><span data-ttu-id="e235f-103">更新 tiIndicator</span><span class="sxs-lookup"><span data-stu-id="e235f-103">Update tiIndicator</span></span>

<span data-ttu-id="e235f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e235f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e235f-105">更新[tiIndicator](../resources/tiindicator.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e235f-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e235f-106">权限</span><span class="sxs-lookup"><span data-stu-id="e235f-106">Permissions</span></span>

<span data-ttu-id="e235f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e235f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e235f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e235f-109">Permission type</span></span>                        | <span data-ttu-id="e235f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e235f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e235f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e235f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e235f-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e235f-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e235f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e235f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e235f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e235f-114">Not supported.</span></span> |
| <span data-ttu-id="e235f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e235f-115">Application</span></span>                            | <span data-ttu-id="e235f-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e235f-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e235f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e235f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e235f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e235f-118">Request headers</span></span>

| <span data-ttu-id="e235f-119">名称</span><span class="sxs-lookup"><span data-stu-id="e235f-119">Name</span></span>       | <span data-ttu-id="e235f-120">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e235f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e235f-121">Authorization</span></span> | <span data-ttu-id="e235f-122">**必需**的持有者 {代码}</span><span class="sxs-lookup"><span data-stu-id="e235f-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="e235f-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="e235f-123">Prefer</span></span> | <span data-ttu-id="e235f-124">return = 表示形式</span><span class="sxs-lookup"><span data-stu-id="e235f-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="e235f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e235f-125">Request body</span></span>

<span data-ttu-id="e235f-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e235f-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e235f-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e235f-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e235f-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e235f-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="e235f-129">必填字段为`id`： `expirationDateTime`、 `targetProduct`、。</span><span class="sxs-lookup"><span data-stu-id="e235f-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="e235f-130">属性</span><span class="sxs-lookup"><span data-stu-id="e235f-130">Property</span></span>     | <span data-ttu-id="e235f-131">类型</span><span class="sxs-lookup"><span data-stu-id="e235f-131">Type</span></span>        | <span data-ttu-id="e235f-132">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e235f-133">action</span><span class="sxs-lookup"><span data-stu-id="e235f-133">action</span></span>|<span data-ttu-id="e235f-134">string</span><span class="sxs-lookup"><span data-stu-id="e235f-134">string</span></span>| <span data-ttu-id="e235f-135">在 targetProduct 安全工具中匹配指标时要应用的操作。</span><span class="sxs-lookup"><span data-stu-id="e235f-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="e235f-136">可取值为：`unknown`、`allow`、`block`、`alert`。</span><span class="sxs-lookup"><span data-stu-id="e235f-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="e235f-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="e235f-137">activityGroupNames</span></span>|<span data-ttu-id="e235f-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="e235f-138">String collection</span></span>|<span data-ttu-id="e235f-139">负责威胁指示器所涵盖的恶意活动的各方的网络威胁智能名称。</span><span class="sxs-lookup"><span data-stu-id="e235f-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="e235f-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e235f-140">additionalInformation</span></span>|<span data-ttu-id="e235f-141">String</span><span class="sxs-lookup"><span data-stu-id="e235f-141">String</span></span>|<span data-ttu-id="e235f-142">可以放置其他 tiIndicator 属性中未涵盖的指标中的额外数据的 "容器" 区域。</span><span class="sxs-lookup"><span data-stu-id="e235f-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="e235f-143">放置在 additionalInformation 中的数据通常不会被 targetProduct 安全工具使用。</span><span class="sxs-lookup"><span data-stu-id="e235f-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="e235f-144">confidence</span><span class="sxs-lookup"><span data-stu-id="e235f-144">confidence</span></span>|<span data-ttu-id="e235f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e235f-145">Int32</span></span>|<span data-ttu-id="e235f-146">一个整数，表示对指示器中的数据准确标识恶意行为的可信度。</span><span class="sxs-lookup"><span data-stu-id="e235f-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="e235f-147">可接受的值为0–100，100的值为最高。</span><span class="sxs-lookup"><span data-stu-id="e235f-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="e235f-148">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-148">description</span></span>|<span data-ttu-id="e235f-149">String</span><span class="sxs-lookup"><span data-stu-id="e235f-149">String</span></span>|<span data-ttu-id="e235f-150">由指示器表示的威胁的简短说明（100个字符或更少）。</span><span class="sxs-lookup"><span data-stu-id="e235f-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="e235f-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="e235f-151">diamondModel</span></span>|[<span data-ttu-id="e235f-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="e235f-152">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="e235f-153">此指示器所在的菱形模型的面积。</span><span class="sxs-lookup"><span data-stu-id="e235f-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="e235f-154">可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。</span><span class="sxs-lookup"><span data-stu-id="e235f-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="e235f-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e235f-155">expirationDateTime</span></span>|<span data-ttu-id="e235f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e235f-156">DateTimeOffset</span></span>| <span data-ttu-id="e235f-157">指示指示器过期时间的日期/时间字符串。</span><span class="sxs-lookup"><span data-stu-id="e235f-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="e235f-158">所有指标都必须具有到期日期，以避免系统中的陈旧指示器持久化。</span><span class="sxs-lookup"><span data-stu-id="e235f-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="e235f-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e235f-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e235f-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e235f-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e235f-161">externalId</span><span class="sxs-lookup"><span data-stu-id="e235f-161">externalId</span></span>|<span data-ttu-id="e235f-162">String</span><span class="sxs-lookup"><span data-stu-id="e235f-162">String</span></span>|<span data-ttu-id="e235f-163">将指示器与指示器提供程序的系统（例如外键）相结合的标识号。</span><span class="sxs-lookup"><span data-stu-id="e235f-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="e235f-164">isActive</span><span class="sxs-lookup"><span data-stu-id="e235f-164">isActive</span></span>|<span data-ttu-id="e235f-165">布尔</span><span class="sxs-lookup"><span data-stu-id="e235f-165">Boolean</span></span>|<span data-ttu-id="e235f-166">用于停用系统中的指示器。</span><span class="sxs-lookup"><span data-stu-id="e235f-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="e235f-167">默认情况下，提交的任何指示器都设置为活动状态。</span><span class="sxs-lookup"><span data-stu-id="e235f-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="e235f-168">但是，提供程序可能会将此设置为 "False" 的现有指示器提交到系统中停用指示器。</span><span class="sxs-lookup"><span data-stu-id="e235f-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="e235f-169">killChain</span><span class="sxs-lookup"><span data-stu-id="e235f-169">killChain</span></span>|<span data-ttu-id="e235f-170">[killChain](#killchain-values)集合</span><span class="sxs-lookup"><span data-stu-id="e235f-170">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="e235f-171">一个 JSON 字符串数组，用于描述此指示器针对终止链上的哪个点或点。</span><span class="sxs-lookup"><span data-stu-id="e235f-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="e235f-172">有关确切值，请参阅下面的 "killChain 值"。</span><span class="sxs-lookup"><span data-stu-id="e235f-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="e235f-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="e235f-173">knownFalsePositives</span></span>|<span data-ttu-id="e235f-174">String</span><span class="sxs-lookup"><span data-stu-id="e235f-174">String</span></span>|<span data-ttu-id="e235f-175">指示符可能导致误报的情况。</span><span class="sxs-lookup"><span data-stu-id="e235f-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="e235f-176">这应该是可读的文本。</span><span class="sxs-lookup"><span data-stu-id="e235f-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="e235f-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e235f-177">lastReportedDateTime</span></span>|<span data-ttu-id="e235f-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e235f-178">DateTimeOffset</span></span>|<span data-ttu-id="e235f-179">上次发现指示器的时间。</span><span class="sxs-lookup"><span data-stu-id="e235f-179">The last time the indicator was seen.</span></span> <span data-ttu-id="e235f-180">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e235f-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e235f-181">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e235f-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e235f-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="e235f-182">malwareFamilyNames</span></span>|<span data-ttu-id="e235f-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="e235f-183">String collection</span></span>|<span data-ttu-id="e235f-184">与指示器关联的恶意软件系列名称（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="e235f-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="e235f-185">如果所有可能都可以通过 Windows Defender 安全智能[威胁百科全书](https://www.microsoft.com/wdsi/threats)找到，microsoft 将首选 microsoft 恶意软件系列名称。</span><span class="sxs-lookup"><span data-stu-id="e235f-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="e235f-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="e235f-186">passiveOnly</span></span>|<span data-ttu-id="e235f-187">布尔</span><span class="sxs-lookup"><span data-stu-id="e235f-187">Boolean</span></span>|<span data-ttu-id="e235f-188">确定该指示符是否应触发对最终用户可见的事件。</span><span class="sxs-lookup"><span data-stu-id="e235f-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="e235f-189">如果设置为 "true"，则安全工具将不会通知最终用户已发生 "命中"。</span><span class="sxs-lookup"><span data-stu-id="e235f-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="e235f-190">通常情况下，这通常被视为审核或静默模式，安全产品只需记录已发生的匹配项，但不会执行该操作。</span><span class="sxs-lookup"><span data-stu-id="e235f-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="e235f-191">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="e235f-191">Default value is false.</span></span>|
|<span data-ttu-id="e235f-192">severity</span><span class="sxs-lookup"><span data-stu-id="e235f-192">severity</span></span>|<span data-ttu-id="e235f-193">Int32</span><span class="sxs-lookup"><span data-stu-id="e235f-193">Int32</span></span>|<span data-ttu-id="e235f-194">一个整数，表示由指示器中的数据标识的恶意行为的严重程度。</span><span class="sxs-lookup"><span data-stu-id="e235f-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="e235f-195">可接受的值为0–5，其中5为最严重，0表示根本不严重。</span><span class="sxs-lookup"><span data-stu-id="e235f-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="e235f-196">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="e235f-196">Default value is 3.</span></span>|
|<span data-ttu-id="e235f-197">标记</span><span class="sxs-lookup"><span data-stu-id="e235f-197">tags</span></span>|<span data-ttu-id="e235f-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="e235f-198">String collection</span></span>|<span data-ttu-id="e235f-199">存储任意标记/关键字的字符串的 JSON 数组。</span><span class="sxs-lookup"><span data-stu-id="e235f-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="e235f-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="e235f-200">tlpLevel</span></span>|[<span data-ttu-id="e235f-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="e235f-201">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="e235f-202">指标的流量灯协议值。</span><span class="sxs-lookup"><span data-stu-id="e235f-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="e235f-203">可取值为：`unknown`、`white`、`green`、`amber`、`red`。</span><span class="sxs-lookup"><span data-stu-id="e235f-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="e235f-204">diamondModel 值</span><span class="sxs-lookup"><span data-stu-id="e235f-204">diamondModel values</span></span>

<span data-ttu-id="e235f-205">有关此模型的信息，请参阅[菱形模型](http://diamondmodel.org)。</span><span class="sxs-lookup"><span data-stu-id="e235f-205">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="e235f-206">值</span><span class="sxs-lookup"><span data-stu-id="e235f-206">Values</span></span> | <span data-ttu-id="e235f-207">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-207">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e235f-208">对手</span><span class="sxs-lookup"><span data-stu-id="e235f-208">adversary</span></span>|<span data-ttu-id="e235f-209">该指示器描述了敌人。</span><span class="sxs-lookup"><span data-stu-id="e235f-209">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="e235f-210">性能</span><span class="sxs-lookup"><span data-stu-id="e235f-210">capability</span></span>|<span data-ttu-id="e235f-211">该指标是入侵者的一种功能。</span><span class="sxs-lookup"><span data-stu-id="e235f-211">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="e235f-212">基本</span><span class="sxs-lookup"><span data-stu-id="e235f-212">infrastructure</span></span>|<span data-ttu-id="e235f-213">此指标介绍了入侵者的基础结构。</span><span class="sxs-lookup"><span data-stu-id="e235f-213">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="e235f-214">者</span><span class="sxs-lookup"><span data-stu-id="e235f-214">victim</span></span>|<span data-ttu-id="e235f-215">该指标描述敌人的牺牲品。</span><span class="sxs-lookup"><span data-stu-id="e235f-215">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="e235f-216">killChain 值</span><span class="sxs-lookup"><span data-stu-id="e235f-216">killChain values</span></span>

| <span data-ttu-id="e235f-217">值</span><span class="sxs-lookup"><span data-stu-id="e235f-217">Values</span></span> | <span data-ttu-id="e235f-218">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-218">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e235f-219">操作</span><span class="sxs-lookup"><span data-stu-id="e235f-219">Actions</span></span>|<span data-ttu-id="e235f-220">代表 "针对目标的操作"。</span><span class="sxs-lookup"><span data-stu-id="e235f-220">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="e235f-221">攻击者利用受攻击的系统执行诸如分布式拒绝服务攻击之类的操作。</span><span class="sxs-lookup"><span data-stu-id="e235f-221">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="e235f-222">C2</span><span class="sxs-lookup"><span data-stu-id="e235f-222">C2</span></span>|<span data-ttu-id="e235f-223">表示操纵受损系统时所使用的控制通道。</span><span class="sxs-lookup"><span data-stu-id="e235f-223">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="e235f-224">Delivery</span><span class="sxs-lookup"><span data-stu-id="e235f-224">Delivery</span></span>|<span data-ttu-id="e235f-225">将攻击代码分发给受害者的过程（例如，USB、电子邮件、网站）。</span><span class="sxs-lookup"><span data-stu-id="e235f-225">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="e235f-226">具备</span><span class="sxs-lookup"><span data-stu-id="e235f-226">Exploitation</span></span>|<span data-ttu-id="e235f-227">利用漏洞的攻击代码（例如，代码执行）。</span><span class="sxs-lookup"><span data-stu-id="e235f-227">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="e235f-228">安装</span><span class="sxs-lookup"><span data-stu-id="e235f-228">Installation</span></span>|<span data-ttu-id="e235f-229">在漏洞受到攻击后安装恶意软件。</span><span class="sxs-lookup"><span data-stu-id="e235f-229">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="e235f-230">侦测</span><span class="sxs-lookup"><span data-stu-id="e235f-230">Reconnaissance</span></span>|<span data-ttu-id="e235f-231">指标是活动组收集信息以用于将来的攻击的证据。</span><span class="sxs-lookup"><span data-stu-id="e235f-231">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="e235f-232">Weaponization</span><span class="sxs-lookup"><span data-stu-id="e235f-232">Weaponization</span></span>|<span data-ttu-id="e235f-233">将漏洞转换为攻击代码（例如恶意软件）。</span><span class="sxs-lookup"><span data-stu-id="e235f-233">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="e235f-234">tlpLevel 值</span><span class="sxs-lookup"><span data-stu-id="e235f-234">tlpLevel values</span></span>

<span data-ttu-id="e235f-235">提交每个指示器时，都必须具有流量灯协议（tlp）值。</span><span class="sxs-lookup"><span data-stu-id="e235f-235">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="e235f-236">此值表示给定指标的敏感度和共享作用域。</span><span class="sxs-lookup"><span data-stu-id="e235f-236">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="e235f-237">值</span><span class="sxs-lookup"><span data-stu-id="e235f-237">Values</span></span> | <span data-ttu-id="e235f-238">说明</span><span class="sxs-lookup"><span data-stu-id="e235f-238">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e235f-239">白色</span><span class="sxs-lookup"><span data-stu-id="e235f-239">White</span></span>| <span data-ttu-id="e235f-240">共享范围：无限制。</span><span class="sxs-lookup"><span data-stu-id="e235f-240">Sharing scope: Unlimited.</span></span> <span data-ttu-id="e235f-241">指示器可以自由共享，无需限制。</span><span class="sxs-lookup"><span data-stu-id="e235f-241">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="e235f-242">绿色</span><span class="sxs-lookup"><span data-stu-id="e235f-242">Green</span></span>| <span data-ttu-id="e235f-243">共享作用域：社区。</span><span class="sxs-lookup"><span data-stu-id="e235f-243">Sharing scope: Community.</span></span> <span data-ttu-id="e235f-244">指标可与安全社区共享。</span><span class="sxs-lookup"><span data-stu-id="e235f-244">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="e235f-245">亮</span><span class="sxs-lookup"><span data-stu-id="e235f-245">Amber</span></span>| <span data-ttu-id="e235f-246">共享作用域：受限。</span><span class="sxs-lookup"><span data-stu-id="e235f-246">Sharing scope: Limited.</span></span> <span data-ttu-id="e235f-247">这是指示器的默认设置，并限制仅与实施了威胁智能的服务和服务运算符共享：2）其系统表现为与指示器一致的行为的客户。</span><span class="sxs-lookup"><span data-stu-id="e235f-247">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="e235f-248">红色</span><span class="sxs-lookup"><span data-stu-id="e235f-248">Red</span></span>| <span data-ttu-id="e235f-249">共享作用域：个人。</span><span class="sxs-lookup"><span data-stu-id="e235f-249">Sharing scope: Personal.</span></span> <span data-ttu-id="e235f-250">这些指标仅可直接共享，最好是人员。</span><span class="sxs-lookup"><span data-stu-id="e235f-250">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="e235f-251">通常情况下，TLP 红色指示器不会引入，因为其预定义限制。</span><span class="sxs-lookup"><span data-stu-id="e235f-251">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="e235f-252">如果提交了 TLP 红色指示器，则**passiveOnly**属性也应设置为`True` 。</span><span class="sxs-lookup"><span data-stu-id="e235f-252">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="e235f-253">响应</span><span class="sxs-lookup"><span data-stu-id="e235f-253">Response</span></span>

<span data-ttu-id="e235f-254">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e235f-254">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="e235f-255">如果使用可选请求标头，则该方法将在`200 OK`响应正文中返回响应代码和更新的[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e235f-255">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e235f-256">示例</span><span class="sxs-lookup"><span data-stu-id="e235f-256">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="e235f-257">示例1：不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="e235f-257">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e235f-258">请求</span><span class="sxs-lookup"><span data-stu-id="e235f-258">Request</span></span>

<span data-ttu-id="e235f-259">以下是不带`Prefer`标头的请求示例。</span><span class="sxs-lookup"><span data-stu-id="e235f-259">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="e235f-260">HTTP</span><span class="sxs-lookup"><span data-stu-id="e235f-260">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="e235f-261">C#</span><span class="sxs-lookup"><span data-stu-id="e235f-261">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e235f-262">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e235f-262">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e235f-263">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e235f-263">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e235f-264">响应</span><span class="sxs-lookup"><span data-stu-id="e235f-264">Response</span></span>

<span data-ttu-id="e235f-265">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e235f-265">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="e235f-266">示例2：具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="e235f-266">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e235f-267">请求</span><span class="sxs-lookup"><span data-stu-id="e235f-267">Request</span></span>

<span data-ttu-id="e235f-268">以下是包含`Prefer`标头的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="e235f-268">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a><span data-ttu-id="e235f-269">响应</span><span class="sxs-lookup"><span data-stu-id="e235f-269">Response</span></span>

<span data-ttu-id="e235f-270">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e235f-270">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e235f-271">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e235f-271">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e235f-272">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e235f-272">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
