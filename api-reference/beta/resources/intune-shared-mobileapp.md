---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bde61142c5d8644ce12911249b17dd61b2c9c131
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199913"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="14386-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="14386-103">mobileApp resource type</span></span>

> <span data-ttu-id="14386-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14386-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14386-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14386-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14386-106">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="14386-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="14386-107">方法</span><span class="sxs-lookup"><span data-stu-id="14386-107">Methods</span></span>
|<span data-ttu-id="14386-108">方法</span><span class="sxs-lookup"><span data-stu-id="14386-108">Method</span></span>|<span data-ttu-id="14386-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="14386-109">Return Type</span></span>|<span data-ttu-id="14386-110">说明</span><span class="sxs-lookup"><span data-stu-id="14386-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14386-111">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="14386-111">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="14386-112">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14386-112">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="14386-113">列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14386-113">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="14386-114">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="14386-114">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="14386-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="14386-115">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="14386-116">读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14386-116">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="14386-117">**应用**</span><span class="sxs-lookup"><span data-stu-id="14386-117">**Apps**</span></span>|
|[<span data-ttu-id="14386-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="14386-118">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="14386-119">无</span><span class="sxs-lookup"><span data-stu-id="14386-119">None</span></span>|<span data-ttu-id="14386-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-120">Not yet documented</span></span>|
|[<span data-ttu-id="14386-121">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="14386-121">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="14386-122">Int64</span><span class="sxs-lookup"><span data-stu-id="14386-122">Int64</span></span>|<span data-ttu-id="14386-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-123">Not yet documented</span></span>|
|[<span data-ttu-id="14386-124">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="14386-124">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="14386-125">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14386-125">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="14386-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-126">Not yet documented</span></span>|
|[<span data-ttu-id="14386-127">updateRelationships 操作</span><span class="sxs-lookup"><span data-stu-id="14386-127">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="14386-128">无</span><span class="sxs-lookup"><span data-stu-id="14386-128">None</span></span>|<span data-ttu-id="14386-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-129">Not yet documented</span></span>|
|[<span data-ttu-id="14386-130">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="14386-130">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="14386-131">mobileAppRelationshipState 集合</span><span class="sxs-lookup"><span data-stu-id="14386-131">mobileAppRelationshipState collection</span></span>|<span data-ttu-id="14386-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-132">Not yet documented</span></span>|
|<span data-ttu-id="14386-133">**策略集**</span><span class="sxs-lookup"><span data-stu-id="14386-133">**Policy Set**</span></span>|
|[<span data-ttu-id="14386-134">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="14386-134">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="14386-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="14386-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="14386-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14386-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="14386-137">属性</span><span class="sxs-lookup"><span data-stu-id="14386-137">Properties</span></span>
|<span data-ttu-id="14386-138">属性</span><span class="sxs-lookup"><span data-stu-id="14386-138">Property</span></span>|<span data-ttu-id="14386-139">类型</span><span class="sxs-lookup"><span data-stu-id="14386-139">Type</span></span>|<span data-ttu-id="14386-140">说明</span><span class="sxs-lookup"><span data-stu-id="14386-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14386-141">id</span><span class="sxs-lookup"><span data-stu-id="14386-141">id</span></span>|<span data-ttu-id="14386-142">字符串</span><span class="sxs-lookup"><span data-stu-id="14386-142">String</span></span>|<span data-ttu-id="14386-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14386-143">Key of the entity.</span></span>|
|<span data-ttu-id="14386-144">displayName</span><span class="sxs-lookup"><span data-stu-id="14386-144">displayName</span></span>|<span data-ttu-id="14386-145">String</span><span class="sxs-lookup"><span data-stu-id="14386-145">String</span></span>|<span data-ttu-id="14386-146">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="14386-146">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="14386-147">说明</span><span class="sxs-lookup"><span data-stu-id="14386-147">description</span></span>|<span data-ttu-id="14386-148">字符串</span><span class="sxs-lookup"><span data-stu-id="14386-148">String</span></span>|<span data-ttu-id="14386-149">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="14386-149">The description of the app.</span></span>|
|<span data-ttu-id="14386-150">publisher</span><span class="sxs-lookup"><span data-stu-id="14386-150">publisher</span></span>|<span data-ttu-id="14386-151">String</span><span class="sxs-lookup"><span data-stu-id="14386-151">String</span></span>|<span data-ttu-id="14386-152">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="14386-152">The publisher of the app.</span></span>|
|<span data-ttu-id="14386-153">largeIcon</span><span class="sxs-lookup"><span data-stu-id="14386-153">largeIcon</span></span>|[<span data-ttu-id="14386-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="14386-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="14386-155">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="14386-155">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="14386-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14386-156">createdDateTime</span></span>|<span data-ttu-id="14386-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14386-157">DateTimeOffset</span></span>|<span data-ttu-id="14386-158">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="14386-158">The date and time the app was created.</span></span>|
|<span data-ttu-id="14386-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14386-159">lastModifiedDateTime</span></span>|<span data-ttu-id="14386-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14386-160">DateTimeOffset</span></span>|<span data-ttu-id="14386-161">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="14386-161">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="14386-162">isFeatured</span><span class="sxs-lookup"><span data-stu-id="14386-162">isFeatured</span></span>|<span data-ttu-id="14386-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="14386-163">Boolean</span></span>|<span data-ttu-id="14386-164">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="14386-164">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="14386-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="14386-165">privacyInformationUrl</span></span>|<span data-ttu-id="14386-166">String</span><span class="sxs-lookup"><span data-stu-id="14386-166">String</span></span>|<span data-ttu-id="14386-167">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="14386-167">The privacy statement Url.</span></span>|
|<span data-ttu-id="14386-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="14386-168">informationUrl</span></span>|<span data-ttu-id="14386-169">String</span><span class="sxs-lookup"><span data-stu-id="14386-169">String</span></span>|<span data-ttu-id="14386-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="14386-170">The more information Url.</span></span>|
|<span data-ttu-id="14386-171">owner</span><span class="sxs-lookup"><span data-stu-id="14386-171">owner</span></span>|<span data-ttu-id="14386-172">String</span><span class="sxs-lookup"><span data-stu-id="14386-172">String</span></span>|<span data-ttu-id="14386-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="14386-173">The owner of the app.</span></span>|
|<span data-ttu-id="14386-174">developer</span><span class="sxs-lookup"><span data-stu-id="14386-174">developer</span></span>|<span data-ttu-id="14386-175">String</span><span class="sxs-lookup"><span data-stu-id="14386-175">String</span></span>|<span data-ttu-id="14386-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="14386-176">The developer of the app.</span></span>|
|<span data-ttu-id="14386-177">notes</span><span class="sxs-lookup"><span data-stu-id="14386-177">notes</span></span>|<span data-ttu-id="14386-178">String</span><span class="sxs-lookup"><span data-stu-id="14386-178">String</span></span>|<span data-ttu-id="14386-179">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="14386-179">Notes for the app.</span></span>|
|<span data-ttu-id="14386-180">uploadState</span><span class="sxs-lookup"><span data-stu-id="14386-180">uploadState</span></span>|<span data-ttu-id="14386-181">Int32</span><span class="sxs-lookup"><span data-stu-id="14386-181">Int32</span></span>|<span data-ttu-id="14386-182">上载状态。</span><span class="sxs-lookup"><span data-stu-id="14386-182">The upload state.</span></span>|
|<span data-ttu-id="14386-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="14386-183">publishingState</span></span>|<span data-ttu-id="14386-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="14386-184">mobileAppPublishingState</span></span>|<span data-ttu-id="14386-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="14386-185">The publishing state for the app.</span></span> <span data-ttu-id="14386-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="14386-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="14386-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="14386-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="14386-188">isAssigned</span><span class="sxs-lookup"><span data-stu-id="14386-188">isAssigned</span></span>|<span data-ttu-id="14386-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="14386-189">Boolean</span></span>|<span data-ttu-id="14386-190">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="14386-190">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="14386-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14386-191">roleScopeTagIds</span></span>|<span data-ttu-id="14386-192">String collection</span><span class="sxs-lookup"><span data-stu-id="14386-192">String collection</span></span>|<span data-ttu-id="14386-193">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="14386-193">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="14386-194">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="14386-194">dependentAppCount</span></span>|<span data-ttu-id="14386-195">Int32</span><span class="sxs-lookup"><span data-stu-id="14386-195">Int32</span></span>|<span data-ttu-id="14386-196">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="14386-196">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14386-197">关系</span><span class="sxs-lookup"><span data-stu-id="14386-197">Relationships</span></span>
|<span data-ttu-id="14386-198">关系</span><span class="sxs-lookup"><span data-stu-id="14386-198">Relationship</span></span>|<span data-ttu-id="14386-199">类型</span><span class="sxs-lookup"><span data-stu-id="14386-199">Type</span></span>|<span data-ttu-id="14386-200">说明</span><span class="sxs-lookup"><span data-stu-id="14386-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14386-201">**应用**</span><span class="sxs-lookup"><span data-stu-id="14386-201">**Apps**</span></span>|
|<span data-ttu-id="14386-202">categories</span><span class="sxs-lookup"><span data-stu-id="14386-202">categories</span></span>|<span data-ttu-id="14386-203">mobileAppCategory 集合</span><span class="sxs-lookup"><span data-stu-id="14386-203">mobileAppCategory collection</span></span>|<span data-ttu-id="14386-204">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="14386-204">The list of categories for this app.</span></span>|
|<span data-ttu-id="14386-205">assignments</span><span class="sxs-lookup"><span data-stu-id="14386-205">assignments</span></span>|<span data-ttu-id="14386-206">mobileAppAssignment 集合</span><span class="sxs-lookup"><span data-stu-id="14386-206">mobileAppAssignment collection</span></span>|<span data-ttu-id="14386-207">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="14386-207">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="14386-208">installSummary</span><span class="sxs-lookup"><span data-stu-id="14386-208">installSummary</span></span>|<span data-ttu-id="14386-209">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="14386-209">mobileAppInstallSummary</span></span>|<span data-ttu-id="14386-210">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="14386-210">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="14386-211">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="14386-211">deviceStatuses</span></span>|<span data-ttu-id="14386-212">mobileAppInstallStatus 集合</span><span class="sxs-lookup"><span data-stu-id="14386-212">mobileAppInstallStatus collection</span></span>|<span data-ttu-id="14386-213">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="14386-213">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="14386-214">userStatuses</span><span class="sxs-lookup"><span data-stu-id="14386-214">userStatuses</span></span>|<span data-ttu-id="14386-215">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="14386-215">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="14386-216">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="14386-216">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="14386-217">相互</span><span class="sxs-lookup"><span data-stu-id="14386-217">relationships</span></span>|<span data-ttu-id="14386-218">mobileAppRelationship 集合</span><span class="sxs-lookup"><span data-stu-id="14386-218">mobileAppRelationship collection</span></span>|<span data-ttu-id="14386-219">此移动应用的关系列表。</span><span class="sxs-lookup"><span data-stu-id="14386-219">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14386-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14386-220">JSON Representation</span></span>
<span data-ttu-id="14386-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14386-221">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024
}
```



