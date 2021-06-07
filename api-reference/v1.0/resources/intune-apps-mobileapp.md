---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1682c08e4fb15de6e5fc9d66d86d83c832e4c27
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752418"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="12535-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="12535-103">mobileApp resource type</span></span>

<span data-ttu-id="12535-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12535-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12535-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12535-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12535-106">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="12535-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="12535-107">Methods</span><span class="sxs-lookup"><span data-stu-id="12535-107">Methods</span></span>
|<span data-ttu-id="12535-108">方法</span><span class="sxs-lookup"><span data-stu-id="12535-108">Method</span></span>|<span data-ttu-id="12535-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="12535-109">Return Type</span></span>|<span data-ttu-id="12535-110">Description</span><span class="sxs-lookup"><span data-stu-id="12535-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12535-111">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="12535-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="12535-112">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12535-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="12535-113">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12535-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="12535-114">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="12535-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="12535-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="12535-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="12535-116">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12535-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="12535-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="12535-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="12535-118">无</span><span class="sxs-lookup"><span data-stu-id="12535-118">None</span></span>|<span data-ttu-id="12535-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="12535-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="12535-120">属性</span><span class="sxs-lookup"><span data-stu-id="12535-120">Properties</span></span>
|<span data-ttu-id="12535-121">属性</span><span class="sxs-lookup"><span data-stu-id="12535-121">Property</span></span>|<span data-ttu-id="12535-122">类型</span><span class="sxs-lookup"><span data-stu-id="12535-122">Type</span></span>|<span data-ttu-id="12535-123">说明</span><span class="sxs-lookup"><span data-stu-id="12535-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12535-124">id</span><span class="sxs-lookup"><span data-stu-id="12535-124">id</span></span>|<span data-ttu-id="12535-125">String</span><span class="sxs-lookup"><span data-stu-id="12535-125">String</span></span>|<span data-ttu-id="12535-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12535-126">Key of the entity.</span></span>|
|<span data-ttu-id="12535-127">displayName</span><span class="sxs-lookup"><span data-stu-id="12535-127">displayName</span></span>|<span data-ttu-id="12535-128">String</span><span class="sxs-lookup"><span data-stu-id="12535-128">String</span></span>|<span data-ttu-id="12535-129">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="12535-129">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="12535-130">说明</span><span class="sxs-lookup"><span data-stu-id="12535-130">description</span></span>|<span data-ttu-id="12535-131">String</span><span class="sxs-lookup"><span data-stu-id="12535-131">String</span></span>|<span data-ttu-id="12535-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="12535-132">The description of the app.</span></span>|
|<span data-ttu-id="12535-133">publisher</span><span class="sxs-lookup"><span data-stu-id="12535-133">publisher</span></span>|<span data-ttu-id="12535-134">String</span><span class="sxs-lookup"><span data-stu-id="12535-134">String</span></span>|<span data-ttu-id="12535-135">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="12535-135">The publisher of the app.</span></span>|
|<span data-ttu-id="12535-136">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12535-136">largeIcon</span></span>|[<span data-ttu-id="12535-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12535-137">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="12535-138">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="12535-138">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="12535-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12535-139">createdDateTime</span></span>|<span data-ttu-id="12535-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12535-140">DateTimeOffset</span></span>|<span data-ttu-id="12535-141">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12535-141">The date and time the app was created.</span></span>|
|<span data-ttu-id="12535-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12535-142">lastModifiedDateTime</span></span>|<span data-ttu-id="12535-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12535-143">DateTimeOffset</span></span>|<span data-ttu-id="12535-144">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="12535-144">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="12535-145">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12535-145">isFeatured</span></span>|<span data-ttu-id="12535-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="12535-146">Boolean</span></span>|<span data-ttu-id="12535-147">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="12535-147">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="12535-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12535-148">privacyInformationUrl</span></span>|<span data-ttu-id="12535-149">String</span><span class="sxs-lookup"><span data-stu-id="12535-149">String</span></span>|<span data-ttu-id="12535-150">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="12535-150">The privacy statement Url.</span></span>|
|<span data-ttu-id="12535-151">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12535-151">informationUrl</span></span>|<span data-ttu-id="12535-152">String</span><span class="sxs-lookup"><span data-stu-id="12535-152">String</span></span>|<span data-ttu-id="12535-153">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="12535-153">The more information Url.</span></span>|
|<span data-ttu-id="12535-154">所有者</span><span class="sxs-lookup"><span data-stu-id="12535-154">owner</span></span>|<span data-ttu-id="12535-155">String</span><span class="sxs-lookup"><span data-stu-id="12535-155">String</span></span>|<span data-ttu-id="12535-156">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="12535-156">The owner of the app.</span></span>|
|<span data-ttu-id="12535-157">developer</span><span class="sxs-lookup"><span data-stu-id="12535-157">developer</span></span>|<span data-ttu-id="12535-158">String</span><span class="sxs-lookup"><span data-stu-id="12535-158">String</span></span>|<span data-ttu-id="12535-159">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="12535-159">The developer of the app.</span></span>|
|<span data-ttu-id="12535-160">notes</span><span class="sxs-lookup"><span data-stu-id="12535-160">notes</span></span>|<span data-ttu-id="12535-161">String</span><span class="sxs-lookup"><span data-stu-id="12535-161">String</span></span>|<span data-ttu-id="12535-162">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="12535-162">Notes for the app.</span></span>|
|<span data-ttu-id="12535-163">publishingState</span><span class="sxs-lookup"><span data-stu-id="12535-163">publishingState</span></span>|[<span data-ttu-id="12535-164">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12535-164">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="12535-165">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="12535-165">The publishing state for the app.</span></span> <span data-ttu-id="12535-166">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="12535-166">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12535-167">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="12535-167">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12535-168">关系</span><span class="sxs-lookup"><span data-stu-id="12535-168">Relationships</span></span>
|<span data-ttu-id="12535-169">关系</span><span class="sxs-lookup"><span data-stu-id="12535-169">Relationship</span></span>|<span data-ttu-id="12535-170">类型</span><span class="sxs-lookup"><span data-stu-id="12535-170">Type</span></span>|<span data-ttu-id="12535-171">Description</span><span class="sxs-lookup"><span data-stu-id="12535-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12535-172">categories</span><span class="sxs-lookup"><span data-stu-id="12535-172">categories</span></span>|<span data-ttu-id="12535-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12535-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="12535-174">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="12535-174">The list of categories for this app.</span></span>|
|<span data-ttu-id="12535-175">assignments</span><span class="sxs-lookup"><span data-stu-id="12535-175">assignments</span></span>|<span data-ttu-id="12535-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12535-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="12535-177">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="12535-177">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12535-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12535-178">JSON Representation</span></span>
<span data-ttu-id="12535-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12535-179">Here is a JSON representation of the resource.</span></span>
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




