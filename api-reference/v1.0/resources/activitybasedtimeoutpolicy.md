---
title: activityBasedTimeoutPolicy 资源类型
description: 表示一个策略，该策略可控制支持基于活动的超时功能的应用程序的 Web 会话的空闲超时。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d2031af6b744bbd81e4e6849e5ed78978396e8c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448882"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="49d9f-103">activityBasedTimeoutPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="49d9f-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="49d9f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49d9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49d9f-105">表示一个策略，该策略可控制支持基于活动的超时功能的应用程序的 Web 会话的空闲超时。</span><span class="sxs-lookup"><span data-stu-id="49d9f-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="49d9f-106">应用程序在一段时间不活动后强制执行自动注销。</span><span class="sxs-lookup"><span data-stu-id="49d9f-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="49d9f-107">此类型的策略只能在组织级别应用， (**isOrganizationDefault** 属性设置为 `true`) 。</span><span class="sxs-lookup"><span data-stu-id="49d9f-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="49d9f-108">继承自 [stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="49d9f-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="49d9f-109">Methods</span><span class="sxs-lookup"><span data-stu-id="49d9f-109">Methods</span></span>

| <span data-ttu-id="49d9f-110">方法</span><span class="sxs-lookup"><span data-stu-id="49d9f-110">Method</span></span>       | <span data-ttu-id="49d9f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="49d9f-111">Return Type</span></span> | <span data-ttu-id="49d9f-112">说明</span><span class="sxs-lookup"><span data-stu-id="49d9f-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="49d9f-113">列出 activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="49d9f-113">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="49d9f-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="49d9f-115">读取 activityBasedTimeoutPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49d9f-115">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="49d9f-116">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-116">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="49d9f-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="49d9f-118">创建 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="49d9f-118">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="49d9f-119">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-119">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="49d9f-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="49d9f-121">读取 activityBasedTimeoutPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49d9f-121">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="49d9f-122">更新 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="49d9f-123">无</span><span class="sxs-lookup"><span data-stu-id="49d9f-123">None</span></span> | <span data-ttu-id="49d9f-124">更新 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="49d9f-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="49d9f-125">删除 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="49d9f-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="49d9f-126">无</span><span class="sxs-lookup"><span data-stu-id="49d9f-126">None</span></span> | <span data-ttu-id="49d9f-127">删除 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="49d9f-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="49d9f-128">属性</span><span class="sxs-lookup"><span data-stu-id="49d9f-128">Properties</span></span>

