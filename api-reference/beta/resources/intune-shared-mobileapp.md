---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9688f0b4223fe0e1ec2e355c54f0efcbffdc2573
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538719"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="9ae29-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ae29-103">mobileApp resource type</span></span>

> <span data-ttu-id="9ae29-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ae29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ae29-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ae29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ae29-106">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="9ae29-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="9ae29-107">方法</span><span class="sxs-lookup"><span data-stu-id="9ae29-107">Methods</span></span>
|<span data-ttu-id="9ae29-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ae29-108">Method</span></span>|<span data-ttu-id="9ae29-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ae29-109">Return Type</span></span>|<span data-ttu-id="9ae29-110">说明</span><span class="sxs-lookup"><span data-stu-id="9ae29-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ae29-111">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="9ae29-111">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="9ae29-112">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-112">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="9ae29-113">列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ae29-113">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="9ae29-114">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="9ae29-114">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="9ae29-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="9ae29-115">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="9ae29-116">读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ae29-116">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="9ae29-117">**应用**</span><span class="sxs-lookup"><span data-stu-id="9ae29-117">**Apps**</span></span>|
|[<span data-ttu-id="9ae29-118">分配操作</span><span class="sxs-lookup"><span data-stu-id="9ae29-118">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="9ae29-119">无</span><span class="sxs-lookup"><span data-stu-id="9ae29-119">None</span></span>|<span data-ttu-id="9ae29-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-120">Not yet documented</span></span>|
|[<span data-ttu-id="9ae29-121">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="9ae29-121">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="9ae29-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9ae29-122">Int64</span></span>|<span data-ttu-id="9ae29-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-123">Not yet documented</span></span>|
|[<span data-ttu-id="9ae29-124">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="9ae29-124">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="9ae29-125">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-125">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="9ae29-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-126">Not yet documented</span></span>|
|[<span data-ttu-id="9ae29-127">updateRelationships 操作</span><span class="sxs-lookup"><span data-stu-id="9ae29-127">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="9ae29-128">无</span><span class="sxs-lookup"><span data-stu-id="9ae29-128">None</span></span>|<span data-ttu-id="9ae29-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-129">Not yet documented</span></span>|
|[<span data-ttu-id="9ae29-130">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="9ae29-130">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="9ae29-131">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-131">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="9ae29-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-132">Not yet documented</span></span>|
|<span data-ttu-id="9ae29-133">**策略集**</span><span class="sxs-lookup"><span data-stu-id="9ae29-133">**Policy Set**</span></span>|
|[<span data-ttu-id="9ae29-134">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="9ae29-134">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="9ae29-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="9ae29-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ae29-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9ae29-137">属性</span><span class="sxs-lookup"><span data-stu-id="9ae29-137">Properties</span></span>
|<span data-ttu-id="9ae29-138">属性</span><span class="sxs-lookup"><span data-stu-id="9ae29-138">Property</span></span>|<span data-ttu-id="9ae29-139">类型</span><span class="sxs-lookup"><span data-stu-id="9ae29-139">Type</span></span>|<span data-ttu-id="9ae29-140">说明</span><span class="sxs-lookup"><span data-stu-id="9ae29-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae29-141">id</span><span class="sxs-lookup"><span data-stu-id="9ae29-141">id</span></span>|<span data-ttu-id="9ae29-142">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-142">String</span></span>|<span data-ttu-id="9ae29-143">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ae29-143">Key of the entity.</span></span>|
|<span data-ttu-id="9ae29-144">displayName</span><span class="sxs-lookup"><span data-stu-id="9ae29-144">displayName</span></span>|<span data-ttu-id="9ae29-145">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-145">String</span></span>|<span data-ttu-id="9ae29-146">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9ae29-146">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="9ae29-147">说明</span><span class="sxs-lookup"><span data-stu-id="9ae29-147">description</span></span>|<span data-ttu-id="9ae29-148">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-148">String</span></span>|<span data-ttu-id="9ae29-149">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9ae29-149">The description of the app.</span></span>|
|<span data-ttu-id="9ae29-150">publisher</span><span class="sxs-lookup"><span data-stu-id="9ae29-150">publisher</span></span>|<span data-ttu-id="9ae29-151">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-151">String</span></span>|<span data-ttu-id="9ae29-152">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9ae29-152">The publisher of the app.</span></span>|
|<span data-ttu-id="9ae29-153">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ae29-153">largeIcon</span></span>|[<span data-ttu-id="9ae29-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ae29-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ae29-155">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9ae29-155">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="9ae29-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ae29-156">createdDateTime</span></span>|<span data-ttu-id="9ae29-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ae29-157">DateTimeOffset</span></span>|<span data-ttu-id="9ae29-158">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9ae29-158">The date and time the app was created.</span></span>|
|<span data-ttu-id="9ae29-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ae29-159">lastModifiedDateTime</span></span>|<span data-ttu-id="9ae29-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ae29-160">DateTimeOffset</span></span>|<span data-ttu-id="9ae29-161">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9ae29-161">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="9ae29-162">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ae29-162">isFeatured</span></span>|<span data-ttu-id="9ae29-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ae29-163">Boolean</span></span>|<span data-ttu-id="9ae29-164">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="9ae29-164">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="9ae29-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ae29-165">privacyInformationUrl</span></span>|<span data-ttu-id="9ae29-166">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-166">String</span></span>|<span data-ttu-id="9ae29-167">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="9ae29-167">The privacy statement Url.</span></span>|
|<span data-ttu-id="9ae29-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ae29-168">informationUrl</span></span>|<span data-ttu-id="9ae29-169">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-169">String</span></span>|<span data-ttu-id="9ae29-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="9ae29-170">The more information Url.</span></span>|
|<span data-ttu-id="9ae29-171">owner</span><span class="sxs-lookup"><span data-stu-id="9ae29-171">owner</span></span>|<span data-ttu-id="9ae29-172">String</span><span class="sxs-lookup"><span data-stu-id="9ae29-172">String</span></span>|<span data-ttu-id="9ae29-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9ae29-173">The owner of the app.</span></span>|
|<span data-ttu-id="9ae29-174">developer</span><span class="sxs-lookup"><span data-stu-id="9ae29-174">developer</span></span>|<span data-ttu-id="9ae29-175">字符串</span><span class="sxs-lookup"><span data-stu-id="9ae29-175">String</span></span>|<span data-ttu-id="9ae29-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9ae29-176">The developer of the app.</span></span>|
|<span data-ttu-id="9ae29-177">notes</span><span class="sxs-lookup"><span data-stu-id="9ae29-177">notes</span></span>|<span data-ttu-id="9ae29-178">String</span><span class="sxs-lookup"><span data-stu-id="9ae29-178">String</span></span>|<span data-ttu-id="9ae29-179">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9ae29-179">Notes for the app.</span></span>|
|<span data-ttu-id="9ae29-180">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ae29-180">uploadState</span></span>|<span data-ttu-id="9ae29-181">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae29-181">Int32</span></span>|<span data-ttu-id="9ae29-182">上载状态。</span><span class="sxs-lookup"><span data-stu-id="9ae29-182">The upload state.</span></span>|
|<span data-ttu-id="9ae29-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ae29-183">publishingState</span></span>|[<span data-ttu-id="9ae29-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9ae29-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ae29-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9ae29-185">The publishing state for the app.</span></span> <span data-ttu-id="9ae29-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9ae29-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ae29-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9ae29-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ae29-188">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ae29-188">isAssigned</span></span>|<span data-ttu-id="9ae29-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ae29-189">Boolean</span></span>|<span data-ttu-id="9ae29-190">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="9ae29-190">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="9ae29-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ae29-191">roleScopeTagIds</span></span>|<span data-ttu-id="9ae29-192">String 集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-192">String collection</span></span>|<span data-ttu-id="9ae29-193">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-193">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="9ae29-194">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9ae29-194">dependentAppCount</span></span>|<span data-ttu-id="9ae29-195">Int32</span><span class="sxs-lookup"><span data-stu-id="9ae29-195">Int32</span></span>|<span data-ttu-id="9ae29-196">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="9ae29-196">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ae29-197">关系</span><span class="sxs-lookup"><span data-stu-id="9ae29-197">Relationships</span></span>
|<span data-ttu-id="9ae29-198">关系</span><span class="sxs-lookup"><span data-stu-id="9ae29-198">Relationship</span></span>|<span data-ttu-id="9ae29-199">类型</span><span class="sxs-lookup"><span data-stu-id="9ae29-199">Type</span></span>|<span data-ttu-id="9ae29-200">说明</span><span class="sxs-lookup"><span data-stu-id="9ae29-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae29-201">**应用**</span><span class="sxs-lookup"><span data-stu-id="9ae29-201">**Apps**</span></span>|
|<span data-ttu-id="9ae29-202">categories</span><span class="sxs-lookup"><span data-stu-id="9ae29-202">categories</span></span>|<span data-ttu-id="9ae29-203">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-203">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="9ae29-204">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-204">The list of categories for this app.</span></span>|
|<span data-ttu-id="9ae29-205">assignments</span><span class="sxs-lookup"><span data-stu-id="9ae29-205">assignments</span></span>|<span data-ttu-id="9ae29-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="9ae29-207">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-207">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="9ae29-208">installSummary</span><span class="sxs-lookup"><span data-stu-id="9ae29-208">installSummary</span></span>|[<span data-ttu-id="9ae29-209">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9ae29-209">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="9ae29-210">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="9ae29-210">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="9ae29-211">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="9ae29-211">deviceStatuses</span></span>|<span data-ttu-id="9ae29-212">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-212">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="9ae29-213">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-213">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="9ae29-214">userStatuses</span><span class="sxs-lookup"><span data-stu-id="9ae29-214">userStatuses</span></span>|<span data-ttu-id="9ae29-215">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-215">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="9ae29-216">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-216">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="9ae29-217">相互</span><span class="sxs-lookup"><span data-stu-id="9ae29-217">relationships</span></span>|<span data-ttu-id="9ae29-218">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ae29-218">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="9ae29-219">此移动应用的关系列表。</span><span class="sxs-lookup"><span data-stu-id="9ae29-219">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ae29-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ae29-220">JSON Representation</span></span>
<span data-ttu-id="9ae29-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ae29-221">Here is a JSON representation of the resource.</span></span>
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



