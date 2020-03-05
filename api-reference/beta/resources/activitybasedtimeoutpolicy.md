---
title: activityBasedTimeoutPolicy 资源类型
description: 表示一个策略，该策略可控制支持基于活动的超时功能的应用程序的 web 会话的空闲超时。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c4255315c8eef4de0895cf7c01569a2ceeb8272e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508434"
---
# <a name="activitybasedtimeoutpolicy-resource-type"></a><span data-ttu-id="2617b-103">activityBasedTimeoutPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="2617b-103">activityBasedTimeoutPolicy resource type</span></span>

<span data-ttu-id="2617b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2617b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2617b-105">表示一个策略，该策略可控制支持基于活动的超时功能的应用程序的 web 会话的空闲超时。</span><span class="sxs-lookup"><span data-stu-id="2617b-105">Represents a policy that can control the idle timeout for web sessions for applications that support activity-based timeout functionality.</span></span> <span data-ttu-id="2617b-106">应用程序在处于非活动状态一段时间后强制自动 signout。</span><span class="sxs-lookup"><span data-stu-id="2617b-106">Applications enforce automatic signout after a period of inactivity.</span></span> <span data-ttu-id="2617b-107">此类型的策略仅可在组织级别应用（通过将**isOrganizationDefault**属性设置为`true`）。</span><span class="sxs-lookup"><span data-stu-id="2617b-107">This type of policy can only be applied at the organization level (by setting the **isOrganizationDefault** property to `true`).</span></span>

