---
title: managedApp 资源类型
description: 包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fbb934f3bb52c1980908c1595c2252800c465e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756048"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="6de6a-103">managedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6de6a-103">managedApp resource type</span></span>

<span data-ttu-id="6de6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6de6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6de6a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6de6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6de6a-106">包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="6de6a-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="6de6a-107">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6de6a-108">Methods</span><span class="sxs-lookup"><span data-stu-id="6de6a-108">Methods</span></span>
|<span data-ttu-id="6de6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="6de6a-109">Method</span></span>|<span data-ttu-id="6de6a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6de6a-110">Return Type</span></span>|<span data-ttu-id="6de6a-111">Description</span><span class="sxs-lookup"><span data-stu-id="6de6a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6de6a-112">List managedApps</span><span class="sxs-lookup"><span data-stu-id="6de6a-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="6de6a-113">[managedApp](../resources/intune-apps-managedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6de6a-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="6de6a-114">列出 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6de6a-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="6de6a-115">Get managedApp</span><span class="sxs-lookup"><span data-stu-id="6de6a-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="6de6a-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="6de6a-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="6de6a-117">读取 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6de6a-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6de6a-118">属性</span><span class="sxs-lookup"><span data-stu-id="6de6a-118">Properties</span></span>
|<span data-ttu-id="6de6a-119">属性</span><span class="sxs-lookup"><span data-stu-id="6de6a-119">Property</span></span>|<span data-ttu-id="6de6a-120">类型</span><span class="sxs-lookup"><span data-stu-id="6de6a-120">Type</span></span>|<span data-ttu-id="6de6a-121">说明</span><span class="sxs-lookup"><span data-stu-id="6de6a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de6a-122">id</span><span class="sxs-lookup"><span data-stu-id="6de6a-122">id</span></span>|<span data-ttu-id="6de6a-123">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-123">String</span></span>|<span data-ttu-id="6de6a-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6de6a-124">Key of the entity.</span></span> <span data-ttu-id="6de6a-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-126">displayName</span><span class="sxs-lookup"><span data-stu-id="6de6a-126">displayName</span></span>|<span data-ttu-id="6de6a-127">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-127">String</span></span>|<span data-ttu-id="6de6a-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="6de6a-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6de6a-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-130">说明</span><span class="sxs-lookup"><span data-stu-id="6de6a-130">description</span></span>|<span data-ttu-id="6de6a-131">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-131">String</span></span>|<span data-ttu-id="6de6a-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6de6a-132">The description of the app.</span></span> <span data-ttu-id="6de6a-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-134">publisher</span><span class="sxs-lookup"><span data-stu-id="6de6a-134">publisher</span></span>|<span data-ttu-id="6de6a-135">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-135">String</span></span>|<span data-ttu-id="6de6a-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="6de6a-136">The publisher of the app.</span></span> <span data-ttu-id="6de6a-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6de6a-138">largeIcon</span></span>|[<span data-ttu-id="6de6a-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6de6a-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6de6a-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="6de6a-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6de6a-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6de6a-142">createdDateTime</span></span>|<span data-ttu-id="6de6a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6de6a-143">DateTimeOffset</span></span>|<span data-ttu-id="6de6a-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6de6a-144">The date and time the app was created.</span></span> <span data-ttu-id="6de6a-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6de6a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6de6a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6de6a-147">DateTimeOffset</span></span>|<span data-ttu-id="6de6a-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6de6a-148">The date and time the app was last modified.</span></span> <span data-ttu-id="6de6a-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6de6a-150">isFeatured</span></span>|<span data-ttu-id="6de6a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="6de6a-151">Boolean</span></span>|<span data-ttu-id="6de6a-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6de6a-153">privacyInformationUrl</span></span>|<span data-ttu-id="6de6a-154">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-154">String</span></span>|<span data-ttu-id="6de6a-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="6de6a-155">The privacy statement Url.</span></span> <span data-ttu-id="6de6a-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6de6a-157">informationUrl</span></span>|<span data-ttu-id="6de6a-158">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-158">String</span></span>|<span data-ttu-id="6de6a-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="6de6a-159">The more information Url.</span></span> <span data-ttu-id="6de6a-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-161">所有者</span><span class="sxs-lookup"><span data-stu-id="6de6a-161">owner</span></span>|<span data-ttu-id="6de6a-162">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-162">String</span></span>|<span data-ttu-id="6de6a-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="6de6a-163">The owner of the app.</span></span> <span data-ttu-id="6de6a-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-165">developer</span><span class="sxs-lookup"><span data-stu-id="6de6a-165">developer</span></span>|<span data-ttu-id="6de6a-166">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-166">String</span></span>|<span data-ttu-id="6de6a-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="6de6a-167">The developer of the app.</span></span> <span data-ttu-id="6de6a-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-169">notes</span><span class="sxs-lookup"><span data-stu-id="6de6a-169">notes</span></span>|<span data-ttu-id="6de6a-170">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-170">String</span></span>|<span data-ttu-id="6de6a-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="6de6a-171">Notes for the app.</span></span> <span data-ttu-id="6de6a-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="6de6a-173">publishingState</span></span>|[<span data-ttu-id="6de6a-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6de6a-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6de6a-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6de6a-175">The publishing state for the app.</span></span> <span data-ttu-id="6de6a-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="6de6a-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6de6a-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6de6a-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6de6a-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="6de6a-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6de6a-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6de6a-179">appAvailability</span></span>|[<span data-ttu-id="6de6a-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="6de6a-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6de6a-181">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="6de6a-181">The Application's availability.</span></span> <span data-ttu-id="6de6a-182">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="6de6a-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6de6a-183">version</span><span class="sxs-lookup"><span data-stu-id="6de6a-183">version</span></span>|<span data-ttu-id="6de6a-184">String</span><span class="sxs-lookup"><span data-stu-id="6de6a-184">String</span></span>|<span data-ttu-id="6de6a-185">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="6de6a-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6de6a-186">关系</span><span class="sxs-lookup"><span data-stu-id="6de6a-186">Relationships</span></span>
|<span data-ttu-id="6de6a-187">关系</span><span class="sxs-lookup"><span data-stu-id="6de6a-187">Relationship</span></span>|<span data-ttu-id="6de6a-188">类型</span><span class="sxs-lookup"><span data-stu-id="6de6a-188">Type</span></span>|<span data-ttu-id="6de6a-189">Description</span><span class="sxs-lookup"><span data-stu-id="6de6a-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6de6a-190">categories</span><span class="sxs-lookup"><span data-stu-id="6de6a-190">categories</span></span>|<span data-ttu-id="6de6a-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6de6a-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="6de6a-192">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="6de6a-192">The list of categories for this app.</span></span> <span data-ttu-id="6de6a-193">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6de6a-194">assignments</span><span class="sxs-lookup"><span data-stu-id="6de6a-194">assignments</span></span>|<span data-ttu-id="6de6a-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6de6a-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="6de6a-196">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="6de6a-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="6de6a-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6de6a-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6de6a-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6de6a-198">JSON Representation</span></span>
<span data-ttu-id="6de6a-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6de6a-199">Here is a JSON representation of the resource.</span></span>
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




