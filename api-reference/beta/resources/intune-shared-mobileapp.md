---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca889aadfe5ce3a2bdbb7c2409db0b2ddec451af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523623"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="24303-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="24303-103">mobileApp resource type</span></span>

<span data-ttu-id="24303-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="24303-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24303-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24303-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24303-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24303-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24303-107">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="24303-107">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="24303-108">方法</span><span class="sxs-lookup"><span data-stu-id="24303-108">Methods</span></span>
|<span data-ttu-id="24303-109">方法</span><span class="sxs-lookup"><span data-stu-id="24303-109">Method</span></span>|<span data-ttu-id="24303-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="24303-110">Return Type</span></span>|<span data-ttu-id="24303-111">说明</span><span class="sxs-lookup"><span data-stu-id="24303-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24303-112">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="24303-112">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="24303-113">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24303-113">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="24303-114">列出 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24303-114">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="24303-115">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="24303-115">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="24303-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="24303-116">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="24303-117">读取 [mobileApp](../resources/intune-shared-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24303-117">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="24303-118">**应用**</span><span class="sxs-lookup"><span data-stu-id="24303-118">**Apps**</span></span>|
|[<span data-ttu-id="24303-119">分配操作</span><span class="sxs-lookup"><span data-stu-id="24303-119">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="24303-120">无</span><span class="sxs-lookup"><span data-stu-id="24303-120">None</span></span>|<span data-ttu-id="24303-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-121">Not yet documented</span></span>|
|[<span data-ttu-id="24303-122">了 getmobileappcount 函数</span><span class="sxs-lookup"><span data-stu-id="24303-122">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="24303-123">Int64</span><span class="sxs-lookup"><span data-stu-id="24303-123">Int64</span></span>|<span data-ttu-id="24303-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-124">Not yet documented</span></span>|
|[<span data-ttu-id="24303-125">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="24303-125">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="24303-126">[mobileApp](../resources/intune-shared-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24303-126">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="24303-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-127">Not yet documented</span></span>|
|[<span data-ttu-id="24303-128">updateRelationships 操作</span><span class="sxs-lookup"><span data-stu-id="24303-128">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="24303-129">无</span><span class="sxs-lookup"><span data-stu-id="24303-129">None</span></span>|<span data-ttu-id="24303-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-130">Not yet documented</span></span>|
|[<span data-ttu-id="24303-131">getRelatedAppStates 函数</span><span class="sxs-lookup"><span data-stu-id="24303-131">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="24303-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="24303-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="24303-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-133">Not yet documented</span></span>|
|<span data-ttu-id="24303-134">**策略集**</span><span class="sxs-lookup"><span data-stu-id="24303-134">**Policy Set**</span></span>|
|[<span data-ttu-id="24303-135">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="24303-135">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="24303-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="24303-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="24303-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="24303-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="24303-138">属性</span><span class="sxs-lookup"><span data-stu-id="24303-138">Properties</span></span>
|<span data-ttu-id="24303-139">属性</span><span class="sxs-lookup"><span data-stu-id="24303-139">Property</span></span>|<span data-ttu-id="24303-140">类型</span><span class="sxs-lookup"><span data-stu-id="24303-140">Type</span></span>|<span data-ttu-id="24303-141">说明</span><span class="sxs-lookup"><span data-stu-id="24303-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24303-142">id</span><span class="sxs-lookup"><span data-stu-id="24303-142">id</span></span>|<span data-ttu-id="24303-143">字符串</span><span class="sxs-lookup"><span data-stu-id="24303-143">String</span></span>|<span data-ttu-id="24303-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24303-144">Key of the entity.</span></span>|
|<span data-ttu-id="24303-145">displayName</span><span class="sxs-lookup"><span data-stu-id="24303-145">displayName</span></span>|<span data-ttu-id="24303-146">String</span><span class="sxs-lookup"><span data-stu-id="24303-146">String</span></span>|<span data-ttu-id="24303-147">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="24303-147">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="24303-148">说明</span><span class="sxs-lookup"><span data-stu-id="24303-148">description</span></span>|<span data-ttu-id="24303-149">字符串</span><span class="sxs-lookup"><span data-stu-id="24303-149">String</span></span>|<span data-ttu-id="24303-150">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="24303-150">The description of the app.</span></span>|
|<span data-ttu-id="24303-151">publisher</span><span class="sxs-lookup"><span data-stu-id="24303-151">publisher</span></span>|<span data-ttu-id="24303-152">String</span><span class="sxs-lookup"><span data-stu-id="24303-152">String</span></span>|<span data-ttu-id="24303-153">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="24303-153">The publisher of the app.</span></span>|
|<span data-ttu-id="24303-154">largeIcon</span><span class="sxs-lookup"><span data-stu-id="24303-154">largeIcon</span></span>|[<span data-ttu-id="24303-155">mimeContent</span><span class="sxs-lookup"><span data-stu-id="24303-155">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="24303-156">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="24303-156">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="24303-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24303-157">createdDateTime</span></span>|<span data-ttu-id="24303-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24303-158">DateTimeOffset</span></span>|<span data-ttu-id="24303-159">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24303-159">The date and time the app was created.</span></span>|
|<span data-ttu-id="24303-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24303-160">lastModifiedDateTime</span></span>|<span data-ttu-id="24303-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24303-161">DateTimeOffset</span></span>|<span data-ttu-id="24303-162">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24303-162">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="24303-163">isFeatured</span><span class="sxs-lookup"><span data-stu-id="24303-163">isFeatured</span></span>|<span data-ttu-id="24303-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="24303-164">Boolean</span></span>|<span data-ttu-id="24303-165">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="24303-165">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="24303-166">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="24303-166">privacyInformationUrl</span></span>|<span data-ttu-id="24303-167">String</span><span class="sxs-lookup"><span data-stu-id="24303-167">String</span></span>|<span data-ttu-id="24303-168">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="24303-168">The privacy statement Url.</span></span>|
|<span data-ttu-id="24303-169">informationUrl</span><span class="sxs-lookup"><span data-stu-id="24303-169">informationUrl</span></span>|<span data-ttu-id="24303-170">String</span><span class="sxs-lookup"><span data-stu-id="24303-170">String</span></span>|<span data-ttu-id="24303-171">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="24303-171">The more information Url.</span></span>|
|<span data-ttu-id="24303-172">owner</span><span class="sxs-lookup"><span data-stu-id="24303-172">owner</span></span>|<span data-ttu-id="24303-173">String</span><span class="sxs-lookup"><span data-stu-id="24303-173">String</span></span>|<span data-ttu-id="24303-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="24303-174">The owner of the app.</span></span>|
|<span data-ttu-id="24303-175">developer</span><span class="sxs-lookup"><span data-stu-id="24303-175">developer</span></span>|<span data-ttu-id="24303-176">String</span><span class="sxs-lookup"><span data-stu-id="24303-176">String</span></span>|<span data-ttu-id="24303-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="24303-177">The developer of the app.</span></span>|
|<span data-ttu-id="24303-178">notes</span><span class="sxs-lookup"><span data-stu-id="24303-178">notes</span></span>|<span data-ttu-id="24303-179">String</span><span class="sxs-lookup"><span data-stu-id="24303-179">String</span></span>|<span data-ttu-id="24303-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="24303-180">Notes for the app.</span></span>|
|<span data-ttu-id="24303-181">uploadState</span><span class="sxs-lookup"><span data-stu-id="24303-181">uploadState</span></span>|<span data-ttu-id="24303-182">Int32</span><span class="sxs-lookup"><span data-stu-id="24303-182">Int32</span></span>|<span data-ttu-id="24303-183">上载状态。</span><span class="sxs-lookup"><span data-stu-id="24303-183">The upload state.</span></span>|
|<span data-ttu-id="24303-184">publishingState</span><span class="sxs-lookup"><span data-stu-id="24303-184">publishingState</span></span>|[<span data-ttu-id="24303-185">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="24303-185">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="24303-186">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="24303-186">The publishing state for the app.</span></span> <span data-ttu-id="24303-187">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="24303-187">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="24303-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="24303-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="24303-189">isAssigned</span><span class="sxs-lookup"><span data-stu-id="24303-189">isAssigned</span></span>|<span data-ttu-id="24303-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="24303-190">Boolean</span></span>|<span data-ttu-id="24303-191">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="24303-191">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="24303-192">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24303-192">roleScopeTagIds</span></span>|<span data-ttu-id="24303-193">String 集合</span><span class="sxs-lookup"><span data-stu-id="24303-193">String collection</span></span>|<span data-ttu-id="24303-194">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="24303-194">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="24303-195">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="24303-195">dependentAppCount</span></span>|<span data-ttu-id="24303-196">Int32</span><span class="sxs-lookup"><span data-stu-id="24303-196">Int32</span></span>|<span data-ttu-id="24303-197">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="24303-197">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24303-198">关系</span><span class="sxs-lookup"><span data-stu-id="24303-198">Relationships</span></span>
|<span data-ttu-id="24303-199">关系</span><span class="sxs-lookup"><span data-stu-id="24303-199">Relationship</span></span>|<span data-ttu-id="24303-200">类型</span><span class="sxs-lookup"><span data-stu-id="24303-200">Type</span></span>|<span data-ttu-id="24303-201">说明</span><span class="sxs-lookup"><span data-stu-id="24303-201">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24303-202">**应用**</span><span class="sxs-lookup"><span data-stu-id="24303-202">**Apps**</span></span>|
|<span data-ttu-id="24303-203">categories</span><span class="sxs-lookup"><span data-stu-id="24303-203">categories</span></span>|<span data-ttu-id="24303-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24303-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="24303-205">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="24303-205">The list of categories for this app.</span></span>|
|<span data-ttu-id="24303-206">assignments</span><span class="sxs-lookup"><span data-stu-id="24303-206">assignments</span></span>|<span data-ttu-id="24303-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24303-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="24303-208">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="24303-208">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="24303-209">installSummary</span><span class="sxs-lookup"><span data-stu-id="24303-209">installSummary</span></span>|[<span data-ttu-id="24303-210">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="24303-210">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="24303-211">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="24303-211">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="24303-212">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="24303-212">deviceStatuses</span></span>|<span data-ttu-id="24303-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="24303-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="24303-214">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="24303-214">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="24303-215">userStatuses</span><span class="sxs-lookup"><span data-stu-id="24303-215">userStatuses</span></span>|<span data-ttu-id="24303-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="24303-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="24303-217">此移动应用程序的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="24303-217">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="24303-218">相互</span><span class="sxs-lookup"><span data-stu-id="24303-218">relationships</span></span>|<span data-ttu-id="24303-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合</span><span class="sxs-lookup"><span data-stu-id="24303-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="24303-220">此移动应用的关系列表。</span><span class="sxs-lookup"><span data-stu-id="24303-220">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24303-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24303-221">JSON Representation</span></span>
<span data-ttu-id="24303-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24303-222">Here is a JSON representation of the resource.</span></span>
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