<span data-ttu-id="2617b-108">继承自[stsPolicy](stsPolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="2617b-108">Inherits from [stsPolicy](stsPolicy.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2617b-109">方法</span><span class="sxs-lookup"><span data-stu-id="2617b-109">Methods</span></span>

| <span data-ttu-id="2617b-110">方法</span><span class="sxs-lookup"><span data-stu-id="2617b-110">Method</span></span>       | <span data-ttu-id="2617b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2617b-111">Return Type</span></span> | <span data-ttu-id="2617b-112">说明</span><span class="sxs-lookup"><span data-stu-id="2617b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2617b-113">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-113">Create activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-post-activitybasedtimeoutpolicies.md) | [<span data-ttu-id="2617b-114">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-114">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="2617b-115">创建 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="2617b-115">Create an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="2617b-116">获取 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-116">Get activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-get.md) | [<span data-ttu-id="2617b-117">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-117">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="2617b-118">读取 activityBasedTimeoutPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2617b-118">Read properties and relationships of an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="2617b-119">列出 activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="2617b-119">List activityBasedTimeoutPolicies</span></span>](../api/activitybasedtimeoutpolicy-list.md) | [<span data-ttu-id="2617b-120">activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-120">activityBasedTimeoutPolicy</span></span>](activitybasedtimeoutpolicy.md) | <span data-ttu-id="2617b-121">读取 activityBasedTimeoutPolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2617b-121">Read properties and relationships of activityBasedTimeoutPolicy objects.</span></span> |
| [<span data-ttu-id="2617b-122">更新 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-122">Update activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-update.md) | <span data-ttu-id="2617b-123">无</span><span class="sxs-lookup"><span data-stu-id="2617b-123">None</span></span> | <span data-ttu-id="2617b-124">更新 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="2617b-124">Update an activityBasedTimeoutPolicy object.</span></span> |
| [<span data-ttu-id="2617b-125">删除 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="2617b-125">Delete activityBasedTimeoutPolicy</span></span>](../api/activitybasedtimeoutpolicy-delete.md) | <span data-ttu-id="2617b-126">无</span><span class="sxs-lookup"><span data-stu-id="2617b-126">None</span></span> | <span data-ttu-id="2617b-127">删除 activityBasedTimeoutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="2617b-127">Delete an activityBasedTimeoutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2617b-128">属性</span><span class="sxs-lookup"><span data-stu-id="2617b-128">Properties</span></span>

| <span data-ttu-id="2617b-129">属性</span><span class="sxs-lookup"><span data-stu-id="2617b-129">Property</span></span>     | <span data-ttu-id="2617b-130">类型</span><span class="sxs-lookup"><span data-stu-id="2617b-130">Type</span></span>        | <span data-ttu-id="2617b-131">说明</span><span class="sxs-lookup"><span data-stu-id="2617b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2617b-132">id</span><span class="sxs-lookup"><span data-stu-id="2617b-132">id</span></span>|<span data-ttu-id="2617b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2617b-133">String</span></span>| <span data-ttu-id="2617b-134">此策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2617b-134">Unique identifier for this policy.</span></span> <span data-ttu-id="2617b-135">只读。</span><span class="sxs-lookup"><span data-stu-id="2617b-135">Read-only.</span></span>|
|<span data-ttu-id="2617b-136">定义</span><span class="sxs-lookup"><span data-stu-id="2617b-136">definition</span></span>|<span data-ttu-id="2617b-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="2617b-137">String collection</span></span>| <span data-ttu-id="2617b-138">一个包含 JSON 字符串的字符串集合，该字符串定义此策略的规则和设置。</span><span class="sxs-lookup"><span data-stu-id="2617b-138">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span> <span data-ttu-id="2617b-139">有关此属性的 JSON 架构的更多详细信息，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="2617b-139">See below for more details about the JSON schema for this property.</span></span> <span data-ttu-id="2617b-140">必需。</span><span class="sxs-lookup"><span data-stu-id="2617b-140">Required.</span></span>|
|<span data-ttu-id="2617b-141">description</span><span class="sxs-lookup"><span data-stu-id="2617b-141">description</span></span>|<span data-ttu-id="2617b-142">String</span><span class="sxs-lookup"><span data-stu-id="2617b-142">String</span></span>| <span data-ttu-id="2617b-143">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="2617b-143">Description for this policy.</span></span>|
|<span data-ttu-id="2617b-144">displayName</span><span class="sxs-lookup"><span data-stu-id="2617b-144">displayName</span></span>|<span data-ttu-id="2617b-145">String</span><span class="sxs-lookup"><span data-stu-id="2617b-145">String</span></span>| <span data-ttu-id="2617b-146">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2617b-146">Display name for this policy.</span></span> <span data-ttu-id="2617b-147">必填。</span><span class="sxs-lookup"><span data-stu-id="2617b-147">Required.</span></span>|
|<span data-ttu-id="2617b-148">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="2617b-148">isOrganizationDefault</span></span>|<span data-ttu-id="2617b-149">布尔</span><span class="sxs-lookup"><span data-stu-id="2617b-149">Boolean</span></span>|<span data-ttu-id="2617b-150">如果设置为 true，则激活此策略。</span><span class="sxs-lookup"><span data-stu-id="2617b-150">If set to true, activates this policy.</span></span> <span data-ttu-id="2617b-151">对于同一策略类型，可以有多个策略，但只有一个策略可以作为组织默认激活。</span><span class="sxs-lookup"><span data-stu-id="2617b-151">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="2617b-152">可选，默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="2617b-152">Optional, default value is false.</span></span>|


### <a name="properties-of-an-activity-based-timeout-policy-definition"></a><span data-ttu-id="2617b-153">基于活动的超时策略定义的属性</span><span class="sxs-lookup"><span data-stu-id="2617b-153">Properties of an activity-based timeout policy definition</span></span>
<span data-ttu-id="2617b-154">下面的属性构成了表示基于活动的超时策略的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2617b-154">The properties below form the JSON object that represents an activity-based timeout policy.</span></span> <span data-ttu-id="2617b-155">此 JSON 对象必须**转换为转义了引号的字符串**，以将其插入到**定义**属性中。</span><span class="sxs-lookup"><span data-stu-id="2617b-155">This JSON object must be **converted to a string with quotations escaped** to be inserted into the **definition** property.</span></span> <span data-ttu-id="2617b-156">下面以 JSON 格式显示了一个示例：</span><span class="sxs-lookup"><span data-stu-id="2617b-156">An example is shown below in JSON format:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```json
{
  "definition":["{\"ActivityBasedTimeoutPolicy\":{\"Version\":1,\"ApplicationPolicies\":[{\"ApplicationId\":\"default\",\"WebSessionIdleTimeout\":\"01:00:00\"},{\"ApplicationId\":\"c44b4083-3bb0-49c1-b47d-974e53cbdf3c\",\"WebSessionIdleTimeout\":\"00:15:00\"}]}}"]
}
```

><span data-ttu-id="2617b-157">注意：这些属性中的所有持续时间均以 "dd. hh： mm： ss" 的格式指定。</span><span class="sxs-lookup"><span data-stu-id="2617b-157">Note: All time durations in these properties are specified in the format "dd.hh:mm:ss".</span></span>

><span data-ttu-id="2617b-158">注意： "天" 中表示的属性的最大值是表示的天数的1秒。</span><span class="sxs-lookup"><span data-stu-id="2617b-158">Note: Max values for properties denoted in "days" are 1 second short of the denoted number of days.</span></span> <span data-ttu-id="2617b-159">例如，"最大值为1天" 指定为 "23:59:59"。</span><span class="sxs-lookup"><span data-stu-id="2617b-159">For example, the max value of 1 days is specified as "23:59:59".</span></span>

| <span data-ttu-id="2617b-160">属性</span><span class="sxs-lookup"><span data-stu-id="2617b-160">Property</span></span>     | <span data-ttu-id="2617b-161">类型</span><span class="sxs-lookup"><span data-stu-id="2617b-161">Type</span></span>   |<span data-ttu-id="2617b-162">说明</span><span class="sxs-lookup"><span data-stu-id="2617b-162">Description</span></span>|
|:-------------|:------|:---------|
|<span data-ttu-id="2617b-163">版本</span><span class="sxs-lookup"><span data-stu-id="2617b-163">Version</span></span>|<span data-ttu-id="2617b-164">整数</span><span class="sxs-lookup"><span data-stu-id="2617b-164">Integer</span></span>|<span data-ttu-id="2617b-165">策略版本。</span><span class="sxs-lookup"><span data-stu-id="2617b-165">Policy version.</span></span> <span data-ttu-id="2617b-166">将值设置为1。</span><span class="sxs-lookup"><span data-stu-id="2617b-166">Set value of 1.</span></span> <span data-ttu-id="2617b-167">必填。</span><span class="sxs-lookup"><span data-stu-id="2617b-167">Required.</span></span>|
|<span data-ttu-id="2617b-168">ApplicationPolicies</span><span class="sxs-lookup"><span data-stu-id="2617b-168">ApplicationPolicies</span></span>|<span data-ttu-id="2617b-169">JSON 对象</span><span class="sxs-lookup"><span data-stu-id="2617b-169">JSON object</span></span>|<span data-ttu-id="2617b-170">应用程序策略的集合。</span><span class="sxs-lookup"><span data-stu-id="2617b-170">Collection of application policy.</span></span> <span data-ttu-id="2617b-171">应用程序策略是 ApplicationId 和 WebSessionIdleTimeout 的组合：</span><span class="sxs-lookup"><span data-stu-id="2617b-171">An application policy, is a combination of an ApplicationId and a WebSessionIdleTimeout:</span></span> <br> <ul><li><span data-ttu-id="2617b-172">**ApplicationId**：允许的值：</span><span class="sxs-lookup"><span data-stu-id="2617b-172">**ApplicationId**: Allowed values:</span></span><ul><li> <span data-ttu-id="2617b-173">默认：将策略应用于所有支持基于活动的超时功能但不具有特定于应用程序的替代的应用程序</span><span class="sxs-lookup"><span data-stu-id="2617b-173">default: applies the policy to all applications that support activity-based timeout functionality but do not have application-specific override</span></span></li><li> <span data-ttu-id="2617b-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c：将策略应用于 Azure 门户</span><span class="sxs-lookup"><span data-stu-id="2617b-174">c44b4083-3bb0-49c1-b47d-974e53cbdf3c: applies the policy to the Azure Portal</span></span></li></ul></li><li><span data-ttu-id="2617b-175">**WebSessionIdleTimeout**：用户的 web 会话被认为已过期的用户非活动时段。</span><span class="sxs-lookup"><span data-stu-id="2617b-175">**WebSessionIdleTimeout**: The period of user inactivity after which the user's web session is considered expired.</span></span> <span data-ttu-id="2617b-176">最小值为5分钟;最大值为1天。</span><span class="sxs-lookup"><span data-stu-id="2617b-176">The minimum value is 5 minutes; the maximum value is 1 day.</span></span></li></ul> |


## <a name="relationships"></a><span data-ttu-id="2617b-177">关系</span><span class="sxs-lookup"><span data-stu-id="2617b-177">Relationships</span></span>

<span data-ttu-id="2617b-178">无</span><span class="sxs-lookup"><span data-stu-id="2617b-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2617b-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2617b-179">JSON representation</span></span>

<span data-ttu-id="2617b-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2617b-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "baseType": "",
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