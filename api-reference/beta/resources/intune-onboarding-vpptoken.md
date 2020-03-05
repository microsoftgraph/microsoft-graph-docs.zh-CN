---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a27f6d2e630d6e83d600cc555cf625590584a677
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524074"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="ccec9-106">vppToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="ccec9-106">vppToken resource type</span></span>

<span data-ttu-id="ccec9-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ccec9-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccec9-108">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ccec9-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccec9-109">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccec9-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccec9-110">通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。</span><span class="sxs-lookup"><span data-stu-id="ccec9-110">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="ccec9-111">这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。</span><span class="sxs-lookup"><span data-stu-id="ccec9-111">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="ccec9-112">然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。</span><span class="sxs-lookup"><span data-stu-id="ccec9-112">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="ccec9-113">可上传多个 Apple VPP 企业版或教育版令牌。</span><span class="sxs-lookup"><span data-stu-id="ccec9-113">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="ccec9-114">方法</span><span class="sxs-lookup"><span data-stu-id="ccec9-114">Methods</span></span>
|<span data-ttu-id="ccec9-115">方法</span><span class="sxs-lookup"><span data-stu-id="ccec9-115">Method</span></span>|<span data-ttu-id="ccec9-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="ccec9-116">Return Type</span></span>|<span data-ttu-id="ccec9-117">说明</span><span class="sxs-lookup"><span data-stu-id="ccec9-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ccec9-118">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="ccec9-118">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="ccec9-119">[vppToken](../resources/intune-onboarding-vpptoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ccec9-119">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="ccec9-120">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccec9-120">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="ccec9-121">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-121">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="ccec9-122">vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-122">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="ccec9-123">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccec9-123">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="ccec9-124">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-124">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="ccec9-125">vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-125">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="ccec9-126">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ccec9-126">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="ccec9-127">删除 vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-127">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="ccec9-128">无</span><span class="sxs-lookup"><span data-stu-id="ccec9-128">None</span></span>|<span data-ttu-id="ccec9-129">删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="ccec9-129">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="ccec9-130">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-130">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="ccec9-131">vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-131">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="ccec9-132">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ccec9-132">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="ccec9-133">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="ccec9-133">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="ccec9-134">vppToken</span><span class="sxs-lookup"><span data-stu-id="ccec9-134">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="ccec9-135">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="ccec9-135">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="ccec9-136">revokeLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="ccec9-136">revokeLicenses action</span></span>](../api/intune-onboarding-vpptoken-revokelicenses.md)|<span data-ttu-id="ccec9-137">无</span><span class="sxs-lookup"><span data-stu-id="ccec9-137">None</span></span>|<span data-ttu-id="ccec9-138">吊销与特定 appleVolumePurchaseProgramToken 相关联的许可证</span><span class="sxs-lookup"><span data-stu-id="ccec9-138">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="ccec9-139">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="ccec9-139">getLicensesForApp function</span></span>](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|<span data-ttu-id="ccec9-140">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="ccec9-140">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection</span></span>|<span data-ttu-id="ccec9-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ccec9-141">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ccec9-142">属性</span><span class="sxs-lookup"><span data-stu-id="ccec9-142">Properties</span></span>
|<span data-ttu-id="ccec9-143">属性</span><span class="sxs-lookup"><span data-stu-id="ccec9-143">Property</span></span>|<span data-ttu-id="ccec9-144">类型</span><span class="sxs-lookup"><span data-stu-id="ccec9-144">Type</span></span>|<span data-ttu-id="ccec9-145">说明</span><span class="sxs-lookup"><span data-stu-id="ccec9-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccec9-146">id</span><span class="sxs-lookup"><span data-stu-id="ccec9-146">id</span></span>|<span data-ttu-id="ccec9-147">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-147">String</span></span>|<span data-ttu-id="ccec9-148">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="ccec9-148">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="ccec9-149">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="ccec9-149">It is the Key of the entity.</span></span>|
|<span data-ttu-id="ccec9-150">organizationName</span><span class="sxs-lookup"><span data-stu-id="ccec9-150">organizationName</span></span>|<span data-ttu-id="ccec9-151">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-151">String</span></span>|<span data-ttu-id="ccec9-152">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="ccec9-152">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ccec9-153">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ccec9-153">vppTokenAccountType</span></span>|[<span data-ttu-id="ccec9-154">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ccec9-154">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ccec9-155">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="ccec9-155">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ccec9-156">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-156">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ccec9-157">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-157">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ccec9-158">appleId</span><span class="sxs-lookup"><span data-stu-id="ccec9-158">appleId</span></span>|<span data-ttu-id="ccec9-159">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-159">String</span></span>|<span data-ttu-id="ccec9-160">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ccec9-160">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ccec9-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ccec9-161">expirationDateTime</span></span>|<span data-ttu-id="ccec9-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccec9-162">DateTimeOffset</span></span>|<span data-ttu-id="ccec9-163">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="ccec9-163">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ccec9-164">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ccec9-164">lastSyncDateTime</span></span>|<span data-ttu-id="ccec9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccec9-165">DateTimeOffset</span></span>|<span data-ttu-id="ccec9-166">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="ccec9-166">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ccec9-167">token</span><span class="sxs-lookup"><span data-stu-id="ccec9-167">token</span></span>|<span data-ttu-id="ccec9-168">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-168">String</span></span>|<span data-ttu-id="ccec9-169">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="ccec9-169">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ccec9-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccec9-170">lastModifiedDateTime</span></span>|<span data-ttu-id="ccec9-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccec9-171">DateTimeOffset</span></span>|<span data-ttu-id="ccec9-172">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ccec9-172">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ccec9-173">state</span><span class="sxs-lookup"><span data-stu-id="ccec9-173">state</span></span>|[<span data-ttu-id="ccec9-174">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ccec9-174">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="ccec9-175">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="ccec9-175">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ccec9-176">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-176">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="ccec9-177">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-177">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="ccec9-178">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="ccec9-178">tokenActionResults</span></span>|<span data-ttu-id="ccec9-179">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="ccec9-179">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="ccec9-180">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="ccec9-180">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ccec9-181">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ccec9-181">lastSyncStatus</span></span>|[<span data-ttu-id="ccec9-182">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ccec9-182">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="ccec9-183">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="ccec9-183">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ccec9-184">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-184">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="ccec9-185">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ccec9-185">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ccec9-186">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="ccec9-186">automaticallyUpdateApps</span></span>|<span data-ttu-id="ccec9-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccec9-187">Boolean</span></span>|<span data-ttu-id="ccec9-188">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="ccec9-188">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ccec9-189">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ccec9-189">countryOrRegion</span></span>|<span data-ttu-id="ccec9-190">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-190">String</span></span>|<span data-ttu-id="ccec9-191">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="ccec9-191">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ccec9-192">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="ccec9-192">dataSharingConsentGranted</span></span>|<span data-ttu-id="ccec9-193">布尔</span><span class="sxs-lookup"><span data-stu-id="ccec9-193">Boolean</span></span>|<span data-ttu-id="ccec9-194">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="ccec9-194">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ccec9-195">displayName</span><span class="sxs-lookup"><span data-stu-id="ccec9-195">displayName</span></span>|<span data-ttu-id="ccec9-196">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-196">String</span></span>|<span data-ttu-id="ccec9-197">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="ccec9-197">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="ccec9-198">locationName</span><span class="sxs-lookup"><span data-stu-id="ccec9-198">locationName</span></span>|<span data-ttu-id="ccec9-199">String</span><span class="sxs-lookup"><span data-stu-id="ccec9-199">String</span></span>|<span data-ttu-id="ccec9-200">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="ccec9-200">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="ccec9-201">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="ccec9-201">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="ccec9-202">布尔</span><span class="sxs-lookup"><span data-stu-id="ccec9-202">Boolean</span></span>|<span data-ttu-id="ccec9-203">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="ccec9-203">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="ccec9-204">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ccec9-204">roleScopeTagIds</span></span>|<span data-ttu-id="ccec9-205">String 集合</span><span class="sxs-lookup"><span data-stu-id="ccec9-205">String collection</span></span>|<span data-ttu-id="ccec9-206">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="ccec9-206">Role Scope Tags IDs assigned to this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccec9-207">关系</span><span class="sxs-lookup"><span data-stu-id="ccec9-207">Relationships</span></span>
<span data-ttu-id="ccec9-208">无</span><span class="sxs-lookup"><span data-stu-id="ccec9-208">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccec9-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ccec9-209">JSON Representation</span></span>
<span data-ttu-id="ccec9-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccec9-210">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



