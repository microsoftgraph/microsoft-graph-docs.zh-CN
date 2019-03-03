---
title: securityAction 资源类型
description: 立即采取行动以使用 Microsoft Graph Security securityAction 实体防御威胁。 当安全分析员发现新的指标 (如恶意文件、URL、域或 IP 地址) 时, 可以立即在 Microsoft 安全解决方案中启用保护。 调用特定提供程序的操作, 请参阅执行的所有操作, 并在需要时取消操作。 尝试使用 Windows Defender ATP 进行安全操作 (即将推出), 以阻止在调查过程中发现警报或标识的属性的 windows 终结点上的恶意活动。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366985"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="72e99-106">securityAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="72e99-106">securityAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e99-107">立即采取行动以使用 Microsoft Graph Security securityAction 实体防御威胁。</span><span class="sxs-lookup"><span data-stu-id="72e99-107">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="72e99-108">当安全分析员发现新的指标 (如恶意文件、URL、域或 IP 地址) 时, 可以立即在 Microsoft 安全解决方案中启用保护。</span><span class="sxs-lookup"><span data-stu-id="72e99-108">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="72e99-109">调用特定提供程序的操作, 请参阅执行的所有操作, 并在需要时取消操作。</span><span class="sxs-lookup"><span data-stu-id="72e99-109">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="72e99-110">尝试使用[Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)进行安全操作 (即将推出), 以阻止在调查过程中发现警报或标识的属性的 windows 终结点上的恶意活动。</span><span class="sxs-lookup"><span data-stu-id="72e99-110">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (coming soon) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

## <a name="methods"></a><span data-ttu-id="72e99-111">方法</span><span class="sxs-lookup"><span data-stu-id="72e99-111">Methods</span></span>

| <span data-ttu-id="72e99-112">方法</span><span class="sxs-lookup"><span data-stu-id="72e99-112">Method</span></span>       | <span data-ttu-id="72e99-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="72e99-113">Return Type</span></span> | <span data-ttu-id="72e99-114">说明</span><span class="sxs-lookup"><span data-stu-id="72e99-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="72e99-115">获取 securityAction</span><span class="sxs-lookup"><span data-stu-id="72e99-115">Get securityAction</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="72e99-116">securityAction</span><span class="sxs-lookup"><span data-stu-id="72e99-116">securityAction</span></span>](securityaction.md) | <span data-ttu-id="72e99-117">读取 securityAction 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72e99-117">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="72e99-118">创建 securityAction</span><span class="sxs-lookup"><span data-stu-id="72e99-118">Create securityAction</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="72e99-119">securityAction</span><span class="sxs-lookup"><span data-stu-id="72e99-119">securityAction</span></span>](securityaction.md) | <span data-ttu-id="72e99-120">通过发布到 securityActions 集合创建新的 securityAction。</span><span class="sxs-lookup"><span data-stu-id="72e99-120">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="72e99-121">列出 securityActions</span><span class="sxs-lookup"><span data-stu-id="72e99-121">List securityActions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="72e99-122">[securityAction](securityaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="72e99-122">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="72e99-123">获取 securityAction 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72e99-123">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="72e99-124">取消 securityAction</span><span class="sxs-lookup"><span data-stu-id="72e99-124">Cancel securityAction</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="72e99-125">无</span><span class="sxs-lookup"><span data-stu-id="72e99-125">None</span></span>|<span data-ttu-id="72e99-126">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="72e99-126">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="72e99-127">属性</span><span class="sxs-lookup"><span data-stu-id="72e99-127">Properties</span></span>

