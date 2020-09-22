---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9da38e996ddb77f0698b1541e8ea889be3e7ce9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029356"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="462fd-106">vppToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="462fd-106">vppToken resource type</span></span>

<span data-ttu-id="462fd-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="462fd-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="462fd-108">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="462fd-108">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="462fd-109">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="462fd-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="462fd-110">通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。</span><span class="sxs-lookup"><span data-stu-id="462fd-110">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="462fd-111">这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。</span><span class="sxs-lookup"><span data-stu-id="462fd-111">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="462fd-112">然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。</span><span class="sxs-lookup"><span data-stu-id="462fd-112">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="462fd-113">可上传多个 Apple VPP 企业版或教育版令牌。</span><span class="sxs-lookup"><span data-stu-id="462fd-113">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="462fd-114">方法</span><span class="sxs-lookup"><span data-stu-id="462fd-114">Methods</span></span>
|<span data-ttu-id="462fd-115">方法</span><span class="sxs-lookup"><span data-stu-id="462fd-115">Method</span></span>|<span data-ttu-id="462fd-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="462fd-116">Return Type</span></span>|<span data-ttu-id="462fd-117">说明</span><span class="sxs-lookup"><span data-stu-id="462fd-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="462fd-118">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="462fd-118">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="462fd-119">[vppToken](../resources/intune-onboarding-vpptoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="462fd-119">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="462fd-120">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="462fd-120">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="462fd-121">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-121">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="462fd-122">vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-122">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="462fd-123">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="462fd-123">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="462fd-124">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-124">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="462fd-125">vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-125">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="462fd-126">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="462fd-126">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="462fd-127">删除 vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-127">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="462fd-128">无</span><span class="sxs-lookup"><span data-stu-id="462fd-128">None</span></span>|<span data-ttu-id="462fd-129">删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="462fd-129">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="462fd-130">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-130">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="462fd-131">vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-131">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="462fd-132">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="462fd-132">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="462fd-133">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="462fd-133">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="462fd-134">vppToken</span><span class="sxs-lookup"><span data-stu-id="462fd-134">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="462fd-135">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="462fd-135">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="462fd-136">revokeLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="462fd-136">revokeLicenses action</span></span>](../api/intune-onboarding-vpptoken-revokelicenses.md)|<span data-ttu-id="462fd-137">无</span><span class="sxs-lookup"><span data-stu-id="462fd-137">None</span></span>|<span data-ttu-id="462fd-138">吊销与特定 appleVolumePurchaseProgramToken 相关联的许可证</span><span class="sxs-lookup"><span data-stu-id="462fd-138">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="462fd-139">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="462fd-139">getLicensesForApp function</span></span>](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|<span data-ttu-id="462fd-140">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="462fd-140">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection</span></span>|<span data-ttu-id="462fd-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="462fd-141">Not yet documented</span></span>|
|[<span data-ttu-id="462fd-142">syncLicenseCounts 操作</span><span class="sxs-lookup"><span data-stu-id="462fd-142">syncLicenseCounts action</span></span>](../api/intune-onboarding-vpptoken-synclicensecounts.md)|<span data-ttu-id="462fd-143">无</span><span class="sxs-lookup"><span data-stu-id="462fd-143">None</span></span>|<span data-ttu-id="462fd-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="462fd-144">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="462fd-145">属性</span><span class="sxs-lookup"><span data-stu-id="462fd-145">Properties</span></span>
|<span data-ttu-id="462fd-146">属性</span><span class="sxs-lookup"><span data-stu-id="462fd-146">Property</span></span>|<span data-ttu-id="462fd-147">类型</span><span class="sxs-lookup"><span data-stu-id="462fd-147">Type</span></span>|<span data-ttu-id="462fd-148">说明</span><span class="sxs-lookup"><span data-stu-id="462fd-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="462fd-149">id</span><span class="sxs-lookup"><span data-stu-id="462fd-149">id</span></span>|<span data-ttu-id="462fd-150">String</span><span class="sxs-lookup"><span data-stu-id="462fd-150">String</span></span>|<span data-ttu-id="462fd-151">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="462fd-151">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="462fd-152">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="462fd-152">It is the Key of the entity.</span></span>|
|<span data-ttu-id="462fd-153">organizationName</span><span class="sxs-lookup"><span data-stu-id="462fd-153">organizationName</span></span>|<span data-ttu-id="462fd-154">String</span><span class="sxs-lookup"><span data-stu-id="462fd-154">String</span></span>|<span data-ttu-id="462fd-155">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="462fd-155">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="462fd-156">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="462fd-156">vppTokenAccountType</span></span>|[<span data-ttu-id="462fd-157">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="462fd-157">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="462fd-158">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="462fd-158">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="462fd-159">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="462fd-159">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="462fd-160">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="462fd-160">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="462fd-161">appleId</span><span class="sxs-lookup"><span data-stu-id="462fd-161">appleId</span></span>|<span data-ttu-id="462fd-162">String</span><span class="sxs-lookup"><span data-stu-id="462fd-162">String</span></span>|<span data-ttu-id="462fd-163">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="462fd-163">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="462fd-164">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="462fd-164">expirationDateTime</span></span>|<span data-ttu-id="462fd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462fd-165">DateTimeOffset</span></span>|<span data-ttu-id="462fd-166">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="462fd-166">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="462fd-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="462fd-167">lastSyncDateTime</span></span>|<span data-ttu-id="462fd-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462fd-168">DateTimeOffset</span></span>|<span data-ttu-id="462fd-169">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="462fd-169">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="462fd-170">token</span><span class="sxs-lookup"><span data-stu-id="462fd-170">token</span></span>|<span data-ttu-id="462fd-171">String</span><span class="sxs-lookup"><span data-stu-id="462fd-171">String</span></span>|<span data-ttu-id="462fd-172">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="462fd-172">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="462fd-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="462fd-173">lastModifiedDateTime</span></span>|<span data-ttu-id="462fd-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="462fd-174">DateTimeOffset</span></span>|<span data-ttu-id="462fd-175">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="462fd-175">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="462fd-176">state</span><span class="sxs-lookup"><span data-stu-id="462fd-176">state</span></span>|[<span data-ttu-id="462fd-177">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="462fd-177">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="462fd-178">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="462fd-178">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="462fd-179">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="462fd-179">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="462fd-180">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`、`duplicateLocationId`。</span><span class="sxs-lookup"><span data-stu-id="462fd-180">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.</span></span>|
|<span data-ttu-id="462fd-181">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="462fd-181">tokenActionResults</span></span>|<span data-ttu-id="462fd-182">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="462fd-182">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="462fd-183">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="462fd-183">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="462fd-184">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="462fd-184">lastSyncStatus</span></span>|[<span data-ttu-id="462fd-185">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="462fd-185">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="462fd-186">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="462fd-186">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="462fd-187">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="462fd-187">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="462fd-188">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="462fd-188">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="462fd-189">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="462fd-189">automaticallyUpdateApps</span></span>|<span data-ttu-id="462fd-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="462fd-190">Boolean</span></span>|<span data-ttu-id="462fd-191">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="462fd-191">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="462fd-192">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="462fd-192">countryOrRegion</span></span>|<span data-ttu-id="462fd-193">String</span><span class="sxs-lookup"><span data-stu-id="462fd-193">String</span></span>|<span data-ttu-id="462fd-194">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="462fd-194">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="462fd-195">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="462fd-195">dataSharingConsentGranted</span></span>|<span data-ttu-id="462fd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="462fd-196">Boolean</span></span>|<span data-ttu-id="462fd-197">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="462fd-197">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="462fd-198">displayName</span><span class="sxs-lookup"><span data-stu-id="462fd-198">displayName</span></span>|<span data-ttu-id="462fd-199">String</span><span class="sxs-lookup"><span data-stu-id="462fd-199">String</span></span>|<span data-ttu-id="462fd-200">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="462fd-200">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="462fd-201">locationName</span><span class="sxs-lookup"><span data-stu-id="462fd-201">locationName</span></span>|<span data-ttu-id="462fd-202">String</span><span class="sxs-lookup"><span data-stu-id="462fd-202">String</span></span>|<span data-ttu-id="462fd-203">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="462fd-203">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="462fd-204">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="462fd-204">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="462fd-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="462fd-205">Boolean</span></span>|<span data-ttu-id="462fd-206">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="462fd-206">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="462fd-207">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="462fd-207">roleScopeTagIds</span></span>|<span data-ttu-id="462fd-208">String 集合</span><span class="sxs-lookup"><span data-stu-id="462fd-208">String collection</span></span>|<span data-ttu-id="462fd-209">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="462fd-209">Role Scope Tags IDs assigned to this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="462fd-210">关系</span><span class="sxs-lookup"><span data-stu-id="462fd-210">Relationships</span></span>
<span data-ttu-id="462fd-211">无</span><span class="sxs-lookup"><span data-stu-id="462fd-211">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="462fd-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="462fd-212">JSON Representation</span></span>
<span data-ttu-id="462fd-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="462fd-213">Here is a JSON representation of the resource.</span></span>
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






