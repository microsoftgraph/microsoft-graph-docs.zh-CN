---
title: mobileContainedApp 资源类型
description: 一个抽象类，表示充当包的 mobileApp 中包含的应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ebe9834cc527fe79b4fcd920927dfb70fa42db5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48719748"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="85441-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="85441-103">mobileContainedApp resource type</span></span>

<span data-ttu-id="85441-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85441-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85441-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85441-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85441-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85441-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85441-107">一个抽象类，表示充当包的 mobileApp 中包含的应用程序。</span><span class="sxs-lookup"><span data-stu-id="85441-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="85441-108">Methods</span><span class="sxs-lookup"><span data-stu-id="85441-108">Methods</span></span>
|<span data-ttu-id="85441-109">方法</span><span class="sxs-lookup"><span data-stu-id="85441-109">Method</span></span>|<span data-ttu-id="85441-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="85441-110">Return Type</span></span>|<span data-ttu-id="85441-111">说明</span><span class="sxs-lookup"><span data-stu-id="85441-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85441-112">列出 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="85441-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="85441-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85441-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="85441-114">列出 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="85441-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="85441-115">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="85441-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="85441-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="85441-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="85441-117">读取 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="85441-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85441-118">属性</span><span class="sxs-lookup"><span data-stu-id="85441-118">Properties</span></span>
|<span data-ttu-id="85441-119">属性</span><span class="sxs-lookup"><span data-stu-id="85441-119">Property</span></span>|<span data-ttu-id="85441-120">类型</span><span class="sxs-lookup"><span data-stu-id="85441-120">Type</span></span>|<span data-ttu-id="85441-121">说明</span><span class="sxs-lookup"><span data-stu-id="85441-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85441-122">id</span><span class="sxs-lookup"><span data-stu-id="85441-122">id</span></span>|<span data-ttu-id="85441-123">String</span><span class="sxs-lookup"><span data-stu-id="85441-123">String</span></span>|<span data-ttu-id="85441-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85441-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85441-125">关系</span><span class="sxs-lookup"><span data-stu-id="85441-125">Relationships</span></span>
<span data-ttu-id="85441-126">无</span><span class="sxs-lookup"><span data-stu-id="85441-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85441-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85441-127">JSON Representation</span></span>
<span data-ttu-id="85441-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85441-128">Here is a JSON representation of the resource.</span></span>
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





