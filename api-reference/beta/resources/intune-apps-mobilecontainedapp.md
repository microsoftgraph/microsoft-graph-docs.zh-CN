---
title: mobileContainedApp 资源类型
description: 一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3400349244e738644d4885b2265c5f7f4ceb84e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145197"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="7e8b6-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e8b6-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="7e8b6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e8b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e8b6-106">一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="7e8b6-107">方法</span><span class="sxs-lookup"><span data-stu-id="7e8b6-107">Methods</span></span>
|<span data-ttu-id="7e8b6-108">方法</span><span class="sxs-lookup"><span data-stu-id="7e8b6-108">Method</span></span>|<span data-ttu-id="7e8b6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e8b6-109">Return Type</span></span>|<span data-ttu-id="7e8b6-110">说明</span><span class="sxs-lookup"><span data-stu-id="7e8b6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e8b6-111">列出 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="7e8b6-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="7e8b6-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e8b6-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="7e8b6-113">列出[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="7e8b6-114">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="7e8b6-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="7e8b6-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="7e8b6-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="7e8b6-116">读取[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e8b6-117">属性</span><span class="sxs-lookup"><span data-stu-id="7e8b6-117">Properties</span></span>
|<span data-ttu-id="7e8b6-118">属性</span><span class="sxs-lookup"><span data-stu-id="7e8b6-118">Property</span></span>|<span data-ttu-id="7e8b6-119">类型</span><span class="sxs-lookup"><span data-stu-id="7e8b6-119">Type</span></span>|<span data-ttu-id="7e8b6-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e8b6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e8b6-121">id</span><span class="sxs-lookup"><span data-stu-id="7e8b6-121">id</span></span>|<span data-ttu-id="7e8b6-122">String</span><span class="sxs-lookup"><span data-stu-id="7e8b6-122">String</span></span>|<span data-ttu-id="7e8b6-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e8b6-124">关系</span><span class="sxs-lookup"><span data-stu-id="7e8b6-124">Relationships</span></span>
<span data-ttu-id="7e8b6-125">无</span><span class="sxs-lookup"><span data-stu-id="7e8b6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e8b6-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e8b6-126">JSON Representation</span></span>
<span data-ttu-id="7e8b6-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e8b6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




