---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6f6adcc3e4f069297fd0b22dee24a33331d040cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076508"
---
# <a name="update-tiindicator"></a><span data-ttu-id="5bd8e-103">更新 tiIndicator</span><span class="sxs-lookup"><span data-stu-id="5bd8e-103">Update tiIndicator</span></span>

<span data-ttu-id="5bd8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bd8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd8e-105">更新 [tiIndicator](../resources/tiindicator.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bd8e-106">权限</span><span class="sxs-lookup"><span data-stu-id="5bd8e-106">Permissions</span></span>

<span data-ttu-id="5bd8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bd8e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bd8e-109">Permission type</span></span>                        | <span data-ttu-id="5bd8e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bd8e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5bd8e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd8e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bd8e-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5bd8e-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="5bd8e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bd8e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-114">Not supported.</span></span> |
| <span data-ttu-id="5bd8e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bd8e-115">Application</span></span>                            | <span data-ttu-id="5bd8e-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="5bd8e-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bd8e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bd8e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5bd8e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bd8e-118">Request headers</span></span>

| <span data-ttu-id="5bd8e-119">名称</span><span class="sxs-lookup"><span data-stu-id="5bd8e-119">Name</span></span>       | <span data-ttu-id="5bd8e-120">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5bd8e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd8e-121">Authorization</span></span> | <span data-ttu-id="5bd8e-122">**必需**的持有者 {代码}</span><span class="sxs-lookup"><span data-stu-id="5bd8e-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="5bd8e-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="5bd8e-123">Prefer</span></span> | <span data-ttu-id="5bd8e-124">return = 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bd8e-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bd8e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bd8e-125">Request body</span></span>

<span data-ttu-id="5bd8e-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5bd8e-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5bd8e-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="5bd8e-129">必填字段为： `id` 、 `expirationDateTime` 、 `targetProduct` 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="5bd8e-130">属性</span><span class="sxs-lookup"><span data-stu-id="5bd8e-130">Property</span></span>     | <span data-ttu-id="5bd8e-131">类型</span><span class="sxs-lookup"><span data-stu-id="5bd8e-131">Type</span></span>        | <span data-ttu-id="5bd8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5bd8e-133">action</span><span class="sxs-lookup"><span data-stu-id="5bd8e-133">action</span></span>|<span data-ttu-id="5bd8e-134">string</span><span class="sxs-lookup"><span data-stu-id="5bd8e-134">string</span></span>| <span data-ttu-id="5bd8e-135">在 targetProduct 安全工具中匹配指标时要应用的操作。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="5bd8e-136">可取值为：`unknown`、`allow`、`block`、`alert`。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="5bd8e-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="5bd8e-137">activityGroupNames</span></span>|<span data-ttu-id="5bd8e-138">String 集合</span><span class="sxs-lookup"><span data-stu-id="5bd8e-138">String collection</span></span>|<span data-ttu-id="5bd8e-139">负责威胁指示器所涵盖的恶意活动的各方) 的网络威胁智能名称 (s。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="5bd8e-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="5bd8e-140">additionalInformation</span></span>|<span data-ttu-id="5bd8e-141">String</span><span class="sxs-lookup"><span data-stu-id="5bd8e-141">String</span></span>|<span data-ttu-id="5bd8e-142">可以放置其他 tiIndicator 属性中未涵盖的指标中的额外数据的 "容器" 区域。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="5bd8e-143">放置在 additionalInformation 中的数据通常不会被 targetProduct 安全工具使用。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="5bd8e-144">confidence</span><span class="sxs-lookup"><span data-stu-id="5bd8e-144">confidence</span></span>|<span data-ttu-id="5bd8e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd8e-145">Int32</span></span>|<span data-ttu-id="5bd8e-146">一个整数，表示对指示器中的数据准确标识恶意行为的可信度。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="5bd8e-147">可接受的值为0–100，100的值为最高。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="5bd8e-148">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-148">description</span></span>|<span data-ttu-id="5bd8e-149">String</span><span class="sxs-lookup"><span data-stu-id="5bd8e-149">String</span></span>|<span data-ttu-id="5bd8e-150">由指示器表示的威胁 (100 个字符或更少) 的简短说明。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="5bd8e-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="5bd8e-151">diamondModel</span></span>|[<span data-ttu-id="5bd8e-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="5bd8e-152">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="5bd8e-153">此指示器所在的菱形模型的面积。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="5bd8e-154">可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="5bd8e-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd8e-155">expirationDateTime</span></span>|<span data-ttu-id="5bd8e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd8e-156">DateTimeOffset</span></span>| <span data-ttu-id="5bd8e-157">指示指示器过期时间的日期/时间字符串。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="5bd8e-158">所有指标都必须具有到期日期，以避免系统中的陈旧指示器持久化。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="5bd8e-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5bd8e-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5bd8e-161">externalId</span><span class="sxs-lookup"><span data-stu-id="5bd8e-161">externalId</span></span>|<span data-ttu-id="5bd8e-162">String</span><span class="sxs-lookup"><span data-stu-id="5bd8e-162">String</span></span>|<span data-ttu-id="5bd8e-163">将指示器与指示器提供程序的系统相结合的标识号 (例如，外键) 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="5bd8e-164">isActive</span><span class="sxs-lookup"><span data-stu-id="5bd8e-164">isActive</span></span>|<span data-ttu-id="5bd8e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd8e-165">Boolean</span></span>|<span data-ttu-id="5bd8e-166">用于停用系统中的指示器。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="5bd8e-167">默认情况下，提交的任何指示器都设置为活动状态。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="5bd8e-168">但是，提供程序可能会将此设置为 "False" 的现有指示器提交到系统中停用指示器。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="5bd8e-169">killChain</span><span class="sxs-lookup"><span data-stu-id="5bd8e-169">killChain</span></span>|<span data-ttu-id="5bd8e-170">[killChain](#killchain-values) 集合</span><span class="sxs-lookup"><span data-stu-id="5bd8e-170">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="5bd8e-171">一个 JSON 字符串数组，用于描述此指示器针对终止链上的哪个点或点。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="5bd8e-172">有关确切值，请参阅下面的 "killChain 值"。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="5bd8e-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="5bd8e-173">knownFalsePositives</span></span>|<span data-ttu-id="5bd8e-174">String</span><span class="sxs-lookup"><span data-stu-id="5bd8e-174">String</span></span>|<span data-ttu-id="5bd8e-175">指示符可能导致误报的情况。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="5bd8e-176">这应该是可读的文本。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="5bd8e-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd8e-177">lastReportedDateTime</span></span>|<span data-ttu-id="5bd8e-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd8e-178">DateTimeOffset</span></span>|<span data-ttu-id="5bd8e-179">上次发现指示器的时间。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-179">The last time the indicator was seen.</span></span> <span data-ttu-id="5bd8e-180">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5bd8e-181">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5bd8e-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5bd8e-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="5bd8e-182">malwareFamilyNames</span></span>|<span data-ttu-id="5bd8e-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="5bd8e-183">String collection</span></span>|<span data-ttu-id="5bd8e-184">与指示器关联的恶意软件系列名称（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="5bd8e-185">如果所有可能都可以通过 Windows Defender 安全智能 [威胁百科全书](https://www.microsoft.com/wdsi/threats)找到，microsoft 将首选 microsoft 恶意软件系列名称。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="5bd8e-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="5bd8e-186">passiveOnly</span></span>|<span data-ttu-id="5bd8e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd8e-187">Boolean</span></span>|<span data-ttu-id="5bd8e-188">确定该指示符是否应触发对最终用户可见的事件。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="5bd8e-189">如果设置为 "true"，则安全工具将不会通知最终用户已发生 "命中"。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="5bd8e-190">通常情况下，这通常被视为审核或静默模式，安全产品只需记录已发生的匹配项，但不会执行该操作。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="5bd8e-191">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-191">Default value is false.</span></span>|
|<span data-ttu-id="5bd8e-192">severity</span><span class="sxs-lookup"><span data-stu-id="5bd8e-192">severity</span></span>|<span data-ttu-id="5bd8e-193">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd8e-193">Int32</span></span>|<span data-ttu-id="5bd8e-194">一个整数，表示由指示器中的数据标识的恶意行为的严重程度。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="5bd8e-195">可接受的值为0–5，其中5为最严重，0表示根本不严重。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="5bd8e-196">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-196">Default value is 3.</span></span>|
|<span data-ttu-id="5bd8e-197">tags</span><span class="sxs-lookup"><span data-stu-id="5bd8e-197">tags</span></span>|<span data-ttu-id="5bd8e-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="5bd8e-198">String collection</span></span>|<span data-ttu-id="5bd8e-199">存储任意标记/关键字的字符串的 JSON 数组。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="5bd8e-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="5bd8e-200">tlpLevel</span></span>|[<span data-ttu-id="5bd8e-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="5bd8e-201">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="5bd8e-202">指标的流量灯协议值。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="5bd8e-203">可取值为：`unknown`、`white`、`green`、`amber`、`red`。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="5bd8e-204">diamondModel 值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-204">diamondModel values</span></span>

<span data-ttu-id="5bd8e-205">有关此模型的信息，请参阅 [菱形模型](http://diamondmodel.org)。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-205">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="5bd8e-206">值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-206">Values</span></span> | <span data-ttu-id="5bd8e-207">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-207">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="5bd8e-208">对手</span><span class="sxs-lookup"><span data-stu-id="5bd8e-208">adversary</span></span>|<span data-ttu-id="5bd8e-209">该指示器描述了敌人。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-209">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="5bd8e-210">性能</span><span class="sxs-lookup"><span data-stu-id="5bd8e-210">capability</span></span>|<span data-ttu-id="5bd8e-211">该指标是入侵者的一种功能。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-211">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="5bd8e-212">基本</span><span class="sxs-lookup"><span data-stu-id="5bd8e-212">infrastructure</span></span>|<span data-ttu-id="5bd8e-213">此指标介绍了入侵者的基础结构。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-213">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="5bd8e-214">者</span><span class="sxs-lookup"><span data-stu-id="5bd8e-214">victim</span></span>|<span data-ttu-id="5bd8e-215">该指标描述敌人的牺牲品。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-215">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="5bd8e-216">killChain 值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-216">killChain values</span></span>

| <span data-ttu-id="5bd8e-217">值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-217">Values</span></span> | <span data-ttu-id="5bd8e-218">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-218">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="5bd8e-219">操作</span><span class="sxs-lookup"><span data-stu-id="5bd8e-219">Actions</span></span>|<span data-ttu-id="5bd8e-220">代表 "针对目标的操作"。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-220">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="5bd8e-221">攻击者利用受攻击的系统执行诸如分布式拒绝服务攻击之类的操作。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-221">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="5bd8e-222">C2</span><span class="sxs-lookup"><span data-stu-id="5bd8e-222">C2</span></span>|<span data-ttu-id="5bd8e-223">表示操纵受损系统时所使用的控制通道。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-223">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="5bd8e-224">Delivery</span><span class="sxs-lookup"><span data-stu-id="5bd8e-224">Delivery</span></span>|<span data-ttu-id="5bd8e-225">将攻击代码分发给受害者的过程 (例如，USB、电子邮件、网站) 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-225">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="5bd8e-226">具备</span><span class="sxs-lookup"><span data-stu-id="5bd8e-226">Exploitation</span></span>|<span data-ttu-id="5bd8e-227">利用漏洞的攻击代码 (例如，代码执行) 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-227">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="5bd8e-228">安装</span><span class="sxs-lookup"><span data-stu-id="5bd8e-228">Installation</span></span>|<span data-ttu-id="5bd8e-229">在漏洞受到攻击后安装恶意软件。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-229">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="5bd8e-230">侦查</span><span class="sxs-lookup"><span data-stu-id="5bd8e-230">Reconnaissance</span></span>|<span data-ttu-id="5bd8e-231">指标是活动组收集信息以用于将来的攻击的证据。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-231">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="5bd8e-232">Weaponization</span><span class="sxs-lookup"><span data-stu-id="5bd8e-232">Weaponization</span></span>|<span data-ttu-id="5bd8e-233">将漏洞变成攻击代码 (例如，恶意软件) 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-233">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="5bd8e-234">tlpLevel 值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-234">tlpLevel values</span></span>

<span data-ttu-id="5bd8e-235">每个指示器在提交时都必须有流量灯协议 (tlp) 值。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-235">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="5bd8e-236">此值表示给定指标的敏感度和共享作用域。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-236">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="5bd8e-237">值</span><span class="sxs-lookup"><span data-stu-id="5bd8e-237">Values</span></span> | <span data-ttu-id="5bd8e-238">说明</span><span class="sxs-lookup"><span data-stu-id="5bd8e-238">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="5bd8e-239">白色</span><span class="sxs-lookup"><span data-stu-id="5bd8e-239">White</span></span>| <span data-ttu-id="5bd8e-240">共享范围：无限制。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-240">Sharing scope: Unlimited.</span></span> <span data-ttu-id="5bd8e-241">指示器可以自由共享，无需限制。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-241">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="5bd8e-242">绿色</span><span class="sxs-lookup"><span data-stu-id="5bd8e-242">Green</span></span>| <span data-ttu-id="5bd8e-243">共享作用域：社区。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-243">Sharing scope: Community.</span></span> <span data-ttu-id="5bd8e-244">指标可与安全社区共享。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-244">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="5bd8e-245">亮</span><span class="sxs-lookup"><span data-stu-id="5bd8e-245">Amber</span></span>| <span data-ttu-id="5bd8e-246">共享作用域：受限。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-246">Sharing scope: Limited.</span></span> <span data-ttu-id="5bd8e-247">这是指示器的默认设置，并且仅将共享限制为仅有需要了解的内容： 1) 服务和实施威胁智能的服务运算符;2) 其系统 (s) 表现为与指示器一致的行为的客户。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-247">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="5bd8e-248">红色</span><span class="sxs-lookup"><span data-stu-id="5bd8e-248">Red</span></span>| <span data-ttu-id="5bd8e-249">共享作用域：个人。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-249">Sharing scope: Personal.</span></span> <span data-ttu-id="5bd8e-250">这些指标仅可直接共享，最好是人员。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-250">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="5bd8e-251">通常情况下，TLP 红色指示器不会引入，因为其预定义限制。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-251">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="5bd8e-252">如果提交了 TLP 红色指示器，则 **passiveOnly** 属性也应设置为 `True` 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-252">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="5bd8e-253">响应</span><span class="sxs-lookup"><span data-stu-id="5bd8e-253">Response</span></span>

<span data-ttu-id="5bd8e-254">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-254">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="5bd8e-255">如果使用可选请求标头，则该方法将 `200 OK` 在响应正文中返回响应代码和更新的 [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-255">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5bd8e-256">示例</span><span class="sxs-lookup"><span data-stu-id="5bd8e-256">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="5bd8e-257">示例1：不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="5bd8e-257">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="5bd8e-258">请求</span><span class="sxs-lookup"><span data-stu-id="5bd8e-258">Request</span></span>

<span data-ttu-id="5bd8e-259">以下是不带标头的请求示例 `Prefer` 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-259">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="5bd8e-260">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bd8e-260">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5bd8e-261">C#</span><span class="sxs-lookup"><span data-stu-id="5bd8e-261">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bd8e-262">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bd8e-262">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bd8e-263">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bd8e-263">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5bd8e-264">响应</span><span class="sxs-lookup"><span data-stu-id="5bd8e-264">Response</span></span>

<span data-ttu-id="5bd8e-265">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-265">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="5bd8e-266">示例2：具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="5bd8e-266">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="5bd8e-267">请求</span><span class="sxs-lookup"><span data-stu-id="5bd8e-267">Request</span></span>

<span data-ttu-id="5bd8e-268">以下是包含标头的请求的示例 `Prefer` 。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-268">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="5bd8e-269">响应</span><span class="sxs-lookup"><span data-stu-id="5bd8e-269">Response</span></span>

<span data-ttu-id="5bd8e-270">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-270">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5bd8e-271">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-271">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5bd8e-272">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5bd8e-272">All the properties will be returned from an actual call.</span></span>

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


