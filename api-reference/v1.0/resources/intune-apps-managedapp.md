---
title: managedApp 资源类型
description: 包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 32094696c2e2c84c9c40cfb1c1c3df525159f4ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835733"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="c6c91-103">managedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6c91-103">managedApp resource type</span></span>

> <span data-ttu-id="c6c91-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6c91-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6c91-105">包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="c6c91-105">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>

<span data-ttu-id="c6c91-106">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c6c91-107">方法</span><span class="sxs-lookup"><span data-stu-id="c6c91-107">Methods</span></span>
|<span data-ttu-id="c6c91-108">方法</span><span class="sxs-lookup"><span data-stu-id="c6c91-108">Method</span></span>|<span data-ttu-id="c6c91-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6c91-109">Return Type</span></span>|<span data-ttu-id="c6c91-110">说明</span><span class="sxs-lookup"><span data-stu-id="c6c91-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6c91-111">List managedApps</span><span class="sxs-lookup"><span data-stu-id="c6c91-111">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="c6c91-112">[managedApp](../resources/intune-apps-managedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6c91-112">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="c6c91-113">列出 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6c91-113">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="c6c91-114">Get managedApp</span><span class="sxs-lookup"><span data-stu-id="c6c91-114">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="c6c91-115">managedApp</span><span class="sxs-lookup"><span data-stu-id="c6c91-115">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="c6c91-116">读取 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6c91-116">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6c91-117">属性</span><span class="sxs-lookup"><span data-stu-id="c6c91-117">Properties</span></span>
|<span data-ttu-id="c6c91-118">属性</span><span class="sxs-lookup"><span data-stu-id="c6c91-118">Property</span></span>|<span data-ttu-id="c6c91-119">类型</span><span class="sxs-lookup"><span data-stu-id="c6c91-119">Type</span></span>|<span data-ttu-id="c6c91-120">说明</span><span class="sxs-lookup"><span data-stu-id="c6c91-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c91-121">id</span><span class="sxs-lookup"><span data-stu-id="c6c91-121">id</span></span>|<span data-ttu-id="c6c91-122">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-122">String</span></span>|<span data-ttu-id="c6c91-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c6c91-123">Key of the entity.</span></span> <span data-ttu-id="c6c91-124">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-125">displayName</span><span class="sxs-lookup"><span data-stu-id="c6c91-125">displayName</span></span>|<span data-ttu-id="c6c91-126">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-126">String</span></span>|<span data-ttu-id="c6c91-127">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c6c91-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c6c91-128">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-129">description</span><span class="sxs-lookup"><span data-stu-id="c6c91-129">description</span></span>|<span data-ttu-id="c6c91-130">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-130">String</span></span>|<span data-ttu-id="c6c91-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c6c91-131">The description of the app.</span></span> <span data-ttu-id="c6c91-132">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-133">publisher</span><span class="sxs-lookup"><span data-stu-id="c6c91-133">publisher</span></span>|<span data-ttu-id="c6c91-134">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-134">String</span></span>|<span data-ttu-id="c6c91-135">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c6c91-135">The publisher of the app.</span></span> <span data-ttu-id="c6c91-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c6c91-137">largeIcon</span></span>|[<span data-ttu-id="c6c91-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c6c91-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c6c91-139">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c6c91-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c6c91-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c91-141">createdDateTime</span></span>|<span data-ttu-id="c6c91-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c91-142">DateTimeOffset</span></span>|<span data-ttu-id="c6c91-143">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6c91-143">The date and time the app was created.</span></span> <span data-ttu-id="c6c91-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c91-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c6c91-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c91-146">DateTimeOffset</span></span>|<span data-ttu-id="c6c91-147">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c6c91-147">The date and time the app was last modified.</span></span> <span data-ttu-id="c6c91-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c6c91-149">isFeatured</span></span>|<span data-ttu-id="c6c91-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6c91-150">Boolean</span></span>|<span data-ttu-id="c6c91-151">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c6c91-152">privacyInformationUrl</span></span>|<span data-ttu-id="c6c91-153">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-153">String</span></span>|<span data-ttu-id="c6c91-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c6c91-154">The privacy statement Url.</span></span> <span data-ttu-id="c6c91-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c6c91-156">informationUrl</span></span>|<span data-ttu-id="c6c91-157">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-157">String</span></span>|<span data-ttu-id="c6c91-158">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="c6c91-158">The more information Url.</span></span> <span data-ttu-id="c6c91-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-160">owner</span><span class="sxs-lookup"><span data-stu-id="c6c91-160">owner</span></span>|<span data-ttu-id="c6c91-161">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-161">String</span></span>|<span data-ttu-id="c6c91-162">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c6c91-162">The owner of the app.</span></span> <span data-ttu-id="c6c91-163">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-164">developer</span><span class="sxs-lookup"><span data-stu-id="c6c91-164">developer</span></span>|<span data-ttu-id="c6c91-165">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-165">String</span></span>|<span data-ttu-id="c6c91-166">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c6c91-166">The developer of the app.</span></span> <span data-ttu-id="c6c91-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-168">notes</span><span class="sxs-lookup"><span data-stu-id="c6c91-168">notes</span></span>|<span data-ttu-id="c6c91-169">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-169">String</span></span>|<span data-ttu-id="c6c91-170">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c6c91-170">Notes for the app.</span></span> <span data-ttu-id="c6c91-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="c6c91-172">publishingState</span></span>|[<span data-ttu-id="c6c91-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c6c91-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c6c91-174">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c6c91-174">The publishing state for the app.</span></span> <span data-ttu-id="c6c91-175">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c6c91-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c6c91-176">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c6c91-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c6c91-177">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c6c91-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c6c91-178">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c6c91-178">appAvailability</span></span>|[<span data-ttu-id="c6c91-179">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c6c91-179">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c6c91-180">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="c6c91-180">The Application's availability.</span></span> <span data-ttu-id="c6c91-181">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="c6c91-181">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c6c91-182">version</span><span class="sxs-lookup"><span data-stu-id="c6c91-182">version</span></span>|<span data-ttu-id="c6c91-183">String</span><span class="sxs-lookup"><span data-stu-id="c6c91-183">String</span></span>|<span data-ttu-id="c6c91-184">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="c6c91-184">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6c91-185">关系</span><span class="sxs-lookup"><span data-stu-id="c6c91-185">Relationships</span></span>
|<span data-ttu-id="c6c91-186">关系</span><span class="sxs-lookup"><span data-stu-id="c6c91-186">Relationship</span></span>|<span data-ttu-id="c6c91-187">类型</span><span class="sxs-lookup"><span data-stu-id="c6c91-187">Type</span></span>|<span data-ttu-id="c6c91-188">说明</span><span class="sxs-lookup"><span data-stu-id="c6c91-188">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c91-189">categories</span><span class="sxs-lookup"><span data-stu-id="c6c91-189">categories</span></span>|<span data-ttu-id="c6c91-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6c91-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="c6c91-191">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="c6c91-191">The list of categories for this app.</span></span> <span data-ttu-id="c6c91-192">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6c91-193">assignments</span><span class="sxs-lookup"><span data-stu-id="c6c91-193">assignments</span></span>|<span data-ttu-id="c6c91-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6c91-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c6c91-195">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="c6c91-195">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="c6c91-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6c91-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6c91-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6c91-197">JSON Representation</span></span>
<span data-ttu-id="c6c91-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6c91-198">Here is a JSON representation of the resource.</span></span>
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



