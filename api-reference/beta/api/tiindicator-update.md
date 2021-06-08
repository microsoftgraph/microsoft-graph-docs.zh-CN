---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f10370177565a1cbd92fad29bc1547bc042cc7b6
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786304"
---
# <a name="update-tiindicator"></a><span data-ttu-id="2e1d7-103">更新 tiIndicator</span><span class="sxs-lookup"><span data-stu-id="2e1d7-103">Update tiIndicator</span></span>

<span data-ttu-id="2e1d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e1d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e1d7-105">更新 [tiIndicator 对象](../resources/tiindicator.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e1d7-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e1d7-106">Permissions</span></span>

<span data-ttu-id="2e1d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e1d7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e1d7-109">Permission type</span></span>                        | <span data-ttu-id="2e1d7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e1d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e1d7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e1d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e1d7-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2e1d7-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="2e1d7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e1d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e1d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-114">Not supported.</span></span> |
| <span data-ttu-id="2e1d7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e1d7-115">Application</span></span>                            | <span data-ttu-id="2e1d7-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2e1d7-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e1d7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e1d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e1d7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e1d7-118">Request headers</span></span>

| <span data-ttu-id="2e1d7-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e1d7-119">Name</span></span>       | <span data-ttu-id="2e1d7-120">说明</span><span class="sxs-lookup"><span data-stu-id="2e1d7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2e1d7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e1d7-121">Authorization</span></span> | <span data-ttu-id="2e1d7-122">Bearer {code} **必填**</span><span class="sxs-lookup"><span data-stu-id="2e1d7-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="2e1d7-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="2e1d7-123">Prefer</span></span> | <span data-ttu-id="2e1d7-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="2e1d7-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e1d7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e1d7-125">Request body</span></span>

<span data-ttu-id="2e1d7-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2e1d7-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2e1d7-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="2e1d7-129">所需字段包括 `id` `expirationDateTime` `targetProduct` ：、、。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="2e1d7-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e1d7-130">Property</span></span>     | <span data-ttu-id="2e1d7-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e1d7-131">Type</span></span>        | <span data-ttu-id="2e1d7-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e1d7-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e1d7-133">action</span><span class="sxs-lookup"><span data-stu-id="2e1d7-133">action</span></span>|<span data-ttu-id="2e1d7-134">string</span><span class="sxs-lookup"><span data-stu-id="2e1d7-134">string</span></span>| <span data-ttu-id="2e1d7-135">当 targetProduct 安全工具中的指示器匹配时要应用的操作。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="2e1d7-136">可取值为：`unknown`、`allow`、`block`、`alert`。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="2e1d7-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="2e1d7-137">activityGroupNames</span></span>|<span data-ttu-id="2e1d7-138">String collection</span><span class="sxs-lookup"><span data-stu-id="2e1d7-138">String collection</span></span>|<span data-ttu-id="2e1d7-139">网络威胁情报名称 (威胁) 威胁指示器涵盖的恶意活动的各方提供。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="2e1d7-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="2e1d7-140">additionalInformation</span></span>|<span data-ttu-id="2e1d7-141">String</span><span class="sxs-lookup"><span data-stu-id="2e1d7-141">String</span></span>|<span data-ttu-id="2e1d7-142">可以放置其他 tiIndicator 属性未覆盖的指示器的额外数据到的捕获区域。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="2e1d7-143">放置在 additionalInformation 的数据通常不会由 targetProduct 安全工具使用。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="2e1d7-144">confidence</span><span class="sxs-lookup"><span data-stu-id="2e1d7-144">confidence</span></span>|<span data-ttu-id="2e1d7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2e1d7-145">Int32</span></span>|<span data-ttu-id="2e1d7-146">表示指示器内数据准确识别恶意行为的置信度整数。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="2e1d7-147">可接受的值为 0 – 100，100 为最高值。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="2e1d7-148">description</span><span class="sxs-lookup"><span data-stu-id="2e1d7-148">description</span></span>|<span data-ttu-id="2e1d7-149">String</span><span class="sxs-lookup"><span data-stu-id="2e1d7-149">String</span></span>|<span data-ttu-id="2e1d7-150">简要 (指示器所代表的威胁) 少于 100 个字符。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="2e1d7-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="2e1d7-151">diamondModel</span></span>|[<span data-ttu-id="2e1d7-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="2e1d7-152">diamondModel</span></span>](../resources/tiindicator.md#diamondmodel-values)|<span data-ttu-id="2e1d7-153">存在此指示器的菱形模型区域。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="2e1d7-154">可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="2e1d7-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2e1d7-155">expirationDateTime</span></span>|<span data-ttu-id="2e1d7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e1d7-156">DateTimeOffset</span></span>| <span data-ttu-id="2e1d7-157">指示指示器何时过期的 DateTime 字符串。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="2e1d7-158">所有指示器都必须具有过期日期，以避免在系统中保留过时的指示器。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="2e1d7-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e1d7-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="2e1d7-161">externalId</span><span class="sxs-lookup"><span data-stu-id="2e1d7-161">externalId</span></span>|<span data-ttu-id="2e1d7-162">String</span><span class="sxs-lookup"><span data-stu-id="2e1d7-162">String</span></span>|<span data-ttu-id="2e1d7-163">将指示器与指示器提供程序的系统连接在一起 (标识号，例如外键) 。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="2e1d7-164">isActive</span><span class="sxs-lookup"><span data-stu-id="2e1d7-164">isActive</span></span>|<span data-ttu-id="2e1d7-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e1d7-165">Boolean</span></span>|<span data-ttu-id="2e1d7-166">用于在系统内停用指示器。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="2e1d7-167">默认情况下，提交的任何指示器都设置为活动。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="2e1d7-168">但是，提供商可能会提交现有指示器（此设置为"False"）来停用系统指示器。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="2e1d7-169">killChain</span><span class="sxs-lookup"><span data-stu-id="2e1d7-169">killChain</span></span>|<span data-ttu-id="2e1d7-170">[killChain](../resources/tiindicator.md#killchain-values) 集合</span><span class="sxs-lookup"><span data-stu-id="2e1d7-170">[killChain](../resources/tiindicator.md#killchain-values) collection</span></span>|<span data-ttu-id="2e1d7-171">一个字符串的 JSON 数组，描述此指示器指向击杀链上的哪个点。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="2e1d7-172">有关确切值，请参阅下面的"killChain 值"。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="2e1d7-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="2e1d7-173">knownFalsePositives</span></span>|<span data-ttu-id="2e1d7-174">String</span><span class="sxs-lookup"><span data-stu-id="2e1d7-174">String</span></span>|<span data-ttu-id="2e1d7-175">指示符可能导致误报的方案。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="2e1d7-176">这应该是可读文本。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="2e1d7-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e1d7-177">lastReportedDateTime</span></span>|<span data-ttu-id="2e1d7-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e1d7-178">DateTimeOffset</span></span>|<span data-ttu-id="2e1d7-179">上一次看到指示器的时间。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-179">The last time the indicator was seen.</span></span> <span data-ttu-id="2e1d7-180">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e1d7-181">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2e1d7-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2e1d7-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="2e1d7-182">malwareFamilyNames</span></span>|<span data-ttu-id="2e1d7-183">String collection</span><span class="sxs-lookup"><span data-stu-id="2e1d7-183">String collection</span></span>|<span data-ttu-id="2e1d7-184">与指示器关联的恶意软件系列名称（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="2e1d7-185">Microsoft 首选 Microsoft 恶意软件系列名称（如果可以通过安全智能威胁Windows Defender[找到）。](https://www.microsoft.com/wdsi/threats)</span><span class="sxs-lookup"><span data-stu-id="2e1d7-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="2e1d7-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="2e1d7-186">passiveOnly</span></span>|<span data-ttu-id="2e1d7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e1d7-187">Boolean</span></span>|<span data-ttu-id="2e1d7-188">确定指示器是否应触发对最终用户可见的事件。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="2e1d7-189">设置为"true"时，安全工具不会通知最终用户"点击"已发生。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="2e1d7-190">这通常被安全产品视为审核或静默模式，在此模式下，安全产品只会记录发生匹配的情况，但不执行该操作。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="2e1d7-191">默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-191">Default value is false.</span></span>|
|<span data-ttu-id="2e1d7-192">severity</span><span class="sxs-lookup"><span data-stu-id="2e1d7-192">severity</span></span>|<span data-ttu-id="2e1d7-193">Int32</span><span class="sxs-lookup"><span data-stu-id="2e1d7-193">Int32</span></span>|<span data-ttu-id="2e1d7-194">表示由指示器内的数据标识的恶意行为严重性的整数。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="2e1d7-195">可接受的值为 0 – 5，其中 5 表示最严重，0 表示不严重。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="2e1d7-196">默认值为 3。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-196">Default value is 3.</span></span>|
|<span data-ttu-id="2e1d7-197">标记</span><span class="sxs-lookup"><span data-stu-id="2e1d7-197">tags</span></span>|<span data-ttu-id="2e1d7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="2e1d7-198">String collection</span></span>|<span data-ttu-id="2e1d7-199">存储任意标记/关键字的字符串的 JSON 数组。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="2e1d7-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="2e1d7-200">tlpLevel</span></span>|[<span data-ttu-id="2e1d7-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="2e1d7-201">tlpLevel</span></span>](../resources/tiindicator.md#tlplevel-values)| <span data-ttu-id="2e1d7-202">指示器的流量光协议值。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="2e1d7-203">可取值为：`unknown`、`white`、`green`、`amber`、`red`。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|


## <a name="response"></a><span data-ttu-id="2e1d7-204">响应</span><span class="sxs-lookup"><span data-stu-id="2e1d7-204">Response</span></span>

<span data-ttu-id="2e1d7-205">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-205">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="2e1d7-206">如果使用可选请求标头，则该方法在响应正文中返回 响应代码和更新的 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-206">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e1d7-207">示例</span><span class="sxs-lookup"><span data-stu-id="2e1d7-207">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="2e1d7-208">示例 1：不带 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="2e1d7-208">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="2e1d7-209">请求</span><span class="sxs-lookup"><span data-stu-id="2e1d7-209">Request</span></span>

<span data-ttu-id="2e1d7-210">下面是一个没有 标头的请求 `Prefer` 示例。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-210">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e1d7-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e1d7-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="2e1d7-212">C#</span><span class="sxs-lookup"><span data-stu-id="2e1d7-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e1d7-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e1d7-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e1d7-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e1d7-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e1d7-215">Java</span><span class="sxs-lookup"><span data-stu-id="2e1d7-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2e1d7-216">响应</span><span class="sxs-lookup"><span data-stu-id="2e1d7-216">Response</span></span>

<span data-ttu-id="2e1d7-217">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-217">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="2e1d7-218">示例 2：具有 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="2e1d7-218">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="2e1d7-219">请求</span><span class="sxs-lookup"><span data-stu-id="2e1d7-219">Request</span></span>

<span data-ttu-id="2e1d7-220">下面是包含 标头的请求 `Prefer` 示例。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-220">The following is an example of the request that includes the `Prefer` header.</span></span>


# <a name="http"></a>[<span data-ttu-id="2e1d7-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e1d7-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_2"
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
# <a name="c"></a>[<span data-ttu-id="2e1d7-222">C#</span><span class="sxs-lookup"><span data-stu-id="2e1d7-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e1d7-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e1d7-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e1d7-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e1d7-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e1d7-225">Java</span><span class="sxs-lookup"><span data-stu-id="2e1d7-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2e1d7-226">响应</span><span class="sxs-lookup"><span data-stu-id="2e1d7-226">Response</span></span>

<span data-ttu-id="2e1d7-227">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-227">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2e1d7-228">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2e1d7-228">The response object shown here might be shortened for readability.</span></span>

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


