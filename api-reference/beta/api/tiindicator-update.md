---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: aec339fd51b6c3e5111dadf29f8a8caf5ba3b724
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990755"
---
# <a name="update-tiindicator"></a><span data-ttu-id="e5b64-103">更新 tiIndicator</span><span class="sxs-lookup"><span data-stu-id="e5b64-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b64-104">更新[tiIndicator](../resources/tiindicator.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5b64-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5b64-105">权限</span><span class="sxs-lookup"><span data-stu-id="e5b64-105">Permissions</span></span>

<span data-ttu-id="e5b64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5b64-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5b64-108">Permission type</span></span>                        | <span data-ttu-id="e5b64-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5b64-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5b64-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b64-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5b64-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e5b64-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="e5b64-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5b64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b64-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5b64-113">Not supported.</span></span> |
| <span data-ttu-id="e5b64-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5b64-114">Application</span></span>                            | <span data-ttu-id="e5b64-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="e5b64-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5b64-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5b64-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e5b64-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5b64-117">Request headers</span></span>

| <span data-ttu-id="e5b64-118">名称</span><span class="sxs-lookup"><span data-stu-id="e5b64-118">Name</span></span>       | <span data-ttu-id="e5b64-119">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e5b64-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b64-120">Authorization</span></span> | <span data-ttu-id="e5b64-121">**必需**的持有者 {代码}</span><span class="sxs-lookup"><span data-stu-id="e5b64-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="e5b64-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="e5b64-122">Prefer</span></span> | <span data-ttu-id="e5b64-123">return = 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5b64-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b64-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5b64-124">Request body</span></span>

