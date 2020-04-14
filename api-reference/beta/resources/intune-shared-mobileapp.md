---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bdc0222f63a881ddf756b6fc436bbf5e49bd831
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466143"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="c99fb-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c99fb-103">mobileApp resource type</span></span>

<span data-ttu-id="c99fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c99fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c99fb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c99fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c99fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c99fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c99fb-107">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="c99fb-107">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="c99fb-108">方法</span><span class="sxs-lookup"><span data-stu-id="c99fb-108">Methods</span></span>
|<span data-ttu-id="c99fb-109">方法</span><span class="sxs-lookup"><span data-stu-id="c99fb-109">Method</span></span>|<span data-ttu-id="c99fb-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c99fb-110">Return Type</span></span>|<span data-ttu-id="c99fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="c99fb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c99fb-112">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="c99fb-112">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="c99fb-113">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-113">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="c99fb-114">列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c99fb-114">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="c99fb-115">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="c99fb-115">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="c99fb-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="c99fb-116">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="c99fb-117">读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c99fb-117">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="c99fb-118">**应用**</span><span class="sxs-lookup"><span data-stu-id="c99fb-118">**Apps**</span></span>|
|[<span data-ttu-id="c99fb-119">分配操作</span><span class="sxs-lookup"><span data-stu-id="c99fb-119">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="c99fb-120">无</span><span class="sxs-lookup"><span data-stu-id="c99fb-120">None</span></span>|<span data-ttu-id="c99fb-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-121">Not yet documented</span></span>|
|[<span data-ttu-id="c99fb-122">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="c99fb-122">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="c99fb-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c99fb-123">Int64</span></span>|<span data-ttu-id="c99fb-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-124">Not yet documented</span></span>|
|[<span data-ttu-id="c99fb-125">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="c99fb-125">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="c99fb-126">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-126">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="c99fb-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-127">Not yet documented</span></span>|
|[<span data-ttu-id="c99fb-128">updateRelationships 操作</span><span class="sxs-lookup"><span data-stu-id="c99fb-128">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="c99fb-129">无</span><span class="sxs-lookup"><span data-stu-id="c99fb-129">None</span></span>|<span data-ttu-id="c99fb-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-130">Not yet documented</span></span>|
|[<span data-ttu-id="c99fb-131">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="c99fb-131">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="c99fb-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="c99fb-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-133">Not yet documented</span></span>|
|<span data-ttu-id="c99fb-134">**策略集**</span><span class="sxs-lookup"><span data-stu-id="c99fb-134">**Policy Set**</span></span>|
|[<span data-ttu-id="c99fb-135">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="c99fb-135">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="c99fb-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="c99fb-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c99fb-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c99fb-138">属性</span><span class="sxs-lookup"><span data-stu-id="c99fb-138">Properties</span></span>
|<span data-ttu-id="c99fb-139">属性</span><span class="sxs-lookup"><span data-stu-id="c99fb-139">Property</span></span>|<span data-ttu-id="c99fb-140">类型</span><span class="sxs-lookup"><span data-stu-id="c99fb-140">Type</span></span>|<span data-ttu-id="c99fb-141">说明</span><span class="sxs-lookup"><span data-stu-id="c99fb-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99fb-142">id</span><span class="sxs-lookup"><span data-stu-id="c99fb-142">id</span></span>|<span data-ttu-id="c99fb-143">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fb-143">String</span></span>|<span data-ttu-id="c99fb-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c99fb-144">Key of the entity.</span></span>|
|<span data-ttu-id="c99fb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c99fb-145">displayName</span></span>|<span data-ttu-id="c99fb-146">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-146">String</span></span>|<span data-ttu-id="c99fb-147">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c99fb-147">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="c99fb-148">description</span><span class="sxs-lookup"><span data-stu-id="c99fb-148">description</span></span>|<span data-ttu-id="c99fb-149">字符串</span><span class="sxs-lookup"><span data-stu-id="c99fb-149">String</span></span>|<span data-ttu-id="c99fb-150">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c99fb-150">The description of the app.</span></span>|
|<span data-ttu-id="c99fb-151">publisher</span><span class="sxs-lookup"><span data-stu-id="c99fb-151">publisher</span></span>|<span data-ttu-id="c99fb-152">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-152">String</span></span>|<span data-ttu-id="c99fb-153">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c99fb-153">The publisher of the app.</span></span>|
|<span data-ttu-id="c99fb-154">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c99fb-154">largeIcon</span></span>|[<span data-ttu-id="c99fb-155">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c99fb-155">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c99fb-156">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c99fb-156">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="c99fb-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c99fb-157">createdDateTime</span></span>|<span data-ttu-id="c99fb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c99fb-158">DateTimeOffset</span></span>|<span data-ttu-id="c99fb-159">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c99fb-159">The date and time the app was created.</span></span>|
|<span data-ttu-id="c99fb-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c99fb-160">lastModifiedDateTime</span></span>|<span data-ttu-id="c99fb-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c99fb-161">DateTimeOffset</span></span>|<span data-ttu-id="c99fb-162">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c99fb-162">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="c99fb-163">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c99fb-163">isFeatured</span></span>|<span data-ttu-id="c99fb-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fb-164">Boolean</span></span>|<span data-ttu-id="c99fb-165">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="c99fb-165">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="c99fb-166">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c99fb-166">privacyInformationUrl</span></span>|<span data-ttu-id="c99fb-167">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-167">String</span></span>|<span data-ttu-id="c99fb-168">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c99fb-168">The privacy statement Url.</span></span>|
|<span data-ttu-id="c99fb-169">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c99fb-169">informationUrl</span></span>|<span data-ttu-id="c99fb-170">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-170">String</span></span>|<span data-ttu-id="c99fb-171">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="c99fb-171">The more information Url.</span></span>|
|<span data-ttu-id="c99fb-172">owner</span><span class="sxs-lookup"><span data-stu-id="c99fb-172">owner</span></span>|<span data-ttu-id="c99fb-173">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-173">String</span></span>|<span data-ttu-id="c99fb-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c99fb-174">The owner of the app.</span></span>|
|<span data-ttu-id="c99fb-175">developer</span><span class="sxs-lookup"><span data-stu-id="c99fb-175">developer</span></span>|<span data-ttu-id="c99fb-176">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-176">String</span></span>|<span data-ttu-id="c99fb-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c99fb-177">The developer of the app.</span></span>|
|<span data-ttu-id="c99fb-178">notes</span><span class="sxs-lookup"><span data-stu-id="c99fb-178">notes</span></span>|<span data-ttu-id="c99fb-179">String</span><span class="sxs-lookup"><span data-stu-id="c99fb-179">String</span></span>|<span data-ttu-id="c99fb-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c99fb-180">Notes for the app.</span></span>|
|<span data-ttu-id="c99fb-181">uploadState</span><span class="sxs-lookup"><span data-stu-id="c99fb-181">uploadState</span></span>|<span data-ttu-id="c99fb-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c99fb-182">Int32</span></span>|<span data-ttu-id="c99fb-183">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c99fb-183">The upload state.</span></span>|
|<span data-ttu-id="c99fb-184">publishingState</span><span class="sxs-lookup"><span data-stu-id="c99fb-184">publishingState</span></span>|[<span data-ttu-id="c99fb-185">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c99fb-185">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c99fb-186">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c99fb-186">The publishing state for the app.</span></span> <span data-ttu-id="c99fb-187">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c99fb-187">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c99fb-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c99fb-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c99fb-189">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c99fb-189">isAssigned</span></span>|<span data-ttu-id="c99fb-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99fb-190">Boolean</span></span>|<span data-ttu-id="c99fb-191">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="c99fb-191">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="c99fb-192">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c99fb-192">roleScopeTagIds</span></span>|<span data-ttu-id="c99fb-193">String collection</span><span class="sxs-lookup"><span data-stu-id="c99fb-193">String collection</span></span>|<span data-ttu-id="c99fb-194">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-194">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="c99fb-195">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c99fb-195">dependentAppCount</span></span>|<span data-ttu-id="c99fb-196">Int32</span><span class="sxs-lookup"><span data-stu-id="c99fb-196">Int32</span></span>|<span data-ttu-id="c99fb-197">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="c99fb-197">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c99fb-198">关系</span><span class="sxs-lookup"><span data-stu-id="c99fb-198">Relationships</span></span>
|<span data-ttu-id="c99fb-199">关系</span><span class="sxs-lookup"><span data-stu-id="c99fb-199">Relationship</span></span>|<span data-ttu-id="c99fb-200">类型</span><span class="sxs-lookup"><span data-stu-id="c99fb-200">Type</span></span>|<span data-ttu-id="c99fb-201">说明</span><span class="sxs-lookup"><span data-stu-id="c99fb-201">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99fb-202">**应用**</span><span class="sxs-lookup"><span data-stu-id="c99fb-202">**Apps**</span></span>|
|<span data-ttu-id="c99fb-203">categories</span><span class="sxs-lookup"><span data-stu-id="c99fb-203">categories</span></span>|<span data-ttu-id="c99fb-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="c99fb-205">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-205">The list of categories for this app.</span></span>|
|<span data-ttu-id="c99fb-206">assignments</span><span class="sxs-lookup"><span data-stu-id="c99fb-206">assignments</span></span>|<span data-ttu-id="c99fb-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c99fb-208">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-208">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="c99fb-209">installSummary</span><span class="sxs-lookup"><span data-stu-id="c99fb-209">installSummary</span></span>|[<span data-ttu-id="c99fb-210">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c99fb-210">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="c99fb-211">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="c99fb-211">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="c99fb-212">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c99fb-212">deviceStatuses</span></span>|<span data-ttu-id="c99fb-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="c99fb-214">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-214">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="c99fb-215">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c99fb-215">userStatuses</span></span>|<span data-ttu-id="c99fb-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="c99fb-217">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-217">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="c99fb-218">相互</span><span class="sxs-lookup"><span data-stu-id="c99fb-218">relationships</span></span>|<span data-ttu-id="c99fb-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="c99fb-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="c99fb-220">此移动应用的关系列表。</span><span class="sxs-lookup"><span data-stu-id="c99fb-220">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c99fb-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c99fb-221">JSON Representation</span></span>
<span data-ttu-id="c99fb-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c99fb-222">Here is a JSON representation of the resource.</span></span>
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



