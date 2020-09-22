---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54a6f6d3ea02df88a02f590017527fc2e5bce6a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025281"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="a877a-106">vppToken 资源类型</span><span class="sxs-lookup"><span data-stu-id="a877a-106">vppToken resource type</span></span>

<span data-ttu-id="a877a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a877a-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a877a-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a877a-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a877a-109">通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。</span><span class="sxs-lookup"><span data-stu-id="a877a-109">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="a877a-110">这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。</span><span class="sxs-lookup"><span data-stu-id="a877a-110">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="a877a-111">然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。</span><span class="sxs-lookup"><span data-stu-id="a877a-111">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="a877a-112">可上传多个 Apple VPP 企业版或教育版令牌。</span><span class="sxs-lookup"><span data-stu-id="a877a-112">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="a877a-113">方法</span><span class="sxs-lookup"><span data-stu-id="a877a-113">Methods</span></span>
|<span data-ttu-id="a877a-114">方法</span><span class="sxs-lookup"><span data-stu-id="a877a-114">Method</span></span>|<span data-ttu-id="a877a-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="a877a-115">Return Type</span></span>|<span data-ttu-id="a877a-116">说明</span><span class="sxs-lookup"><span data-stu-id="a877a-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a877a-117">列出 vppTokens</span><span class="sxs-lookup"><span data-stu-id="a877a-117">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="a877a-118">[vppToken](../resources/intune-onboarding-vpptoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a877a-118">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="a877a-119">列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a877a-119">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="a877a-120">获取 vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-120">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="a877a-121">vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-121">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="a877a-122">读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a877a-122">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="a877a-123">创建 vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-123">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="a877a-124">vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-124">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="a877a-125">创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a877a-125">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="a877a-126">删除 vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-126">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="a877a-127">无</span><span class="sxs-lookup"><span data-stu-id="a877a-127">None</span></span>|<span data-ttu-id="a877a-128">删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="a877a-128">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="a877a-129">更新 vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-129">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="a877a-130">vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-130">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="a877a-131">更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a877a-131">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="a877a-132">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="a877a-132">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="a877a-133">vppToken</span><span class="sxs-lookup"><span data-stu-id="a877a-133">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="a877a-134">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="a877a-134">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|

## <a name="properties"></a><span data-ttu-id="a877a-135">属性</span><span class="sxs-lookup"><span data-stu-id="a877a-135">Properties</span></span>
|<span data-ttu-id="a877a-136">属性</span><span class="sxs-lookup"><span data-stu-id="a877a-136">Property</span></span>|<span data-ttu-id="a877a-137">类型</span><span class="sxs-lookup"><span data-stu-id="a877a-137">Type</span></span>|<span data-ttu-id="a877a-138">说明</span><span class="sxs-lookup"><span data-stu-id="a877a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a877a-139">id</span><span class="sxs-lookup"><span data-stu-id="a877a-139">id</span></span>|<span data-ttu-id="a877a-140">String</span><span class="sxs-lookup"><span data-stu-id="a877a-140">String</span></span>|<span data-ttu-id="a877a-141">这是创建 appleVolumePurchaseProgramToken 时自动生成的。</span><span class="sxs-lookup"><span data-stu-id="a877a-141">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="a877a-142">它是实体的键。</span><span class="sxs-lookup"><span data-stu-id="a877a-142">It is the Key of the entity.</span></span>|
|<span data-ttu-id="a877a-143">organizationName</span><span class="sxs-lookup"><span data-stu-id="a877a-143">organizationName</span></span>|<span data-ttu-id="a877a-144">String</span><span class="sxs-lookup"><span data-stu-id="a877a-144">String</span></span>|<span data-ttu-id="a877a-145">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="a877a-145">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a877a-146">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a877a-146">vppTokenAccountType</span></span>|[<span data-ttu-id="a877a-147">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a877a-147">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="a877a-148">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="a877a-148">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a877a-149">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a877a-149">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a877a-150">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="a877a-150">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a877a-151">appleId</span><span class="sxs-lookup"><span data-stu-id="a877a-151">appleId</span></span>|<span data-ttu-id="a877a-152">String</span><span class="sxs-lookup"><span data-stu-id="a877a-152">String</span></span>|<span data-ttu-id="a877a-153">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="a877a-153">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a877a-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a877a-154">expirationDateTime</span></span>|<span data-ttu-id="a877a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a877a-155">DateTimeOffset</span></span>|<span data-ttu-id="a877a-156">Apple Volume Purchase Program 令牌的到期日期时间。</span><span class="sxs-lookup"><span data-stu-id="a877a-156">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a877a-157">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a877a-157">lastSyncDateTime</span></span>|<span data-ttu-id="a877a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a877a-158">DateTimeOffset</span></span>|<span data-ttu-id="a877a-159">上次使用 Apple Volume purchase program 服务（apple Volume purchase program 令牌）完成应用程序同步的时间。</span><span class="sxs-lookup"><span data-stu-id="a877a-159">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a877a-160">token</span><span class="sxs-lookup"><span data-stu-id="a877a-160">token</span></span>|<span data-ttu-id="a877a-161">String</span><span class="sxs-lookup"><span data-stu-id="a877a-161">String</span></span>|<span data-ttu-id="a877a-162">从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。</span><span class="sxs-lookup"><span data-stu-id="a877a-162">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="a877a-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a877a-163">lastModifiedDateTime</span></span>|<span data-ttu-id="a877a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a877a-164">DateTimeOffset</span></span>|<span data-ttu-id="a877a-165">与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="a877a-165">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a877a-166">state</span><span class="sxs-lookup"><span data-stu-id="a877a-166">state</span></span>|[<span data-ttu-id="a877a-167">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="a877a-167">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="a877a-168">Apple Volume Purchase Program 令牌的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a877a-168">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a877a-169">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a877a-169">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="a877a-170">可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。</span><span class="sxs-lookup"><span data-stu-id="a877a-170">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="a877a-171">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a877a-171">lastSyncStatus</span></span>|[<span data-ttu-id="a877a-172">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="a877a-172">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="a877a-173">使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。</span><span class="sxs-lookup"><span data-stu-id="a877a-173">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="a877a-174">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a877a-174">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="a877a-175">可取值为：`none`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a877a-175">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a877a-176">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="a877a-176">automaticallyUpdateApps</span></span>|<span data-ttu-id="a877a-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a877a-177">Boolean</span></span>|<span data-ttu-id="a877a-178">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a877a-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="a877a-179">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="a877a-179">countryOrRegion</span></span>|<span data-ttu-id="a877a-180">String</span><span class="sxs-lookup"><span data-stu-id="a877a-180">String</span></span>|<span data-ttu-id="a877a-181">是否自动更新适用于 VPP 令牌的应用。</span><span class="sxs-lookup"><span data-stu-id="a877a-181">Whether or not apps for the VPP token will be automatically updated.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a877a-182">关系</span><span class="sxs-lookup"><span data-stu-id="a877a-182">Relationships</span></span>
<span data-ttu-id="a877a-183">无</span><span class="sxs-lookup"><span data-stu-id="a877a-183">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a877a-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a877a-184">JSON Representation</span></span>
<span data-ttu-id="a877a-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a877a-185">Here is a JSON representation of the resource.</span></span>
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









