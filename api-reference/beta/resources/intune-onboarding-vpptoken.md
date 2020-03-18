---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2cdb7ff14984243c5e8b6317e4f0f3c05b12b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777845"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="bb8c7-106">vppToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb8c7-106">vppToken resource type</span></span>

> <span data-ttu-id="bb8c7-107">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb8c7-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb8c7-109">通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-109">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="bb8c7-110">这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-110">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="bb8c7-111">然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-111">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="bb8c7-112">可上传多个 Apple VPP 企业版或教育版令牌。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-112">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="bb8c7-113">方法</span><span class="sxs-lookup"><span data-stu-id="bb8c7-113">Methods</span></span>
|<span data-ttu-id="bb8c7-114">方法</span><span class="sxs-lookup"><span data-stu-id="bb8c7-114">Method</span></span>|<span data-ttu-id="bb8c7-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb8c7-115">Return Type</span></span>|<span data-ttu-id="bb8c7-116">说明</span><span class="sxs-lookup"><span data-stu-id="bb8c7-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb8c7-117">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="bb8c7-117">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="bb8c7-118">[vppToken](../resources/intune-onboarding-vpptoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb8c7-118">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="bb8c7-119">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-119">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="bb8c7-120">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-120">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="bb8c7-121">vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-121">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="bb8c7-122">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-122">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="bb8c7-123">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-123">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="bb8c7-124">vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-124">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="bb8c7-125">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-125">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="bb8c7-126">删除 vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-126">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="bb8c7-127">无</span><span class="sxs-lookup"><span data-stu-id="bb8c7-127">None</span></span>|<span data-ttu-id="bb8c7-128">删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-128">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="bb8c7-129">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-129">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="bb8c7-130">vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-130">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="bb8c7-131">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-131">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="bb8c7-132">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="bb8c7-132">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="bb8c7-133">vppToken</span><span class="sxs-lookup"><span data-stu-id="bb8c7-133">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="bb8c7-134">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="bb8c7-134">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="bb8c7-135">revokeLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="bb8c7-135">revokeLicenses action</span></span>](../api/intune-onboarding-vpptoken-revokelicenses.md)|<span data-ttu-id="bb8c7-136">None</span><span class="sxs-lookup"><span data-stu-id="bb8c7-136">None</span></span>|<span data-ttu-id="bb8c7-137">吊销与特定 appleVolumePurchaseProgramToken 相关联的许可证</span><span class="sxs-lookup"><span data-stu-id="bb8c7-137">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="bb8c7-138">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="bb8c7-138">getLicensesForApp function</span></span>](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|<span data-ttu-id="bb8c7-139">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb8c7-139">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection</span></span>|<span data-ttu-id="bb8c7-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bb8c7-140">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bb8c7-141">属性</span><span class="sxs-lookup"><span data-stu-id="bb8c7-141">Properties</span></span>
|<span data-ttu-id="bb8c7-142">属性</span><span class="sxs-lookup"><span data-stu-id="bb8c7-142">Property</span></span>|<span data-ttu-id="bb8c7-143">类型</span><span class="sxs-lookup"><span data-stu-id="bb8c7-143">Type</span></span>|<span data-ttu-id="bb8c7-144">说明</span><span class="sxs-lookup"><span data-stu-id="bb8c7-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb8c7-145">id</span><span class="sxs-lookup"><span data-stu-id="bb8c7-145">id</span></span>|<span data-ttu-id="bb8c7-146">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-146">String</span></span>|<span data-ttu-id="bb8c7-147">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-147">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="bb8c7-148">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-148">It is the Key of the entity.</span></span>|
|<span data-ttu-id="bb8c7-149">organizationName</span><span class="sxs-lookup"><span data-stu-id="bb8c7-149">organizationName</span></span>|<span data-ttu-id="bb8c7-150">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-150">String</span></span>|<span data-ttu-id="bb8c7-151">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="bb8c7-151">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="bb8c7-152">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="bb8c7-152">vppTokenAccountType</span></span>|[<span data-ttu-id="bb8c7-153">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="bb8c7-153">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="bb8c7-154">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-154">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="bb8c7-155">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-155">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="bb8c7-156">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-156">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="bb8c7-157">appleId</span><span class="sxs-lookup"><span data-stu-id="bb8c7-157">appleId</span></span>|<span data-ttu-id="bb8c7-158">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-158">String</span></span>|<span data-ttu-id="bb8c7-159">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-159">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="bb8c7-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c7-160">expirationDateTime</span></span>|<span data-ttu-id="bb8c7-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb8c7-161">DateTimeOffset</span></span>|<span data-ttu-id="bb8c7-162">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-162">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="bb8c7-163">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c7-163">lastSyncDateTime</span></span>|<span data-ttu-id="bb8c7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb8c7-164">DateTimeOffset</span></span>|<span data-ttu-id="bb8c7-165">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-165">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="bb8c7-166">token</span><span class="sxs-lookup"><span data-stu-id="bb8c7-166">token</span></span>|<span data-ttu-id="bb8c7-167">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-167">String</span></span>|<span data-ttu-id="bb8c7-168">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-168">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="bb8c7-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c7-169">lastModifiedDateTime</span></span>|<span data-ttu-id="bb8c7-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb8c7-170">DateTimeOffset</span></span>|<span data-ttu-id="bb8c7-171">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-171">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="bb8c7-172">state</span><span class="sxs-lookup"><span data-stu-id="bb8c7-172">state</span></span>|[<span data-ttu-id="bb8c7-173">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="bb8c7-173">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="bb8c7-174">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-174">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="bb8c7-175">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-175">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="bb8c7-176">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-176">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="bb8c7-177">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="bb8c7-177">tokenActionResults</span></span>|<span data-ttu-id="bb8c7-178">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb8c7-178">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="bb8c7-179">在 Apple Volume Purchase Program 令牌上执行的操作的状态的集合。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-179">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="bb8c7-180">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="bb8c7-180">lastSyncStatus</span></span>|[<span data-ttu-id="bb8c7-181">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="bb8c7-181">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="bb8c7-182">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-182">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="bb8c7-183">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-183">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="bb8c7-184">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-184">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="bb8c7-185">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="bb8c7-185">automaticallyUpdateApps</span></span>|<span data-ttu-id="bb8c7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb8c7-186">Boolean</span></span>|<span data-ttu-id="bb8c7-187">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-187">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="bb8c7-188">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="bb8c7-188">countryOrRegion</span></span>|<span data-ttu-id="bb8c7-189">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-189">String</span></span>|<span data-ttu-id="bb8c7-190">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-190">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="bb8c7-191">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="bb8c7-191">dataSharingConsentGranted</span></span>|<span data-ttu-id="bb8c7-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="bb8c7-192">Boolean</span></span>|<span data-ttu-id="bb8c7-193">同意授予与 Apple Volume Purchase Program 的数据共享。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-193">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="bb8c7-194">displayName</span><span class="sxs-lookup"><span data-stu-id="bb8c7-194">displayName</span></span>|<span data-ttu-id="bb8c7-195">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-195">String</span></span>|<span data-ttu-id="bb8c7-196">管理员指定的令牌友好名称。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-196">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="bb8c7-197">locationName</span><span class="sxs-lookup"><span data-stu-id="bb8c7-197">locationName</span></span>|<span data-ttu-id="bb8c7-198">String</span><span class="sxs-lookup"><span data-stu-id="bb8c7-198">String</span></span>|<span data-ttu-id="bb8c7-199">从 Apple VPP 返回的令牌位置。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-199">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="bb8c7-200">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="bb8c7-200">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="bb8c7-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="bb8c7-201">Boolean</span></span>|<span data-ttu-id="bb8c7-202">管理员同意允许来自外部 MDM 的声明令牌管理。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-202">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="bb8c7-203">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb8c7-203">roleScopeTagIds</span></span>|<span data-ttu-id="bb8c7-204">String collection</span><span class="sxs-lookup"><span data-stu-id="bb8c7-204">String collection</span></span>|<span data-ttu-id="bb8c7-205">分配给此实体的角色范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-205">Role Scope Tags IDs assigned to this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb8c7-206">关系</span><span class="sxs-lookup"><span data-stu-id="bb8c7-206">Relationships</span></span>
<span data-ttu-id="bb8c7-207">无</span><span class="sxs-lookup"><span data-stu-id="bb8c7-207">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb8c7-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb8c7-208">JSON Representation</span></span>
<span data-ttu-id="bb8c7-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb8c7-209">Here is a JSON representation of the resource.</span></span>
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



