---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 69992ad07c5a0d97168db44cca8474c021d9a230
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947475"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="ecf53-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecf53-103">mobileApp resource type</span></span>

> <span data-ttu-id="ecf53-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ecf53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecf53-105">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="ecf53-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="ecf53-106">方法</span><span class="sxs-lookup"><span data-stu-id="ecf53-106">Methods</span></span>
|<span data-ttu-id="ecf53-107">方法</span><span class="sxs-lookup"><span data-stu-id="ecf53-107">Method</span></span>|<span data-ttu-id="ecf53-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ecf53-108">Return Type</span></span>|<span data-ttu-id="ecf53-109">说明</span><span class="sxs-lookup"><span data-stu-id="ecf53-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ecf53-110">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="ecf53-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="ecf53-111">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ecf53-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="ecf53-112">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ecf53-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="ecf53-113">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="ecf53-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="ecf53-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="ecf53-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="ecf53-115">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ecf53-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="ecf53-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="ecf53-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="ecf53-117">无</span><span class="sxs-lookup"><span data-stu-id="ecf53-117">None</span></span>|<span data-ttu-id="ecf53-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ecf53-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ecf53-119">属性</span><span class="sxs-lookup"><span data-stu-id="ecf53-119">Properties</span></span>
|<span data-ttu-id="ecf53-120">属性</span><span class="sxs-lookup"><span data-stu-id="ecf53-120">Property</span></span>|<span data-ttu-id="ecf53-121">类型</span><span class="sxs-lookup"><span data-stu-id="ecf53-121">Type</span></span>|<span data-ttu-id="ecf53-122">说明</span><span class="sxs-lookup"><span data-stu-id="ecf53-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf53-123">id</span><span class="sxs-lookup"><span data-stu-id="ecf53-123">id</span></span>|<span data-ttu-id="ecf53-124">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-124">String</span></span>|<span data-ttu-id="ecf53-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ecf53-125">Key of the entity.</span></span>|
|<span data-ttu-id="ecf53-126">displayName</span><span class="sxs-lookup"><span data-stu-id="ecf53-126">displayName</span></span>|<span data-ttu-id="ecf53-127">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-127">String</span></span>|<span data-ttu-id="ecf53-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ecf53-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="ecf53-129">description</span><span class="sxs-lookup"><span data-stu-id="ecf53-129">description</span></span>|<span data-ttu-id="ecf53-130">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-130">String</span></span>|<span data-ttu-id="ecf53-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ecf53-131">The description of the app.</span></span>|
|<span data-ttu-id="ecf53-132">publisher</span><span class="sxs-lookup"><span data-stu-id="ecf53-132">publisher</span></span>|<span data-ttu-id="ecf53-133">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-133">String</span></span>|<span data-ttu-id="ecf53-134">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ecf53-134">The publisher of the app.</span></span>|
|<span data-ttu-id="ecf53-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ecf53-135">largeIcon</span></span>|[<span data-ttu-id="ecf53-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ecf53-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ecf53-137">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ecf53-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="ecf53-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf53-138">createdDateTime</span></span>|<span data-ttu-id="ecf53-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf53-139">DateTimeOffset</span></span>|<span data-ttu-id="ecf53-140">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ecf53-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="ecf53-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecf53-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ecf53-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecf53-142">DateTimeOffset</span></span>|<span data-ttu-id="ecf53-143">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ecf53-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="ecf53-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ecf53-144">isFeatured</span></span>|<span data-ttu-id="ecf53-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecf53-145">Boolean</span></span>|<span data-ttu-id="ecf53-146">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="ecf53-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="ecf53-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ecf53-147">privacyInformationUrl</span></span>|<span data-ttu-id="ecf53-148">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-148">String</span></span>|<span data-ttu-id="ecf53-149">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="ecf53-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="ecf53-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ecf53-150">informationUrl</span></span>|<span data-ttu-id="ecf53-151">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-151">String</span></span>|<span data-ttu-id="ecf53-152">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="ecf53-152">The more information Url.</span></span>|
|<span data-ttu-id="ecf53-153">owner</span><span class="sxs-lookup"><span data-stu-id="ecf53-153">owner</span></span>|<span data-ttu-id="ecf53-154">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-154">String</span></span>|<span data-ttu-id="ecf53-155">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ecf53-155">The owner of the app.</span></span>|
|<span data-ttu-id="ecf53-156">developer</span><span class="sxs-lookup"><span data-stu-id="ecf53-156">developer</span></span>|<span data-ttu-id="ecf53-157">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-157">String</span></span>|<span data-ttu-id="ecf53-158">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ecf53-158">The developer of the app.</span></span>|
|<span data-ttu-id="ecf53-159">notes</span><span class="sxs-lookup"><span data-stu-id="ecf53-159">notes</span></span>|<span data-ttu-id="ecf53-160">String</span><span class="sxs-lookup"><span data-stu-id="ecf53-160">String</span></span>|<span data-ttu-id="ecf53-161">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ecf53-161">Notes for the app.</span></span>|
|<span data-ttu-id="ecf53-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="ecf53-162">publishingState</span></span>|[<span data-ttu-id="ecf53-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ecf53-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ecf53-164">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ecf53-164">The publishing state for the app.</span></span> <span data-ttu-id="ecf53-165">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ecf53-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ecf53-166">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ecf53-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecf53-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="ecf53-167">Relationships</span></span>
|<span data-ttu-id="ecf53-168">关系</span><span class="sxs-lookup"><span data-stu-id="ecf53-168">Relationship</span></span>|<span data-ttu-id="ecf53-169">类型</span><span class="sxs-lookup"><span data-stu-id="ecf53-169">Type</span></span>|<span data-ttu-id="ecf53-170">说明</span><span class="sxs-lookup"><span data-stu-id="ecf53-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecf53-171">categories</span><span class="sxs-lookup"><span data-stu-id="ecf53-171">categories</span></span>|<span data-ttu-id="ecf53-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ecf53-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="ecf53-173">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="ecf53-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="ecf53-174">assignments</span><span class="sxs-lookup"><span data-stu-id="ecf53-174">assignments</span></span>|<span data-ttu-id="ecf53-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ecf53-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="ecf53-176">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="ecf53-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecf53-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecf53-177">JSON Representation</span></span>
<span data-ttu-id="ecf53-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecf53-178">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```



