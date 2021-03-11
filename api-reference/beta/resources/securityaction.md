---
title: securityAction 资源类型
description: 利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。 当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。 针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。 请通过 Windows Defender ATP（即将推出）尝试安全操作，以使用在警报中看到或在调查期间确定的属性来阻止 Windows 终结点上的恶意活动。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c1adeb6ee5ab3b3ad2165e854b2812e39b8df5ab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720625"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="b207e-106">securityAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b207e-106">securityAction resource type</span></span>

<span data-ttu-id="b207e-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b207e-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b207e-108">利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。</span><span class="sxs-lookup"><span data-stu-id="b207e-108">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="b207e-109">当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。</span><span class="sxs-lookup"><span data-stu-id="b207e-109">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="b207e-110">针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。</span><span class="sxs-lookup"><span data-stu-id="b207e-110">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="b207e-111">请通过 [Windows Defender ATP](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) 尝试安全操作，以使用在警报中看到或在调查期间确定的属性来阻止 Windows 终结点上的恶意活动。</span><span class="sxs-lookup"><span data-stu-id="b207e-111">Try security actions with [Windows Defender ATP](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="b207e-112">**注意：** 安全操作当前仅支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="b207e-112">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="b207e-113">方法</span><span class="sxs-lookup"><span data-stu-id="b207e-113">Methods</span></span>

| <span data-ttu-id="b207e-114">方法</span><span class="sxs-lookup"><span data-stu-id="b207e-114">Method</span></span>       | <span data-ttu-id="b207e-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="b207e-115">Return Type</span></span> | <span data-ttu-id="b207e-116">说明</span><span class="sxs-lookup"><span data-stu-id="b207e-116">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b207e-117">获取安全操作</span><span class="sxs-lookup"><span data-stu-id="b207e-117">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="b207e-118">securityAction</span><span class="sxs-lookup"><span data-stu-id="b207e-118">securityAction</span></span>](securityaction.md) | <span data-ttu-id="b207e-119">读取 securityAction 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b207e-119">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="b207e-120">创建安全操作</span><span class="sxs-lookup"><span data-stu-id="b207e-120">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="b207e-121">securityAction</span><span class="sxs-lookup"><span data-stu-id="b207e-121">securityAction</span></span>](securityaction.md) | <span data-ttu-id="b207e-122">通过发布到 securityActions 集合创建新的 securityAction。</span><span class="sxs-lookup"><span data-stu-id="b207e-122">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="b207e-123">列出安全操作</span><span class="sxs-lookup"><span data-stu-id="b207e-123">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="b207e-124">[securityAction](securityaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b207e-124">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="b207e-125">获取 securityAction 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b207e-125">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="b207e-126">取消安全操作</span><span class="sxs-lookup"><span data-stu-id="b207e-126">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="b207e-127">无</span><span class="sxs-lookup"><span data-stu-id="b207e-127">None</span></span>|<span data-ttu-id="b207e-128">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="b207e-128">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="b207e-129">属性</span><span class="sxs-lookup"><span data-stu-id="b207e-129">Properties</span></span>

