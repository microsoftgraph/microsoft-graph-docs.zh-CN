---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 64e012c25d1674bf3d4ce365aa13ac6a5600b755
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531092"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="61313-104">mobileAppContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="61313-104">mobileAppContent resource type</span></span>

<span data-ttu-id="61313-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61313-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61313-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61313-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61313-107">包含特定应用版本的内容属性。</span><span class="sxs-lookup"><span data-stu-id="61313-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="61313-108">每个 mobileAppContent 都可以具有多个 mobileAppContentFile。</span><span class="sxs-lookup"><span data-stu-id="61313-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="61313-109">Methods</span><span class="sxs-lookup"><span data-stu-id="61313-109">Methods</span></span>
|<span data-ttu-id="61313-110">方法</span><span class="sxs-lookup"><span data-stu-id="61313-110">Method</span></span>|<span data-ttu-id="61313-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="61313-111">Return Type</span></span>|<span data-ttu-id="61313-112">说明</span><span class="sxs-lookup"><span data-stu-id="61313-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61313-113">列出 mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="61313-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="61313-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61313-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="61313-115">列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61313-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="61313-116">获取 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="61313-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="61313-118">读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61313-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="61313-119">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="61313-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="61313-121">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61313-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="61313-122">删除 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="61313-123">无</span><span class="sxs-lookup"><span data-stu-id="61313-123">None</span></span>|<span data-ttu-id="61313-124">删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。</span><span class="sxs-lookup"><span data-stu-id="61313-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="61313-125">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="61313-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="61313-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="61313-127">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="61313-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="61313-128">属性</span><span class="sxs-lookup"><span data-stu-id="61313-128">Properties</span></span>
|<span data-ttu-id="61313-129">属性</span><span class="sxs-lookup"><span data-stu-id="61313-129">Property</span></span>|<span data-ttu-id="61313-130">类型</span><span class="sxs-lookup"><span data-stu-id="61313-130">Type</span></span>|<span data-ttu-id="61313-131">说明</span><span class="sxs-lookup"><span data-stu-id="61313-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61313-132">id</span><span class="sxs-lookup"><span data-stu-id="61313-132">id</span></span>|<span data-ttu-id="61313-133">字符串</span><span class="sxs-lookup"><span data-stu-id="61313-133">String</span></span>|<span data-ttu-id="61313-134">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="61313-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61313-135">关系</span><span class="sxs-lookup"><span data-stu-id="61313-135">Relationships</span></span>
|<span data-ttu-id="61313-136">关系</span><span class="sxs-lookup"><span data-stu-id="61313-136">Relationship</span></span>|<span data-ttu-id="61313-137">类型</span><span class="sxs-lookup"><span data-stu-id="61313-137">Type</span></span>|<span data-ttu-id="61313-138">说明</span><span class="sxs-lookup"><span data-stu-id="61313-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61313-139">files</span><span class="sxs-lookup"><span data-stu-id="61313-139">files</span></span>|<span data-ttu-id="61313-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61313-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="61313-141">此应用内容版本的文件列表。</span><span class="sxs-lookup"><span data-stu-id="61313-141">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61313-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61313-142">JSON Representation</span></span>
<span data-ttu-id="61313-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61313-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




