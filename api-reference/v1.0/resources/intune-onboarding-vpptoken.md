---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fd3d625969713c639661562fca517be3f9378b8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755705"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="b8eb4-106">vppToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8eb4-106">vppToken resource type</span></span>

<span data-ttu-id="b8eb4-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8eb4-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8eb4-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8eb4-109">通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-109">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="b8eb4-110">这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-110">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="b8eb4-111">然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-111">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="b8eb4-112">可上传多个 Apple VPP 企业版或教育版令牌。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-112">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="b8eb4-113">Methods</span><span class="sxs-lookup"><span data-stu-id="b8eb4-113">Methods</span></span>
|<span data-ttu-id="b8eb4-114">方法</span><span class="sxs-lookup"><span data-stu-id="b8eb4-114">Method</span></span>|<span data-ttu-id="b8eb4-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8eb4-115">Return Type</span></span>|<span data-ttu-id="b8eb4-116">Description</span><span class="sxs-lookup"><span data-stu-id="b8eb4-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8eb4-117">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="b8eb4-117">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="b8eb4-118">[vppToken](../resources/intune-onboarding-vpptoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8eb4-118">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="b8eb4-119">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-119">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="b8eb4-120">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-120">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="b8eb4-121">vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-121">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="b8eb4-122">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-122">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="b8eb4-123">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-123">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="b8eb4-124">vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-124">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="b8eb4-125">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-125">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="b8eb4-126">删除 vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-126">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="b8eb4-127">无</span><span class="sxs-lookup"><span data-stu-id="b8eb4-127">None</span></span>|<span data-ttu-id="b8eb4-128">删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-128">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="b8eb4-129">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-129">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="b8eb4-130">vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-130">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="b8eb4-131">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-131">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="b8eb4-132">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="b8eb4-132">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="b8eb4-133">vppToken</span><span class="sxs-lookup"><span data-stu-id="b8eb4-133">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="b8eb4-134">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="b8eb4-134">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|

## <a name="properties"></a><span data-ttu-id="b8eb4-135">属性</span><span class="sxs-lookup"><span data-stu-id="b8eb4-135">Properties</span></span>
|<span data-ttu-id="b8eb4-136">属性</span><span class="sxs-lookup"><span data-stu-id="b8eb4-136">Property</span></span>|<span data-ttu-id="b8eb4-137">类型</span><span class="sxs-lookup"><span data-stu-id="b8eb4-137">Type</span></span>|<span data-ttu-id="b8eb4-138">说明</span><span class="sxs-lookup"><span data-stu-id="b8eb4-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8eb4-139">id</span><span class="sxs-lookup"><span data-stu-id="b8eb4-139">id</span></span>|<span data-ttu-id="b8eb4-140">String</span><span class="sxs-lookup"><span data-stu-id="b8eb4-140">String</span></span>|<span data-ttu-id="b8eb4-141">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-141">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="b8eb4-142">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-142">It is the Key of the entity.</span></span>|
|<span data-ttu-id="b8eb4-143">organizationName</span><span class="sxs-lookup"><span data-stu-id="b8eb4-143">organizationName</span></span>|<span data-ttu-id="b8eb4-144">String</span><span class="sxs-lookup"><span data-stu-id="b8eb4-144">String</span></span>|<span data-ttu-id="b8eb4-145">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="b8eb4-145">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b8eb4-146">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b8eb4-146">vppTokenAccountType</span></span>|[<span data-ttu-id="b8eb4-147">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b8eb4-147">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b8eb4-148">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-148">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b8eb4-149">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-149">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b8eb4-150">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-150">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b8eb4-151">appleId</span><span class="sxs-lookup"><span data-stu-id="b8eb4-151">appleId</span></span>|<span data-ttu-id="b8eb4-152">String</span><span class="sxs-lookup"><span data-stu-id="b8eb4-152">String</span></span>|<span data-ttu-id="b8eb4-153">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-153">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8eb4-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb4-154">expirationDateTime</span></span>|<span data-ttu-id="b8eb4-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb4-155">DateTimeOffset</span></span>|<span data-ttu-id="b8eb4-156">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-156">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8eb4-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb4-157">lastSyncDateTime</span></span>|<span data-ttu-id="b8eb4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb4-158">DateTimeOffset</span></span>|<span data-ttu-id="b8eb4-159">上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-159">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8eb4-160">token</span><span class="sxs-lookup"><span data-stu-id="b8eb4-160">token</span></span>|<span data-ttu-id="b8eb4-161">String</span><span class="sxs-lookup"><span data-stu-id="b8eb4-161">String</span></span>|<span data-ttu-id="b8eb4-162">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-162">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b8eb4-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8eb4-163">lastModifiedDateTime</span></span>|<span data-ttu-id="b8eb4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8eb4-164">DateTimeOffset</span></span>|<span data-ttu-id="b8eb4-165">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-165">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b8eb4-166">state</span><span class="sxs-lookup"><span data-stu-id="b8eb4-166">state</span></span>|[<span data-ttu-id="b8eb4-167">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b8eb4-167">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="b8eb4-168">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-168">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b8eb4-169">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-169">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="b8eb4-170">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-170">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="b8eb4-171">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b8eb4-171">lastSyncStatus</span></span>|[<span data-ttu-id="b8eb4-172">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b8eb4-172">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="b8eb4-173">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-173">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b8eb4-174">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-174">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="b8eb4-175">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-175">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="b8eb4-176">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="b8eb4-176">automaticallyUpdateApps</span></span>|<span data-ttu-id="b8eb4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8eb4-177">Boolean</span></span>|<span data-ttu-id="b8eb4-178">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b8eb4-179">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b8eb4-179">countryOrRegion</span></span>|<span data-ttu-id="b8eb4-180">String</span><span class="sxs-lookup"><span data-stu-id="b8eb4-180">String</span></span>|<span data-ttu-id="b8eb4-181">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-181">Whether or not apps for the VPP token will be automatically updated.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8eb4-182">关系</span><span class="sxs-lookup"><span data-stu-id="b8eb4-182">Relationships</span></span>
<span data-ttu-id="b8eb4-183">无</span><span class="sxs-lookup"><span data-stu-id="b8eb4-183">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8eb4-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8eb4-184">JSON Representation</span></span>
<span data-ttu-id="b8eb4-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8eb4-185">Here is a JSON representation of the resource.</span></span>
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
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```