| <span data-ttu-id="b207e-130">属性</span><span class="sxs-lookup"><span data-stu-id="b207e-130">Property</span></span>     | <span data-ttu-id="b207e-131">类型</span><span class="sxs-lookup"><span data-stu-id="b207e-131">Type</span></span>        | <span data-ttu-id="b207e-132">说明</span><span class="sxs-lookup"><span data-stu-id="b207e-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b207e-133">actionReason</span><span class="sxs-lookup"><span data-stu-id="b207e-133">actionReason</span></span>|<span data-ttu-id="b207e-134">String</span><span class="sxs-lookup"><span data-stu-id="b207e-134">String</span></span>|<span data-ttu-id="b207e-135">调用此操作的原因。</span><span class="sxs-lookup"><span data-stu-id="b207e-135">Reason for invoking this action.</span></span>|
|<span data-ttu-id="b207e-136">appId</span><span class="sxs-lookup"><span data-stu-id="b207e-136">appId</span></span>|<span data-ttu-id="b207e-137">String</span><span class="sxs-lookup"><span data-stu-id="b207e-137">String</span></span>|<span data-ttu-id="b207e-138">在 POST 中提交的调用应用程序 (ID) 操作。</span><span class="sxs-lookup"><span data-stu-id="b207e-138">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="b207e-139">appId 应从身份验证令牌中提取，调用应用程序不应手动输入。</span><span class="sxs-lookup"><span data-stu-id="b207e-139">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b207e-140">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="b207e-140">azureTenantId</span></span>|<span data-ttu-id="b207e-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b207e-141">String</span></span>|<span data-ttu-id="b207e-142">实体的 Azure 租户 ID，用于确定实体属于 (租户支持) 。</span><span class="sxs-lookup"><span data-stu-id="b207e-142">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="b207e-143">azureTenantId 应从身份验证令牌中提取，调用应用程序不应手动输入。</span><span class="sxs-lookup"><span data-stu-id="b207e-143">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b207e-144">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b207e-144">completedDateTime</span></span>|<span data-ttu-id="b207e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b207e-145">DateTimeOffset</span></span>|<span data-ttu-id="b207e-146">操作完成时时间戳。</span><span class="sxs-lookup"><span data-stu-id="b207e-146">Timestamp when the action was completed.</span></span> <span data-ttu-id="b207e-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b207e-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b207e-148">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b207e-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b207e-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b207e-149">createdDateTime</span></span>|<span data-ttu-id="b207e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b207e-150">DateTimeOffset</span></span>|<span data-ttu-id="b207e-151">创建操作时时间戳。</span><span class="sxs-lookup"><span data-stu-id="b207e-151">Timestamp when the action is created.</span></span> <span data-ttu-id="b207e-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b207e-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b207e-153">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b207e-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b207e-154">errorInfo</span><span class="sxs-lookup"><span data-stu-id="b207e-154">errorInfo</span></span>|[<span data-ttu-id="b207e-155">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b207e-155">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="b207e-156">操作失败时的错误信息。</span><span class="sxs-lookup"><span data-stu-id="b207e-156">Error info when the action fails.</span></span>|
|<span data-ttu-id="b207e-157">id</span><span class="sxs-lookup"><span data-stu-id="b207e-157">id</span></span>|<span data-ttu-id="b207e-158">String</span><span class="sxs-lookup"><span data-stu-id="b207e-158">String</span></span>| <span data-ttu-id="b207e-159">在操作被启用时由系统创建。</span><span class="sxs-lookup"><span data-stu-id="b207e-159">Created by the system when the action is ingested.</span></span> <span data-ttu-id="b207e-160">生成的 GUID/唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b207e-160">Generated GUID/unique identifier.</span></span> <span data-ttu-id="b207e-161">只读。</span><span class="sxs-lookup"><span data-stu-id="b207e-161">Read-only.</span></span>|
|<span data-ttu-id="b207e-162">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b207e-162">lastActionDateTime</span></span>|<span data-ttu-id="b207e-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b207e-163">DateTimeOffset</span></span>| <span data-ttu-id="b207e-164">上次更新此操作的时间戳。</span><span class="sxs-lookup"><span data-stu-id="b207e-164">Timestamp when this action was last updated.</span></span> <span data-ttu-id="b207e-165">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b207e-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b207e-166">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b207e-166">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b207e-167">name</span><span class="sxs-lookup"><span data-stu-id="b207e-167">name</span></span>|<span data-ttu-id="b207e-168">String</span><span class="sxs-lookup"><span data-stu-id="b207e-168">String</span></span>| <span data-ttu-id="b207e-169">操作名称。</span><span class="sxs-lookup"><span data-stu-id="b207e-169">Action name.</span></span>|
|<span data-ttu-id="b207e-170">parameters</span><span class="sxs-lookup"><span data-stu-id="b207e-170">parameters</span></span>|<span data-ttu-id="b207e-171">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b207e-171">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="b207e-172">参数集合 (键值对) 操作所必需的，例如要阻止的 URL 或 fileHash 等) 。</span><span class="sxs-lookup"><span data-stu-id="b207e-172">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="b207e-173">**必需**</span><span class="sxs-lookup"><span data-stu-id="b207e-173">**Required**</span></span>|
|<span data-ttu-id="b207e-174">状态</span><span class="sxs-lookup"><span data-stu-id="b207e-174">states</span></span>|<span data-ttu-id="b207e-175">[securityActionState](securityactionstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b207e-175">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="b207e-176">securityActionState 集合，以保留操作历史记录。</span><span class="sxs-lookup"><span data-stu-id="b207e-176">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="b207e-177">状态</span><span class="sxs-lookup"><span data-stu-id="b207e-177">status</span></span>|<span data-ttu-id="b207e-178">string</span><span class="sxs-lookup"><span data-stu-id="b207e-178">string</span></span>| <span data-ttu-id="b207e-179">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b207e-179">Status of the action.</span></span> <span data-ttu-id="b207e-180">可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。</span><span class="sxs-lookup"><span data-stu-id="b207e-180">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="b207e-181">user</span><span class="sxs-lookup"><span data-stu-id="b207e-181">user</span></span>|<span data-ttu-id="b207e-182">String</span><span class="sxs-lookup"><span data-stu-id="b207e-182">String</span></span>| <span data-ttu-id="b207e-183">在 POST 中提交的已登录用户的用户主体 () 操作。</span><span class="sxs-lookup"><span data-stu-id="b207e-183">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="b207e-184">用户应从身份验证令牌中提取，而不是由调用应用程序手动输入。</span><span class="sxs-lookup"><span data-stu-id="b207e-184">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="b207e-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="b207e-185">vendorInformation</span></span>|[<span data-ttu-id="b207e-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b207e-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="b207e-187">复杂类型，包含有关安全产品/服务供应商、提供程序和子 (的详细信息，例如 vendor=Microsoft;provider=Windows Defender ATP;sub-provider=AppLocker) 。</span><span class="sxs-lookup"><span data-stu-id="b207e-187">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b207e-188">关系</span><span class="sxs-lookup"><span data-stu-id="b207e-188">Relationships</span></span>

<span data-ttu-id="b207e-189">无</span><span class="sxs-lookup"><span data-stu-id="b207e-189">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b207e-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b207e-190">JSON representation</span></span>

<span data-ttu-id="b207e-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b207e-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
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