| <span data-ttu-id="72e99-128">属性</span><span class="sxs-lookup"><span data-stu-id="72e99-128">Property</span></span>     | <span data-ttu-id="72e99-129">类型</span><span class="sxs-lookup"><span data-stu-id="72e99-129">Type</span></span>        | <span data-ttu-id="72e99-130">说明</span><span class="sxs-lookup"><span data-stu-id="72e99-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="72e99-131">actionReason</span><span class="sxs-lookup"><span data-stu-id="72e99-131">actionReason</span></span>|<span data-ttu-id="72e99-132">String</span><span class="sxs-lookup"><span data-stu-id="72e99-132">String</span></span>|<span data-ttu-id="72e99-133">调用此操作的原因。</span><span class="sxs-lookup"><span data-stu-id="72e99-133">Reason for invoking this action.</span></span>|
|<span data-ttu-id="72e99-134">appId</span><span class="sxs-lookup"><span data-stu-id="72e99-134">appId</span></span>|<span data-ttu-id="72e99-135">String</span><span class="sxs-lookup"><span data-stu-id="72e99-135">String</span></span>|<span data-ttu-id="72e99-136">提交 (POST) 操作的调用应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="72e99-136">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="72e99-137">应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。</span><span class="sxs-lookup"><span data-stu-id="72e99-137">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="72e99-138">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="72e99-138">azureTenantId</span></span>|<span data-ttu-id="72e99-139">String</span><span class="sxs-lookup"><span data-stu-id="72e99-139">String</span></span>|<span data-ttu-id="72e99-140">用于确定实体所属的租户的实体的 Azure 租户 ID (多租户支持)。</span><span class="sxs-lookup"><span data-stu-id="72e99-140">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="72e99-141">应从 auth 令牌中提取 azureTenantId, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="72e99-141">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="72e99-142">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="72e99-142">completedDateTime</span></span>|<span data-ttu-id="72e99-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72e99-143">DateTimeOffset</span></span>|<span data-ttu-id="72e99-144">操作完成时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="72e99-144">Timestamp when the action was completed.</span></span> <span data-ttu-id="72e99-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="72e99-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72e99-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72e99-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72e99-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72e99-147">createdDateTime</span></span>|<span data-ttu-id="72e99-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72e99-148">DateTimeOffset</span></span>|<span data-ttu-id="72e99-149">创建操作时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="72e99-149">Timestamp when the action is created.</span></span> <span data-ttu-id="72e99-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="72e99-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72e99-151">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72e99-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72e99-152">errorInfo</span><span class="sxs-lookup"><span data-stu-id="72e99-152">errorInfo</span></span>|[<span data-ttu-id="72e99-153">resultInfo</span><span class="sxs-lookup"><span data-stu-id="72e99-153">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="72e99-154">操作失败时的错误消息。</span><span class="sxs-lookup"><span data-stu-id="72e99-154">Error info when the action fails.</span></span>|
|<span data-ttu-id="72e99-155">id</span><span class="sxs-lookup"><span data-stu-id="72e99-155">id</span></span>|<span data-ttu-id="72e99-156">字符串</span><span class="sxs-lookup"><span data-stu-id="72e99-156">String</span></span>| <span data-ttu-id="72e99-157">当操作为引入时由系统创建。</span><span class="sxs-lookup"><span data-stu-id="72e99-157">Created by the system when the action is ingested.</span></span> <span data-ttu-id="72e99-158">生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="72e99-158">Generated GUID/unique identifier.</span></span> <span data-ttu-id="72e99-159">只读。</span><span class="sxs-lookup"><span data-stu-id="72e99-159">Read-only.</span></span>|
|<span data-ttu-id="72e99-160">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="72e99-160">lastActionDateTime</span></span>|<span data-ttu-id="72e99-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72e99-161">DateTimeOffset</span></span>| <span data-ttu-id="72e99-162">上次更新此操作时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="72e99-162">Timestamp when this action was last updated.</span></span> <span data-ttu-id="72e99-163">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="72e99-163">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72e99-164">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72e99-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72e99-165">name</span><span class="sxs-lookup"><span data-stu-id="72e99-165">name</span></span>|<span data-ttu-id="72e99-166">String</span><span class="sxs-lookup"><span data-stu-id="72e99-166">String</span></span>| <span data-ttu-id="72e99-167">操作名称。</span><span class="sxs-lookup"><span data-stu-id="72e99-167">Action name.</span></span>|
|<span data-ttu-id="72e99-168">参数</span><span class="sxs-lookup"><span data-stu-id="72e99-168">parameters</span></span>|<span data-ttu-id="72e99-169">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72e99-169">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="72e99-170">调用操作所必需的参数 (键值对) 集合, 例如 URL 或 fileHash to block 等。</span><span class="sxs-lookup"><span data-stu-id="72e99-170">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="72e99-171">**Required**</span><span class="sxs-lookup"><span data-stu-id="72e99-171">**Required**</span></span>|
|<span data-ttu-id="72e99-172">市</span><span class="sxs-lookup"><span data-stu-id="72e99-172">states</span></span>|<span data-ttu-id="72e99-173">[securityActionState](securityactionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="72e99-173">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="72e99-174">securityActionState 的集合, 以保留操作的历史记录。</span><span class="sxs-lookup"><span data-stu-id="72e99-174">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="72e99-175">status</span><span class="sxs-lookup"><span data-stu-id="72e99-175">status</span></span>|<span data-ttu-id="72e99-176">string</span><span class="sxs-lookup"><span data-stu-id="72e99-176">string</span></span>| <span data-ttu-id="72e99-177">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="72e99-177">Status of the action.</span></span> <span data-ttu-id="72e99-178">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="72e99-178">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="72e99-179">user</span><span class="sxs-lookup"><span data-stu-id="72e99-179">user</span></span>|<span data-ttu-id="72e99-180">String</span><span class="sxs-lookup"><span data-stu-id="72e99-180">String</span></span>| <span data-ttu-id="72e99-181">已提交 (POST) 操作的已登录用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="72e99-181">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="72e99-182">应从身份验证令牌中提取用户, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="72e99-182">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="72e99-183">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="72e99-183">vendorInformation</span></span>|[<span data-ttu-id="72e99-184">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="72e99-184">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="72e99-185">包含有关安全产品/服务供应商、提供程序和子提供商的详细信息的复杂类型 (例如, 供应商 = Microsoft; 提供商 = Windows Defender ATP; 子提供程序 = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="72e99-185">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="72e99-186">关系</span><span class="sxs-lookup"><span data-stu-id="72e99-186">Relationships</span></span>

<span data-ttu-id="72e99-187">无</span><span class="sxs-lookup"><span data-stu-id="72e99-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72e99-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72e99-188">JSON representation</span></span>

<span data-ttu-id="72e99-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72e99-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->