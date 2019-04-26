---
title: securityAction 资源类型
description: 利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。 当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。 针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。 请通过 Windows Defender ATP（即将推出）尝试安全操作，以使用在警报中看到或在调查期间确定的属性来阻止 Windows 终结点上的恶意活动。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5aa99119f23baa4cd9450d48ee4955d7ce91f60d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343365"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="fea39-106">securityAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fea39-106">securityAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea39-107">利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。</span><span class="sxs-lookup"><span data-stu-id="fea39-107">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="fea39-108">当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。</span><span class="sxs-lookup"><span data-stu-id="fea39-108">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="fea39-109">针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。</span><span class="sxs-lookup"><span data-stu-id="fea39-109">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="fea39-110">尝试使用[Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)进行安全操作, 以阻止使用警报中显示的属性或调查过程中确定的属性阻止 windows 终结点上的恶意活动。</span><span class="sxs-lookup"><span data-stu-id="fea39-110">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="fea39-111">**注意:** 当前安全操作仅支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="fea39-111">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="fea39-112">方法</span><span class="sxs-lookup"><span data-stu-id="fea39-112">Methods</span></span>

| <span data-ttu-id="fea39-113">方法</span><span class="sxs-lookup"><span data-stu-id="fea39-113">Method</span></span>       | <span data-ttu-id="fea39-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="fea39-114">Return Type</span></span> | <span data-ttu-id="fea39-115">说明</span><span class="sxs-lookup"><span data-stu-id="fea39-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fea39-116">获取安全操作</span><span class="sxs-lookup"><span data-stu-id="fea39-116">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="fea39-117">securityAction</span><span class="sxs-lookup"><span data-stu-id="fea39-117">securityAction</span></span>](securityaction.md) | <span data-ttu-id="fea39-118">读取 securityAction 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fea39-118">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="fea39-119">创建安全操作</span><span class="sxs-lookup"><span data-stu-id="fea39-119">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="fea39-120">securityAction</span><span class="sxs-lookup"><span data-stu-id="fea39-120">securityAction</span></span>](securityaction.md) | <span data-ttu-id="fea39-121">通过发布到 securityActions 集合创建新的 securityAction。</span><span class="sxs-lookup"><span data-stu-id="fea39-121">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="fea39-122">列出安全操作</span><span class="sxs-lookup"><span data-stu-id="fea39-122">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="fea39-123">[securityAction](securityaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="fea39-123">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="fea39-124">获取 securityAction 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fea39-124">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="fea39-125">取消安全操作</span><span class="sxs-lookup"><span data-stu-id="fea39-125">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="fea39-126">无</span><span class="sxs-lookup"><span data-stu-id="fea39-126">None</span></span>|<span data-ttu-id="fea39-127">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="fea39-127">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="fea39-128">属性</span><span class="sxs-lookup"><span data-stu-id="fea39-128">Properties</span></span>

| <span data-ttu-id="fea39-129">属性</span><span class="sxs-lookup"><span data-stu-id="fea39-129">Property</span></span>     | <span data-ttu-id="fea39-130">类型</span><span class="sxs-lookup"><span data-stu-id="fea39-130">Type</span></span>        | <span data-ttu-id="fea39-131">说明</span><span class="sxs-lookup"><span data-stu-id="fea39-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fea39-132">actionReason</span><span class="sxs-lookup"><span data-stu-id="fea39-132">actionReason</span></span>|<span data-ttu-id="fea39-133">String</span><span class="sxs-lookup"><span data-stu-id="fea39-133">String</span></span>|<span data-ttu-id="fea39-134">调用此操作的原因。</span><span class="sxs-lookup"><span data-stu-id="fea39-134">Reason for invoking this action.</span></span>|
|<span data-ttu-id="fea39-135">appId</span><span class="sxs-lookup"><span data-stu-id="fea39-135">appId</span></span>|<span data-ttu-id="fea39-136">String</span><span class="sxs-lookup"><span data-stu-id="fea39-136">String</span></span>|<span data-ttu-id="fea39-137">提交 (POST) 操作的调用应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="fea39-137">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="fea39-138">应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。</span><span class="sxs-lookup"><span data-stu-id="fea39-138">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="fea39-139">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="fea39-139">azureTenantId</span></span>|<span data-ttu-id="fea39-140">String</span><span class="sxs-lookup"><span data-stu-id="fea39-140">String</span></span>|<span data-ttu-id="fea39-141">用于确定实体所属的租户的实体的 Azure 租户 ID (多租户支持)。</span><span class="sxs-lookup"><span data-stu-id="fea39-141">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="fea39-142">应从 auth 令牌中提取 azureTenantId, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="fea39-142">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="fea39-143">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="fea39-143">completedDateTime</span></span>|<span data-ttu-id="fea39-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea39-144">DateTimeOffset</span></span>|<span data-ttu-id="fea39-145">操作完成时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="fea39-145">Timestamp when the action was completed.</span></span> <span data-ttu-id="fea39-146">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="fea39-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fea39-147">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fea39-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fea39-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fea39-148">createdDateTime</span></span>|<span data-ttu-id="fea39-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea39-149">DateTimeOffset</span></span>|<span data-ttu-id="fea39-150">创建操作时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="fea39-150">Timestamp when the action is created.</span></span> <span data-ttu-id="fea39-151">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="fea39-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fea39-152">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fea39-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fea39-153">errorInfo</span><span class="sxs-lookup"><span data-stu-id="fea39-153">errorInfo</span></span>|[<span data-ttu-id="fea39-154">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fea39-154">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="fea39-155">操作失败时的错误消息。</span><span class="sxs-lookup"><span data-stu-id="fea39-155">Error info when the action fails.</span></span>|
|<span data-ttu-id="fea39-156">id</span><span class="sxs-lookup"><span data-stu-id="fea39-156">id</span></span>|<span data-ttu-id="fea39-157">String</span><span class="sxs-lookup"><span data-stu-id="fea39-157">String</span></span>| <span data-ttu-id="fea39-158">当操作为引入时由系统创建。</span><span class="sxs-lookup"><span data-stu-id="fea39-158">Created by the system when the action is ingested.</span></span> <span data-ttu-id="fea39-159">生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fea39-159">Generated GUID/unique identifier.</span></span> <span data-ttu-id="fea39-160">只读。</span><span class="sxs-lookup"><span data-stu-id="fea39-160">Read-only.</span></span>|
|<span data-ttu-id="fea39-161">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="fea39-161">lastActionDateTime</span></span>|<span data-ttu-id="fea39-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea39-162">DateTimeOffset</span></span>| <span data-ttu-id="fea39-163">上次更新此操作时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="fea39-163">Timestamp when this action was last updated.</span></span> <span data-ttu-id="fea39-164">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="fea39-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fea39-165">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fea39-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fea39-166">name</span><span class="sxs-lookup"><span data-stu-id="fea39-166">name</span></span>|<span data-ttu-id="fea39-167">字符串</span><span class="sxs-lookup"><span data-stu-id="fea39-167">String</span></span>| <span data-ttu-id="fea39-168">操作名称。</span><span class="sxs-lookup"><span data-stu-id="fea39-168">Action name.</span></span>|
|<span data-ttu-id="fea39-169">parameters</span><span class="sxs-lookup"><span data-stu-id="fea39-169">parameters</span></span>|<span data-ttu-id="fea39-170">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fea39-170">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="fea39-171">调用操作所必需的参数 (键值对) 集合, 例如 URL 或 fileHash to block 等。</span><span class="sxs-lookup"><span data-stu-id="fea39-171">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="fea39-172">**必需**</span><span class="sxs-lookup"><span data-stu-id="fea39-172">**Required**</span></span>|
|<span data-ttu-id="fea39-173">市</span><span class="sxs-lookup"><span data-stu-id="fea39-173">states</span></span>|<span data-ttu-id="fea39-174">[securityActionState](securityactionstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="fea39-174">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="fea39-175">securityActionState 的集合, 以保留操作的历史记录。</span><span class="sxs-lookup"><span data-stu-id="fea39-175">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="fea39-176">状态</span><span class="sxs-lookup"><span data-stu-id="fea39-176">status</span></span>|<span data-ttu-id="fea39-177">string</span><span class="sxs-lookup"><span data-stu-id="fea39-177">string</span></span>| <span data-ttu-id="fea39-178">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fea39-178">Status of the action.</span></span> <span data-ttu-id="fea39-179">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="fea39-179">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="fea39-180">user</span><span class="sxs-lookup"><span data-stu-id="fea39-180">user</span></span>|<span data-ttu-id="fea39-181">String</span><span class="sxs-lookup"><span data-stu-id="fea39-181">String</span></span>| <span data-ttu-id="fea39-182">已提交 (POST) 操作的已登录用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="fea39-182">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="fea39-183">应从身份验证令牌中提取用户, 而不是通过调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="fea39-183">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="fea39-184">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="fea39-184">vendorInformation</span></span>|[<span data-ttu-id="fea39-185">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="fea39-185">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="fea39-186">包含有关安全产品/服务供应商、提供程序和子提供商的详细信息的复杂类型 (例如, 供应商 = Microsoft; 提供商 = Windows Defender ATP; 子提供程序 = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="fea39-186">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="fea39-187">关系</span><span class="sxs-lookup"><span data-stu-id="fea39-187">Relationships</span></span>

<span data-ttu-id="fea39-188">无</span><span class="sxs-lookup"><span data-stu-id="fea39-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fea39-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fea39-189">JSON representation</span></span>

<span data-ttu-id="fea39-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fea39-190">The following is a JSON representation of the resource.</span></span>

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