<span data-ttu-id="e5b64-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="e5b64-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e5b64-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e5b64-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e5b64-127">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e5b64-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5b64-128">属性</span><span class="sxs-lookup"><span data-stu-id="e5b64-128">Property</span></span>     | <span data-ttu-id="e5b64-129">类型</span><span class="sxs-lookup"><span data-stu-id="e5b64-129">Type</span></span>        | <span data-ttu-id="e5b64-130">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e5b64-131">action</span><span class="sxs-lookup"><span data-stu-id="e5b64-131">action</span></span>|<span data-ttu-id="e5b64-132">string</span><span class="sxs-lookup"><span data-stu-id="e5b64-132">string</span></span>| <span data-ttu-id="e5b64-133">在 targetProduct 安全工具中匹配指标时要应用的操作。</span><span class="sxs-lookup"><span data-stu-id="e5b64-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="e5b64-134">可取值为：`unknown`、`allow`、`block`、`alert`。</span><span class="sxs-lookup"><span data-stu-id="e5b64-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="e5b64-135">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="e5b64-135">activityGroupNames</span></span>|<span data-ttu-id="e5b64-136">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b64-136">String collection</span></span>|<span data-ttu-id="e5b64-137">负责威胁指示器所涵盖的恶意活动的各方的网络威胁智能名称。</span><span class="sxs-lookup"><span data-stu-id="e5b64-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="e5b64-138">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e5b64-138">additionalInformation</span></span>|<span data-ttu-id="e5b64-139">String</span><span class="sxs-lookup"><span data-stu-id="e5b64-139">String</span></span>|<span data-ttu-id="e5b64-140">可以放置其他 tiIndicator 属性中未涵盖的指标中的额外数据的 "容器" 区域。</span><span class="sxs-lookup"><span data-stu-id="e5b64-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="e5b64-141">放置在 additionalInformation 中的数据通常不会被 targetProduct 安全工具使用。</span><span class="sxs-lookup"><span data-stu-id="e5b64-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="e5b64-142">confidence</span><span class="sxs-lookup"><span data-stu-id="e5b64-142">confidence</span></span>|<span data-ttu-id="e5b64-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b64-143">Int32</span></span>|<span data-ttu-id="e5b64-144">一个整数, 表示对指示器中的数据准确标识恶意行为的可信度。</span><span class="sxs-lookup"><span data-stu-id="e5b64-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="e5b64-145">可接受的值为0– 100, 100 的值为最高。</span><span class="sxs-lookup"><span data-stu-id="e5b64-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="e5b64-146">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-146">description</span></span>|<span data-ttu-id="e5b64-147">String</span><span class="sxs-lookup"><span data-stu-id="e5b64-147">String</span></span>|<span data-ttu-id="e5b64-148">由指示器表示的威胁的简短说明 (100 个字符或更少)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="e5b64-149">diamondModel</span><span class="sxs-lookup"><span data-stu-id="e5b64-149">diamondModel</span></span>|[<span data-ttu-id="e5b64-150">diamondModel</span><span class="sxs-lookup"><span data-stu-id="e5b64-150">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="e5b64-151">此指示器所在的菱形模型的面积。</span><span class="sxs-lookup"><span data-stu-id="e5b64-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="e5b64-152">可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。</span><span class="sxs-lookup"><span data-stu-id="e5b64-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="e5b64-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b64-153">expirationDateTime</span></span>|<span data-ttu-id="e5b64-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b64-154">DateTimeOffset</span></span>| <span data-ttu-id="e5b64-155">指示指示器过期时间的日期/时间字符串。</span><span class="sxs-lookup"><span data-stu-id="e5b64-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="e5b64-156">所有指标都必须具有到期日期, 以避免系统中的陈旧指示器持久化。</span><span class="sxs-lookup"><span data-stu-id="e5b64-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="e5b64-157">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e5b64-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e5b64-158">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e5b64-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e5b64-159">externalId</span><span class="sxs-lookup"><span data-stu-id="e5b64-159">externalId</span></span>|<span data-ttu-id="e5b64-160">String</span><span class="sxs-lookup"><span data-stu-id="e5b64-160">String</span></span>|<span data-ttu-id="e5b64-161">将指示器与指示器提供程序的系统 (例如外键) 相结合的标识号。</span><span class="sxs-lookup"><span data-stu-id="e5b64-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="e5b64-162">isActive</span><span class="sxs-lookup"><span data-stu-id="e5b64-162">isActive</span></span>|<span data-ttu-id="e5b64-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b64-163">Boolean</span></span>|<span data-ttu-id="e5b64-164">用于停用系统中的指示器。</span><span class="sxs-lookup"><span data-stu-id="e5b64-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="e5b64-165">默认情况下, 提交的任何指示器都设置为活动状态。</span><span class="sxs-lookup"><span data-stu-id="e5b64-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="e5b64-166">但是, 提供程序可能会将此设置为 "False" 的现有指示器提交到系统中停用指示器。</span><span class="sxs-lookup"><span data-stu-id="e5b64-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="e5b64-167">killChain</span><span class="sxs-lookup"><span data-stu-id="e5b64-167">killChain</span></span>|<span data-ttu-id="e5b64-168">[killChain](#killchain-values)集合</span><span class="sxs-lookup"><span data-stu-id="e5b64-168">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="e5b64-169">一个 JSON 字符串数组, 用于描述此指示器针对终止链上的哪个点或点。</span><span class="sxs-lookup"><span data-stu-id="e5b64-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="e5b64-170">有关确切值, 请参阅下面的 "killChain 值"。</span><span class="sxs-lookup"><span data-stu-id="e5b64-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="e5b64-171">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="e5b64-171">knownFalsePositives</span></span>|<span data-ttu-id="e5b64-172">String</span><span class="sxs-lookup"><span data-stu-id="e5b64-172">String</span></span>|<span data-ttu-id="e5b64-173">指示符可能导致误报的情况。</span><span class="sxs-lookup"><span data-stu-id="e5b64-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="e5b64-174">这应该是可读的文本。</span><span class="sxs-lookup"><span data-stu-id="e5b64-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="e5b64-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b64-175">lastReportedDateTime</span></span>|<span data-ttu-id="e5b64-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b64-176">DateTimeOffset</span></span>|<span data-ttu-id="e5b64-177">上次发现指示器的时间。</span><span class="sxs-lookup"><span data-stu-id="e5b64-177">The last time the indicator was seen.</span></span> <span data-ttu-id="e5b64-178">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e5b64-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e5b64-179">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e5b64-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e5b64-180">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="e5b64-180">malwareFamilyNames</span></span>|<span data-ttu-id="e5b64-181">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b64-181">String collection</span></span>|<span data-ttu-id="e5b64-182">与指示器关联的恶意软件系列名称 (如果存在)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="e5b64-183">如果所有可能都可以通过 Windows Defender 安全智能[威胁百科全书](https://www.microsoft.com/wdsi/threats)找到, microsoft 将首选 microsoft 恶意软件系列名称。</span><span class="sxs-lookup"><span data-stu-id="e5b64-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="e5b64-184">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="e5b64-184">passiveOnly</span></span>|<span data-ttu-id="e5b64-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b64-185">Boolean</span></span>|<span data-ttu-id="e5b64-186">确定该指示符是否应触发对最终用户可见的事件。</span><span class="sxs-lookup"><span data-stu-id="e5b64-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="e5b64-187">如果设置为 "true", 则安全工具将不会通知最终用户已发生 "命中"。</span><span class="sxs-lookup"><span data-stu-id="e5b64-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="e5b64-188">通常情况下, 这通常被视为审核或静默模式, 安全产品只需记录已发生的匹配项, 但不会执行该操作。</span><span class="sxs-lookup"><span data-stu-id="e5b64-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="e5b64-189">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="e5b64-189">Default value is false.</span></span>|
|<span data-ttu-id="e5b64-190">severity</span><span class="sxs-lookup"><span data-stu-id="e5b64-190">severity</span></span>|<span data-ttu-id="e5b64-191">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b64-191">Int32</span></span>|<span data-ttu-id="e5b64-192">一个整数, 表示由指示器中的数据标识的恶意行为的严重程度。</span><span class="sxs-lookup"><span data-stu-id="e5b64-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="e5b64-193">可接受的值为0– 5, 其中5为最严重, 0 表示根本不严重。</span><span class="sxs-lookup"><span data-stu-id="e5b64-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="e5b64-194">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="e5b64-194">Default value is 3.</span></span>|
|<span data-ttu-id="e5b64-195">tags</span><span class="sxs-lookup"><span data-stu-id="e5b64-195">tags</span></span>|<span data-ttu-id="e5b64-196">String collection</span><span class="sxs-lookup"><span data-stu-id="e5b64-196">String collection</span></span>|<span data-ttu-id="e5b64-197">存储任意标记/关键字的字符串的 JSON 数组。</span><span class="sxs-lookup"><span data-stu-id="e5b64-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="e5b64-198">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="e5b64-198">tlpLevel</span></span>|[<span data-ttu-id="e5b64-199">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="e5b64-199">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="e5b64-200">指标的流量灯协议值。</span><span class="sxs-lookup"><span data-stu-id="e5b64-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="e5b64-201">可取值为：`unknown`、`white`、`green`、`amber`、`red`。</span><span class="sxs-lookup"><span data-stu-id="e5b64-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="e5b64-202">diamondModel 值</span><span class="sxs-lookup"><span data-stu-id="e5b64-202">diamondModel values</span></span>

<span data-ttu-id="e5b64-203">有关此模型的信息, 请参阅[菱形模型](http://diamondmodel.org)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="e5b64-204">值</span><span class="sxs-lookup"><span data-stu-id="e5b64-204">Values</span></span> | <span data-ttu-id="e5b64-205">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e5b64-206">对手</span><span class="sxs-lookup"><span data-stu-id="e5b64-206">adversary</span></span>|<span data-ttu-id="e5b64-207">该指示器描述了敌人。</span><span class="sxs-lookup"><span data-stu-id="e5b64-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="e5b64-208">性能</span><span class="sxs-lookup"><span data-stu-id="e5b64-208">capability</span></span>|<span data-ttu-id="e5b64-209">该指标是入侵者的一种功能。</span><span class="sxs-lookup"><span data-stu-id="e5b64-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="e5b64-210">基本</span><span class="sxs-lookup"><span data-stu-id="e5b64-210">infrastructure</span></span>|<span data-ttu-id="e5b64-211">此指标介绍了入侵者的基础结构。</span><span class="sxs-lookup"><span data-stu-id="e5b64-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="e5b64-212">者</span><span class="sxs-lookup"><span data-stu-id="e5b64-212">victim</span></span>|<span data-ttu-id="e5b64-213">该指标描述敌人的牺牲品。</span><span class="sxs-lookup"><span data-stu-id="e5b64-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="e5b64-214">killChain 值</span><span class="sxs-lookup"><span data-stu-id="e5b64-214">killChain values</span></span>

| <span data-ttu-id="e5b64-215">值</span><span class="sxs-lookup"><span data-stu-id="e5b64-215">Values</span></span> | <span data-ttu-id="e5b64-216">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e5b64-217">操作</span><span class="sxs-lookup"><span data-stu-id="e5b64-217">Actions</span></span>|<span data-ttu-id="e5b64-218">代表 "针对目标的操作"。</span><span class="sxs-lookup"><span data-stu-id="e5b64-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="e5b64-219">攻击者利用受攻击的系统执行诸如分布式拒绝服务攻击之类的操作。</span><span class="sxs-lookup"><span data-stu-id="e5b64-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="e5b64-220">C2</span><span class="sxs-lookup"><span data-stu-id="e5b64-220">C2</span></span>|<span data-ttu-id="e5b64-221">表示操纵受损系统时所使用的控制通道。</span><span class="sxs-lookup"><span data-stu-id="e5b64-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="e5b64-222">Delivery</span><span class="sxs-lookup"><span data-stu-id="e5b64-222">Delivery</span></span>|<span data-ttu-id="e5b64-223">将攻击代码分发给受害者的过程 (例如, USB、电子邮件、网站)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="e5b64-224">具备</span><span class="sxs-lookup"><span data-stu-id="e5b64-224">Exploitation</span></span>|<span data-ttu-id="e5b64-225">利用漏洞的攻击代码 (例如, 代码执行)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="e5b64-226">安装</span><span class="sxs-lookup"><span data-stu-id="e5b64-226">Installation</span></span>|<span data-ttu-id="e5b64-227">在漏洞受到攻击后安装恶意软件。</span><span class="sxs-lookup"><span data-stu-id="e5b64-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="e5b64-228">侦测</span><span class="sxs-lookup"><span data-stu-id="e5b64-228">Reconnaissance</span></span>|<span data-ttu-id="e5b64-229">指标是活动组收集信息以用于将来的攻击的证据。</span><span class="sxs-lookup"><span data-stu-id="e5b64-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="e5b64-230">Weaponization</span><span class="sxs-lookup"><span data-stu-id="e5b64-230">Weaponization</span></span>|<span data-ttu-id="e5b64-231">将漏洞转换为攻击代码 (例如恶意软件)。</span><span class="sxs-lookup"><span data-stu-id="e5b64-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="e5b64-232">tlpLevel 值</span><span class="sxs-lookup"><span data-stu-id="e5b64-232">tlpLevel values</span></span>

<span data-ttu-id="e5b64-233">提交每个指示器时, 都必须具有流量灯协议 (tlp) 值。</span><span class="sxs-lookup"><span data-stu-id="e5b64-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="e5b64-234">此值表示给定指标的敏感度和共享作用域。</span><span class="sxs-lookup"><span data-stu-id="e5b64-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="e5b64-235">值</span><span class="sxs-lookup"><span data-stu-id="e5b64-235">Values</span></span> | <span data-ttu-id="e5b64-236">说明</span><span class="sxs-lookup"><span data-stu-id="e5b64-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="e5b64-237">白色</span><span class="sxs-lookup"><span data-stu-id="e5b64-237">White</span></span>| <span data-ttu-id="e5b64-238">共享范围: 无限制。</span><span class="sxs-lookup"><span data-stu-id="e5b64-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="e5b64-239">指示器可以自由共享, 无需限制。</span><span class="sxs-lookup"><span data-stu-id="e5b64-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="e5b64-240">绿色</span><span class="sxs-lookup"><span data-stu-id="e5b64-240">Green</span></span>| <span data-ttu-id="e5b64-241">共享作用域: 社区。</span><span class="sxs-lookup"><span data-stu-id="e5b64-241">Sharing scope: Community.</span></span> <span data-ttu-id="e5b64-242">指标可与安全社区共享。</span><span class="sxs-lookup"><span data-stu-id="e5b64-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="e5b64-243">亮</span><span class="sxs-lookup"><span data-stu-id="e5b64-243">Amber</span></span>| <span data-ttu-id="e5b64-244">共享作用域: 受限。</span><span class="sxs-lookup"><span data-stu-id="e5b64-244">Sharing scope: Limited.</span></span> <span data-ttu-id="e5b64-245">这是指示器的默认设置, 并限制仅与实施了威胁智能的服务和服务运算符共享:2) 其系统表现为与指示器一致的行为的客户。</span><span class="sxs-lookup"><span data-stu-id="e5b64-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="e5b64-246">红色</span><span class="sxs-lookup"><span data-stu-id="e5b64-246">Red</span></span>| <span data-ttu-id="e5b64-247">共享作用域: 个人。</span><span class="sxs-lookup"><span data-stu-id="e5b64-247">Sharing scope: Personal.</span></span> <span data-ttu-id="e5b64-248">这些指标仅可直接共享, 最好是人员。</span><span class="sxs-lookup"><span data-stu-id="e5b64-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="e5b64-249">通常情况下, TLP 红色指示器不会引入, 因为其预定义限制。</span><span class="sxs-lookup"><span data-stu-id="e5b64-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="e5b64-250">如果提交了 TLP 红色指示器, 则**passiveOnly**属性也应设置为`True` 。</span><span class="sxs-lookup"><span data-stu-id="e5b64-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="e5b64-251">响应</span><span class="sxs-lookup"><span data-stu-id="e5b64-251">Response</span></span>

<span data-ttu-id="e5b64-252">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e5b64-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="e5b64-253">如果使用可选请求标头, 则该方法将在`200 OK`响应正文中返回响应代码和更新的[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e5b64-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5b64-254">示例</span><span class="sxs-lookup"><span data-stu-id="e5b64-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="e5b64-255">示例 1: 不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="e5b64-255">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e5b64-256">请求</span><span class="sxs-lookup"><span data-stu-id="e5b64-256">Request</span></span>

<span data-ttu-id="e5b64-257">以下是不带`Prefer`标头的请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5b64-257">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5b64-258">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e5b64-258">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5b64-259">C#</span><span class="sxs-lookup"><span data-stu-id="e5b64-259">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5b64-260">Javascript</span><span class="sxs-lookup"><span data-stu-id="e5b64-260">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5b64-261">目标-C</span><span class="sxs-lookup"><span data-stu-id="e5b64-261">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5b64-262">Java</span><span class="sxs-lookup"><span data-stu-id="e5b64-262">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5b64-263">响应</span><span class="sxs-lookup"><span data-stu-id="e5b64-263">Response</span></span>

<span data-ttu-id="e5b64-264">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5b64-264">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="e5b64-265">示例 2: 具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="e5b64-265">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="e5b64-266">请求</span><span class="sxs-lookup"><span data-stu-id="e5b64-266">Request</span></span>

<span data-ttu-id="e5b64-267">以下是包含`Prefer`标头的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="e5b64-267">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e5b64-268">响应</span><span class="sxs-lookup"><span data-stu-id="e5b64-268">Response</span></span>

<span data-ttu-id="e5b64-269">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e5b64-269">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="e5b64-270">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e5b64-270">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5b64-271">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5b64-271">All the properties will be returned from an actual call.</span></span>

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
