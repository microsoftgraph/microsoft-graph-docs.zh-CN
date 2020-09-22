---
title: managedApp 资源类型
description: 包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72cb905c266dba33c635dded929b32bc333705f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015417"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="71f89-103">managedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="71f89-103">managedApp resource type</span></span>

<span data-ttu-id="71f89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71f89-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71f89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71f89-106">包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="71f89-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="71f89-107">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="71f89-108">方法</span><span class="sxs-lookup"><span data-stu-id="71f89-108">Methods</span></span>
|<span data-ttu-id="71f89-109">方法</span><span class="sxs-lookup"><span data-stu-id="71f89-109">Method</span></span>|<span data-ttu-id="71f89-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="71f89-110">Return Type</span></span>|<span data-ttu-id="71f89-111">说明</span><span class="sxs-lookup"><span data-stu-id="71f89-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71f89-112">List managedApps</span><span class="sxs-lookup"><span data-stu-id="71f89-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="71f89-113">[managedApp](../resources/intune-apps-managedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71f89-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="71f89-114">列出 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71f89-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="71f89-115">Get managedApp</span><span class="sxs-lookup"><span data-stu-id="71f89-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="71f89-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="71f89-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="71f89-117">读取 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71f89-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71f89-118">属性</span><span class="sxs-lookup"><span data-stu-id="71f89-118">Properties</span></span>
|<span data-ttu-id="71f89-119">属性</span><span class="sxs-lookup"><span data-stu-id="71f89-119">Property</span></span>|<span data-ttu-id="71f89-120">类型</span><span class="sxs-lookup"><span data-stu-id="71f89-120">Type</span></span>|<span data-ttu-id="71f89-121">说明</span><span class="sxs-lookup"><span data-stu-id="71f89-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f89-122">id</span><span class="sxs-lookup"><span data-stu-id="71f89-122">id</span></span>|<span data-ttu-id="71f89-123">String</span><span class="sxs-lookup"><span data-stu-id="71f89-123">String</span></span>|<span data-ttu-id="71f89-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71f89-124">Key of the entity.</span></span> <span data-ttu-id="71f89-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-126">displayName</span><span class="sxs-lookup"><span data-stu-id="71f89-126">displayName</span></span>|<span data-ttu-id="71f89-127">String</span><span class="sxs-lookup"><span data-stu-id="71f89-127">String</span></span>|<span data-ttu-id="71f89-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="71f89-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="71f89-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-130">description</span><span class="sxs-lookup"><span data-stu-id="71f89-130">description</span></span>|<span data-ttu-id="71f89-131">String</span><span class="sxs-lookup"><span data-stu-id="71f89-131">String</span></span>|<span data-ttu-id="71f89-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="71f89-132">The description of the app.</span></span> <span data-ttu-id="71f89-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-134">publisher</span><span class="sxs-lookup"><span data-stu-id="71f89-134">publisher</span></span>|<span data-ttu-id="71f89-135">String</span><span class="sxs-lookup"><span data-stu-id="71f89-135">String</span></span>|<span data-ttu-id="71f89-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="71f89-136">The publisher of the app.</span></span> <span data-ttu-id="71f89-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="71f89-138">largeIcon</span></span>|[<span data-ttu-id="71f89-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71f89-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71f89-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="71f89-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="71f89-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71f89-142">createdDateTime</span></span>|<span data-ttu-id="71f89-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71f89-143">DateTimeOffset</span></span>|<span data-ttu-id="71f89-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71f89-144">The date and time the app was created.</span></span> <span data-ttu-id="71f89-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71f89-146">lastModifiedDateTime</span></span>|<span data-ttu-id="71f89-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71f89-147">DateTimeOffset</span></span>|<span data-ttu-id="71f89-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="71f89-148">The date and time the app was last modified.</span></span> <span data-ttu-id="71f89-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="71f89-150">isFeatured</span></span>|<span data-ttu-id="71f89-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="71f89-151">Boolean</span></span>|<span data-ttu-id="71f89-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="71f89-153">privacyInformationUrl</span></span>|<span data-ttu-id="71f89-154">String</span><span class="sxs-lookup"><span data-stu-id="71f89-154">String</span></span>|<span data-ttu-id="71f89-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="71f89-155">The privacy statement Url.</span></span> <span data-ttu-id="71f89-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="71f89-157">informationUrl</span></span>|<span data-ttu-id="71f89-158">String</span><span class="sxs-lookup"><span data-stu-id="71f89-158">String</span></span>|<span data-ttu-id="71f89-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="71f89-159">The more information Url.</span></span> <span data-ttu-id="71f89-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-161">所有者</span><span class="sxs-lookup"><span data-stu-id="71f89-161">owner</span></span>|<span data-ttu-id="71f89-162">String</span><span class="sxs-lookup"><span data-stu-id="71f89-162">String</span></span>|<span data-ttu-id="71f89-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="71f89-163">The owner of the app.</span></span> <span data-ttu-id="71f89-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-165">developer</span><span class="sxs-lookup"><span data-stu-id="71f89-165">developer</span></span>|<span data-ttu-id="71f89-166">String</span><span class="sxs-lookup"><span data-stu-id="71f89-166">String</span></span>|<span data-ttu-id="71f89-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="71f89-167">The developer of the app.</span></span> <span data-ttu-id="71f89-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-169">notes</span><span class="sxs-lookup"><span data-stu-id="71f89-169">notes</span></span>|<span data-ttu-id="71f89-170">String</span><span class="sxs-lookup"><span data-stu-id="71f89-170">String</span></span>|<span data-ttu-id="71f89-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="71f89-171">Notes for the app.</span></span> <span data-ttu-id="71f89-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="71f89-173">publishingState</span></span>|[<span data-ttu-id="71f89-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="71f89-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="71f89-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="71f89-175">The publishing state for the app.</span></span> <span data-ttu-id="71f89-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="71f89-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="71f89-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="71f89-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="71f89-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="71f89-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="71f89-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="71f89-179">appAvailability</span></span>|[<span data-ttu-id="71f89-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="71f89-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="71f89-181">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="71f89-181">The Application's availability.</span></span> <span data-ttu-id="71f89-182">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="71f89-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="71f89-183">version</span><span class="sxs-lookup"><span data-stu-id="71f89-183">version</span></span>|<span data-ttu-id="71f89-184">String</span><span class="sxs-lookup"><span data-stu-id="71f89-184">String</span></span>|<span data-ttu-id="71f89-185">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="71f89-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71f89-186">关系</span><span class="sxs-lookup"><span data-stu-id="71f89-186">Relationships</span></span>
|<span data-ttu-id="71f89-187">关系</span><span class="sxs-lookup"><span data-stu-id="71f89-187">Relationship</span></span>|<span data-ttu-id="71f89-188">类型</span><span class="sxs-lookup"><span data-stu-id="71f89-188">Type</span></span>|<span data-ttu-id="71f89-189">说明</span><span class="sxs-lookup"><span data-stu-id="71f89-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f89-190">categories</span><span class="sxs-lookup"><span data-stu-id="71f89-190">categories</span></span>|<span data-ttu-id="71f89-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71f89-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="71f89-192">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="71f89-192">The list of categories for this app.</span></span> <span data-ttu-id="71f89-193">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71f89-194">assignments</span><span class="sxs-lookup"><span data-stu-id="71f89-194">assignments</span></span>|<span data-ttu-id="71f89-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71f89-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="71f89-196">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="71f89-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="71f89-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71f89-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71f89-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71f89-198">JSON Representation</span></span>
<span data-ttu-id="71f89-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f89-199">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String"
}
```









