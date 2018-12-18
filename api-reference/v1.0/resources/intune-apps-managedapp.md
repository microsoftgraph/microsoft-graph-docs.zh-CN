---
title: managedApp 资源类型
description: 包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。
author: tfitzmac
ms.openlocfilehash: e7a86e9b22939fedb3def43099d756c714c411da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343986"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="b00fb-103">managedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="b00fb-103">managedApp resource type</span></span>

> <span data-ttu-id="b00fb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b00fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b00fb-105">包含可以使用 Intune 应用保护策略管理的应用的属性和继承属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="b00fb-105">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>

<span data-ttu-id="b00fb-106">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b00fb-107">方法</span><span class="sxs-lookup"><span data-stu-id="b00fb-107">Methods</span></span>
|<span data-ttu-id="b00fb-108">方法</span><span class="sxs-lookup"><span data-stu-id="b00fb-108">Method</span></span>|<span data-ttu-id="b00fb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b00fb-109">Return Type</span></span>|<span data-ttu-id="b00fb-110">说明</span><span class="sxs-lookup"><span data-stu-id="b00fb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b00fb-111">List managedApps</span><span class="sxs-lookup"><span data-stu-id="b00fb-111">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="b00fb-112">[managedApp](../resources/intune-apps-managedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b00fb-112">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="b00fb-113">列出 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b00fb-113">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="b00fb-114">Get managedApp</span><span class="sxs-lookup"><span data-stu-id="b00fb-114">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="b00fb-115">managedApp</span><span class="sxs-lookup"><span data-stu-id="b00fb-115">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="b00fb-116">读取 [managedApp](../resources/intune-apps-managedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b00fb-116">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b00fb-117">属性</span><span class="sxs-lookup"><span data-stu-id="b00fb-117">Properties</span></span>
|<span data-ttu-id="b00fb-118">属性</span><span class="sxs-lookup"><span data-stu-id="b00fb-118">Property</span></span>|<span data-ttu-id="b00fb-119">类型</span><span class="sxs-lookup"><span data-stu-id="b00fb-119">Type</span></span>|<span data-ttu-id="b00fb-120">说明</span><span class="sxs-lookup"><span data-stu-id="b00fb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00fb-121">id</span><span class="sxs-lookup"><span data-stu-id="b00fb-121">id</span></span>|<span data-ttu-id="b00fb-122">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-122">String</span></span>|<span data-ttu-id="b00fb-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b00fb-123">Key of the entity.</span></span> <span data-ttu-id="b00fb-124">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-125">displayName</span><span class="sxs-lookup"><span data-stu-id="b00fb-125">displayName</span></span>|<span data-ttu-id="b00fb-126">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-126">String</span></span>|<span data-ttu-id="b00fb-127">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b00fb-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b00fb-128">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-129">description</span><span class="sxs-lookup"><span data-stu-id="b00fb-129">description</span></span>|<span data-ttu-id="b00fb-130">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-130">String</span></span>|<span data-ttu-id="b00fb-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b00fb-131">The description of the app.</span></span> <span data-ttu-id="b00fb-132">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-133">publisher</span><span class="sxs-lookup"><span data-stu-id="b00fb-133">publisher</span></span>|<span data-ttu-id="b00fb-134">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-134">String</span></span>|<span data-ttu-id="b00fb-135">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b00fb-135">The publisher of the app.</span></span> <span data-ttu-id="b00fb-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b00fb-137">largeIcon</span></span>|[<span data-ttu-id="b00fb-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b00fb-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b00fb-139">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b00fb-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b00fb-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b00fb-141">createdDateTime</span></span>|<span data-ttu-id="b00fb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b00fb-142">DateTimeOffset</span></span>|<span data-ttu-id="b00fb-143">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b00fb-143">The date and time the app was created.</span></span> <span data-ttu-id="b00fb-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b00fb-145">lastModifiedDateTime</span></span>|<span data-ttu-id="b00fb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b00fb-146">DateTimeOffset</span></span>|<span data-ttu-id="b00fb-147">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b00fb-147">The date and time the app was last modified.</span></span> <span data-ttu-id="b00fb-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b00fb-149">isFeatured</span></span>|<span data-ttu-id="b00fb-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00fb-150">Boolean</span></span>|<span data-ttu-id="b00fb-151">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b00fb-152">privacyInformationUrl</span></span>|<span data-ttu-id="b00fb-153">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-153">String</span></span>|<span data-ttu-id="b00fb-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="b00fb-154">The privacy statement Url.</span></span> <span data-ttu-id="b00fb-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b00fb-156">informationUrl</span></span>|<span data-ttu-id="b00fb-157">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-157">String</span></span>|<span data-ttu-id="b00fb-158">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="b00fb-158">The more information Url.</span></span> <span data-ttu-id="b00fb-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-160">owner</span><span class="sxs-lookup"><span data-stu-id="b00fb-160">owner</span></span>|<span data-ttu-id="b00fb-161">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-161">String</span></span>|<span data-ttu-id="b00fb-162">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b00fb-162">The owner of the app.</span></span> <span data-ttu-id="b00fb-163">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-164">developer</span><span class="sxs-lookup"><span data-stu-id="b00fb-164">developer</span></span>|<span data-ttu-id="b00fb-165">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-165">String</span></span>|<span data-ttu-id="b00fb-166">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b00fb-166">The developer of the app.</span></span> <span data-ttu-id="b00fb-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-168">notes</span><span class="sxs-lookup"><span data-stu-id="b00fb-168">notes</span></span>|<span data-ttu-id="b00fb-169">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-169">String</span></span>|<span data-ttu-id="b00fb-170">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b00fb-170">Notes for the app.</span></span> <span data-ttu-id="b00fb-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="b00fb-172">publishingState</span></span>|[<span data-ttu-id="b00fb-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b00fb-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b00fb-174">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b00fb-174">The publishing state for the app.</span></span> <span data-ttu-id="b00fb-175">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b00fb-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b00fb-176">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b00fb-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b00fb-177">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b00fb-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b00fb-178">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b00fb-178">appAvailability</span></span>|[<span data-ttu-id="b00fb-179">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b00fb-179">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b00fb-180">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="b00fb-180">The Application's availability.</span></span> <span data-ttu-id="b00fb-181">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="b00fb-181">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b00fb-182">version</span><span class="sxs-lookup"><span data-stu-id="b00fb-182">version</span></span>|<span data-ttu-id="b00fb-183">String</span><span class="sxs-lookup"><span data-stu-id="b00fb-183">String</span></span>|<span data-ttu-id="b00fb-184">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="b00fb-184">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b00fb-185">关系</span><span class="sxs-lookup"><span data-stu-id="b00fb-185">Relationships</span></span>
|<span data-ttu-id="b00fb-186">关系</span><span class="sxs-lookup"><span data-stu-id="b00fb-186">Relationship</span></span>|<span data-ttu-id="b00fb-187">类型</span><span class="sxs-lookup"><span data-stu-id="b00fb-187">Type</span></span>|<span data-ttu-id="b00fb-188">说明</span><span class="sxs-lookup"><span data-stu-id="b00fb-188">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00fb-189">categories</span><span class="sxs-lookup"><span data-stu-id="b00fb-189">categories</span></span>|<span data-ttu-id="b00fb-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b00fb-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="b00fb-191">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="b00fb-191">The list of categories for this app.</span></span> <span data-ttu-id="b00fb-192">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b00fb-193">assignments</span><span class="sxs-lookup"><span data-stu-id="b00fb-193">assignments</span></span>|<span data-ttu-id="b00fb-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b00fb-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="b00fb-195">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="b00fb-195">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="b00fb-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b00fb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b00fb-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b00fb-197">JSON Representation</span></span>
<span data-ttu-id="b00fb-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b00fb-198">Here is a JSON representation of the resource.</span></span>
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