| <span data-ttu-id="49d9f-129">属性</span><span class="sxs-lookup"><span data-stu-id="49d9f-129">Property</span></span>     | <span data-ttu-id="49d9f-130">类型</span><span class="sxs-lookup"><span data-stu-id="49d9f-130">Type</span></span>        | <span data-ttu-id="49d9f-131">说明</span><span class="sxs-lookup"><span data-stu-id="49d9f-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="49d9f-132">id</span><span class="sxs-lookup"><span data-stu-id="49d9f-132">id</span></span>|<span data-ttu-id="49d9f-133">String</span><span class="sxs-lookup"><span data-stu-id="49d9f-133">String</span></span>| <span data-ttu-id="49d9f-134">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="49d9f-134">Unique identifier for this policy.</span></span> <span data-ttu-id="49d9f-135">只读。</span><span class="sxs-lookup"><span data-stu-id="49d9f-135">Read-only.</span></span>|
|<span data-ttu-id="49d9f-136">definition</span><span class="sxs-lookup"><span data-stu-id="49d9f-136">definition</span></span>|<span data-ttu-id="49d9f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="49d9f-137">String collection</span></span>| <span data-ttu-id="49d9f-138">包含 JSON 字符串的字符串集合，用于定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="49d9f-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="49d9f-139">有关此属性的 JSON 架构的详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="49d9f-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="49d9f-140">必需。</span><span class="sxs-lookup"><span data-stu-id="49d9f-140">Required.</span></span>|
|<span data-ttu-id="49d9f-141">description</span><span class="sxs-lookup"><span data-stu-id="49d9f-141">description</span></span>|<span data-ttu-id="49d9f-142">String</span><span class="sxs-lookup"><span data-stu-id="49d9f-142">String</span></span>| <span data-ttu-id="49d9f-143">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="49d9f-143">Description for this policy.</span></span>|
|<span data-ttu-id="49d9f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="49d9f-144">displayName</span></span>|<span data-ttu-id="49d9f-145">String</span><span class="sxs-lookup"><span data-stu-id="49d9f-145">String</span></span>| <span data-ttu-id="49d9f-146">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="49d9f-146">Display name for this policy.</span></span> <span data-ttu-id="49d9f-147">必填。</span><span class="sxs-lookup"><span data-stu-id="49d9f-147">Required.</span></span>|
|<span data-ttu-id="49d9f-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="49d9f-148">isOrganizationDefault</span></span>|<span data-ttu-id="49d9f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="49d9f-149">Boolean</span></span>|<span data-ttu-id="49d9f-150">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="49d9f-150">If set to true, activates this policy.</span></span> <span data-ttu-id="49d9f-151">同一策略类型可以有很多策略，但只有一个策略可以激活为组织默认设置。</span><span class="sxs-lookup"><span data-stu-id="49d9f-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="49d9f-152">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="49d9f-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="49d9f-153">基于活动的超时策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="49d9f-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="49d9f-154">下面的属性构成表示基于活动的超时策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="49d9f-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="49d9f-155">此 JSON 对象 **必须转换为带** 转义引号的字符串，以插入到 **定义** 属性中。</span><span class="sxs-lookup"><span data-stu-id="49d9f-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="49d9f-156">下面显示了 JSON 格式的示例：</span><span class="sxs-lookup"><span data-stu-id="49d9f-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="49d9f-157">**注意：** 这些属性中所有持续时间的指定格式为"dd.hh：mm：ss"。</span><span class="sxs-lookup"><span data-stu-id="49d9f-157">**Note:** All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="49d9f-158">**注意：** 以"days"表示的属性的最大值比表示的天数短 1 秒。</span><span class="sxs-lookup"><span data-stu-id="49d9f-158">**Note:** Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="49d9f-159">例如，最大值 1 天指定为"23：59：59"。</span><span class="sxs-lookup"><span data-stu-id="49d9f-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="49d9f-160">属性</span><span class="sxs-lookup"><span data-stu-id="49d9f-160">Property</span></span>     | <span data-ttu-id="49d9f-161">类型</span><span class="sxs-lookup"><span data-stu-id="49d9f-161">Type</span></span>   |<span data-ttu-id="49d9f-162">说明</span><span class="sxs-lookup"><span data-stu-id="49d9f-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="49d9f-163">版本</span><span class="sxs-lookup"><span data-stu-id="49d9f-163">Version</span></span>|<span data-ttu-id="49d9f-164">整数</span><span class="sxs-lookup"><span data-stu-id="49d9f-164">Integer</span></span>|<span data-ttu-id="49d9f-165">策略版本。</span><span class="sxs-lookup"><span data-stu-id="49d9f-165">Policy version.</span></span> <span data-ttu-id="49d9f-166">设置值 1。</span><span class="sxs-lookup"><span data-stu-id="49d9f-166">Set value of 1.</span></span> <span data-ttu-id="49d9f-167">必填。</span><span class="sxs-lookup"><span data-stu-id="49d9f-167">Required.</span></span>|
|<span data-ttu-id="49d9f-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="49d9f-168">ApplicationPolicies</span></span>|<span data-ttu-id="49d9f-169">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="49d9f-169">JSON object</span></span>|<span data-ttu-id="49d9f-170">应用程序策略的集合。</span><span class="sxs-lookup"><span data-stu-id="49d9f-170">Collection of application policy.</span></span> <span data-ttu-id="49d9f-171">应用程序策略是 ApplicationId 和 WebSessionIdleTimeout 的组合：</span><span class="sxs-lookup"><span data-stu-id="49d9f-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="49d9f-172">**ApplicationId**：允许的值：</span><span class="sxs-lookup"><span data-stu-id="49d9f-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="49d9f-173">默认值：将策略应用于支持基于活动的超时功能但没有应用程序特定覆盖的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="49d9f-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="49d9f-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c：将策略应用于 Azure 门户</span><span class="sxs-lookup"><span data-stu-id="49d9f-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="49d9f-175">**WebSessionIdleTimeout：** 用户处于不活动状态期间，此后用户的 Web 会话被视为已过期。</span><span class="sxs-lookup"><span data-stu-id="49d9f-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="49d9f-176">最小值为 5 分钟;最大值为 1 天。</span><span class="sxs-lookup"><span data-stu-id="49d9f-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="49d9f-177">关系</span><span class="sxs-lookup"><span data-stu-id="49d9f-177">Relationships</span></span>

<span data-ttu-id="49d9f-178">无</span><span class="sxs-lookup"><span data-stu-id="49d9f-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49d9f-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49d9f-179">JSON representation</span></span>

<span data-ttu-id="49d9f-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49d9f-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "definition": ["String"],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityBasedTimeoutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

